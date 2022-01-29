---
layout: docs
title:  "Usage"
sections:
  - Command Line
  - Ruby
  - Ruby on Rails
  - Online editor
---
#### Environment Support
- [Command Line](#command-line)
- [Ruby](#ruby)
- [Ruby on Rails](#ruby-on-rails)
- [Online editor](#online-editor)

{% include header.html name="Command Line" hr="false" %}

[Ruby](https://www.ruby-lang.org/en/documentation/installation/) is required to be installed on the machine you are using to run Bootstrap Email.

1: Install bootstrap email via [Ruby Gems](https://rubygems.org/gems/bootstrap-email)
```bash
gem install bootstrap-email
```

2: There are many ways to use the command line to compile emails:
```bash
# compile all files ending in .html in the current directory
bootstrap-email
# compile the file email.html and save it to the file out.html
bootstrap-email email.html > out.html
# compile a relative path to a file
bootstrap-email ./public/index.html
# specify a path pattern and a destination directory for compiled emails to be saved to
bootstrap-email -p 'emails/*' -d 'emails/compiled/*'
# compile for a string
bootstrap-email -s '<a href="#" class="btn btn-primary">Some Button</a>'
# pipe a file into bootstrap-email
cat input.html | bootstrap-email
# specify config path to use to customize things like colors
bootstrap-email -c bootstrap-email.scss
```

Help: run the command `bootstrap-email -h` for help on all options.

{% include header.html name="Ruby" hr="false" %}

1: Add Bootstrap Email to your `Gemfile`

```ruby
gem 'bootstrap-email'
```

2: Usage is simple, there are two ways to call Bootstrap Email, string and file.
```ruby
# Pass in any html string or html document as a string
html = '<a href="#" class="btn btn-primary">A button</a>'
BootstrapEmail::Compiler.new(html).perform_full_compile

# Pass in a full path to a file
file_path = File.expand_path('path/to/a/file.html', __dir__)
BootstrapEmail::Compiler.new(file_path, type: :file).perform_full_compile
```

{% include header.html name="Ruby on Rails" hr="false" %}

1: Add Bootstrap Email to your `Gemfile`

```ruby
gem 'bootstrap-email'
```

2: You need to create the mailer template which will wrap the email content. Create the file `/app/views/layouts/bootstrap-mailer.html.erb` and paste this HTML into it. (It is very similar to the default mailer).
```erb
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html lang="en">
  <head>
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
    <meta name="x-apple-disable-message-reformatting">
    <meta http-equiv="x-ua-compatible" content="ie=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="format-detection" content="telephone=no, date=no, address=no, email=no">
  </head>
  <body>
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

<!-- 4: Create a new stylesheet `/app/assets/stylesheets/application-mailer.scss` and import `bootstrap-email`. This is where your custom styles and overrides that you want to be inlined should live.

```sass
@import 'bootstrap-email';
```

5: Add this line in `/config/initializers/asset.rb` to compile your new SASS file.

```ruby
Rails.application.config.assets.precompile += %w( application-mailer.scss )
```

6: Create the view file `/app/views/example_mailer/greet.html.erb`.

You can also create the view `/app/views/example_mailer/greet.text.erb`. In this case don't forget to create also the textual layout `/app/views/layouts/example_mailer.text.erb`.

If you do  not create a textual view file, a text part is automatically added by the `premailer-rails` gem. -->


4: That's it! Now all you need to do to use it instead of using the `mail()` method, you use the `bootstrap_mail()` method to kick off Bootstrap Email compilation!

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

{% include header.html name="Online editor" hr="false" %}
An easier, but less integrated and customizable way to use Bootstrap Email is the online editor.
- Write an email and test it's rendering quickly
- Test on desktop and mobile responsive device widths
- Save emails to your account to come back to
- Send test emails directly to your inbox

<a href="https://app.bootstrapemail.com/editor?version=1" class="btn btn-purple my-3">Try the Online Editor</a>
<img class="w-100" src="/img/editor.png" />
