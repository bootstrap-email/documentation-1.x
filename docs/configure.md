---
layout: docs
title:  "Configure"
tagline: "Configure settings, colors, and default styles using SASS variables."
sections:
  - Config
  - Config Path
  - Customize Sass
  - Additional Methods
---
{% include header.html name="Config" hr="false" %}
Configure different aspects of Bootstrap Email. It will look for a file in the working directory for `bootstrap_email.config.rb`. If you are using Rails, put this file in `config/initializers/bootstrap_email.rb`. Here is a list of the config options that you can customize.
```ruby
BootstrapEmail.configure do |config|
  # Defaults to ./bootstrap-email.scss or ./app/assets/stylesheets/bootstrap-email.scss in rails
  config.sass_email_location = File.expand_path('path/to/bootstrap-email.scss', __dir__)
  # Defaults to ./bootstrap-head.scss or ./app/assets/stylesheets/bootstrap-head.scss in rails
  config.sass_head_location = File.expand_path('path/to/bootstrap-head.scss', __dir__)
  # Array of folders to add to the SASS load path to support imports in the custom SASS files
  config.sass_load_paths = [File.expand_path('some/folder', __dir__)]
  # Defaults to ./.sass-cache or ./tmp/cache/bootstrap-email/.sass-cache in rails
  config.sass_cache_location = [File.expand_path('some/folder', __dir__)]
  # Defaults to true, is disabled during CLI commands that output to standard out
  config.sass_log_enabled = true
end
```

{% include header.html name="Config Path" hr="true" %}
If you want to provide a path to a config file, you can use the `options: {config_path: 'path'}}` option in the `BoostrapEmail::Compiler.new()` method or with the `-c` flag via the CLI.
- Using the CLI:
```bash
bootstrap-email -c path/to/bootstrap-email.config.rb
```
- Using Ruby:
```ruby
html = '<div>Hello</div>'
path = File.expand_path('path/to/bootstrap-email.config.rb', __dir__)
BootstrapEmail::Compiler.new(html, options: {config_path: path}).perform_full_compile
```
Also any config above, `sass_email_location` for example, can be passed in via the `options` hash.

{% include header.html name="Customize Sass" hr="true" %}
If you want to customize styles like colors or spacing or even want to add custom styles to be compiled with the SCSS and inlined into your email you can use a config file. By default Bootstrap Email will look for a `bootstrap-email.scss` file in the root of the working directory / project.

Here are the 3 files of SASS variables that you can customize by overriding:
1. [General Variables](https://github.com/bootstrap-email/bootstrap-email/blob/master/core/scss/_variables.scss)
2. [Color Variables](https://github.com/bootstrap-email/bootstrap-email/blob/master/core/scss/_colors.scss)
2. [Utility Variables](https://github.com/bootstrap-email/bootstrap-email/blob/master/core/scss/_utilities.scss)

This is what a basic config file should contain:
```scss
//= @import bootstrap-email;
```

 This allows you to customize all you want surrounding the base SCSS that gets pulled in. Here is an example of setting different colors to be used:
```scss
// Override all colors to black
$primary: #000000;
$secondary: #000000;
$success: #000000;
$info: #000000;
$warning: #000000;
$danger: #000000;
$light: #000000;
$dark: #000000;

//= @import bootstrap-email;

// Make all links pink
a {
  color: pink;
}
```
For more examples of variables that can be overridden check out the SCSS files for [colors](https://github.com/bootstrap-email/bootstrap-email/blob/v1-dev/core/scss/_colors.scss), [utilities](https://github.com/bootstrap-email/bootstrap-email/blob/v1-dev/core/scss/_utilities.scss), and [variables](https://github.com/bootstrap-email/bootstrap-email/blob/v1-dev/core/scss/_variables.scss)

{% include header.html name="Additional Methods" hr="true" %}

`BootstrapEmail.reset_config!` to reset all the configuration.

`BootstrapEmail.clear_sass_cache!` to clear the cached sass files.
