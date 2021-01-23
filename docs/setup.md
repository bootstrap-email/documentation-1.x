---
layout: docs
title:  "Setup"
badges: false
---
#### Environment Support
- [Command Line](#command-line)
- [Ruby](#ruby)
- [Ruby on Rails](#ruby-on-rails)
- [Online editor](https://editor.bootstrapemail.com)

___

#### Command Line

[Ruby](#) is required to be installed on the machine you are using to run Bootstrap Email.

1: Install bootstrap email via [Ruby Gems](#)
```bash
gem install bootstrap-email
```

2: There are many ways to use the command line to compile emails:
```bash
# compile all files in the current directory
bootstrap-email
# compile the file email.html and save it to the file out.html
bootstrap-email email.html > out.html
# compile a relative path to a file
bootstrap-email ./public/index.html
# specify a path pattern and a destination directory for compiled emails to be saved to
bootstrap-email -p 'emails/*' -d emails/output
# compile for a string
bootstrap-email -s '<a href="#" class="btn btn-primary">Some Button</a>'
# pipe a file into bootstrap-email
cat input.html | bootstrap-email
# specify config path to use to customize things like colors
bootstrap-email -c bootstrap-email.scss
```

Help: run the command `bootstrap-email -h` for help on all options.

#### Rails Setup

Setup with Rails could not be easier.

1: Add Bootstrap Email to your `Gemfile`

```ruby
gem 'bootstrap-email'
```

2: You need to create the mailer template which will wrap the email content. Create the file `/app/views/layouts/bootstrap-mailer.html.erb` and paste this HTML into it. (It is very similar to the default mailer).

```erb
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html>
  <head>
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
    <%= stylesheet_link_tag "application-mailer", media: "all" %>
  </head>
  <body class="bg-light">
    <%= yield %>
  </body>
</html>
```

3: Specify the layout for the actions you want to build with bootstrap email. You can specify it for all with ApplicationMailer.
```ruby
class ApplicationMailer < ActionMailer::Base
  layout 'bootstrap-mailer'
end
```
Refer to the [official ActionMailer documentation](http://guides.rubyonrails.org/action_mailer_basics.html#action-mailer-layouts) on more info about using a different layout for different mailers.

4: Create a new stylesheet `/app/assets/stylesheets/application-mailer.scss` and import `bootstrap-email`. This is where your custom styles and overrides that you want to be inlined should live.

```sass
@import 'bootstrap-email';
```

5: Add this line in `/config/initializers/asset.rb` to compile your new SASS file.

```ruby
Rails.application.config.assets.precompile += %w( application-mailer.scss )
```

6: Create the view file `/app/views/example_mailer/greet.html.erb`.

You can also create the view `/app/views/example_mailer/greet.text.erb`. In this case don't forget to create also the textual layout `/app/views/layouts/example_mailer.text.erb`.

If you do  not create a textual view file, a text part is automatically added by the `premailer-rails` gem.

#### Usage
Thats it! Now all you need to do to use it instead of using the `mail()` method, you use the `make_bootstrap_mail()` method to kick off Bootstrap Email compilation!

```ruby
class ExampleMailer < ApplicationMailer

  def greet
    bootstrap_mail(
      to: 'to@example.com',
      from: 'from@example.com',
      subject: 'Hi From Bootstrap Email',
    )
  end
end
```

You can also use the `format` in the usual way.
```ruby
class ExampleMailer < ApplicationMailer

  def greet
    bootstrap_mail(
      to: 'to@example.com',
      from: 'from@example.com',
      subject: 'Hi From Bootstrap Email',
      ) do |format|
        format.html { layout 'custom_bootstrap_layout' }
        format.text # here example_mailer.text.erb is used
      end
  end
end
```
