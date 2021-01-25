---
layout: docs
title:  "Customize"
badges: false
---
If you want to customize styles like colors or spacing or even want to add custom styles to be compiled with the SCSS and inlined into your email you can use a config file. By default Bootstrap Email will look for a `bootstrap-email.config.scss` file in the root of the working directory / project.
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

#### Path to config
If you want to put your config file in a different location or use a different name other than the default you can:
- Using the CLI:
```bash
bootstrap-email -c path/to/bootstrap-email.config.scss
```
- Using Ruby:
```ruby
html = '<div>Hello</div>'
path = File.expand_path('path/to/bootstrap-email.config.scss', __dir__)
BootstrapEmail::Compiler.new(html, options: {config_path: path}).perform_full_compile
```
- Using Rails
```
Bootstrap email will also look in `app/assets/stylesheets/bootstrap-email.config.scss` for the file.
```
