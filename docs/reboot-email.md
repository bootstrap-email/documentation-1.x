---
layout: docs
title:  "Reboot Email"
tagline: "Consistent email reset to level out the playing field."
---
Similar to Bootstraps Reboot, Reboot Email set styles to try and normalize the differences between email clients so the base email is as consistent as possible. Here is the Reboot Email file which is influenced greatly by the [Mailchimp email reset](https://templates.mailchimp.com/development/css/reset-styles/).

```scss
body, .body {
  margin: 0;
  Margin: 0; // For compatibility with Outlook
  padding: 0;
  border: 0;
  outline: 0;
  width: 100%;
  min-width: 100%;
  height: 100%;
  -webkit-text-size-adjust: 100%;
  -ms-text-size-adjust: 100%;
  font-family: $font-family-base;
  line-height: $line-height-base * $font-size-base;
  font-weight: $font-weight-base;
  font-size: $font-size-base;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
  background-color: $body-bg;
  color: $body-color;
}

img {
  border: 0 none;
  height: auto;
  line-height: 100%;
  outline: none;
  text-decoration: none;
  display: block;
}

// to fix centering in yahoo
table[align=center] {
  margin: 0 auto;
}

th,
td,
p {
  text-align: left;
  line-height: $line-height-base * $font-size-base;
  font-size: $font-size-base;
  margin: 0;
}

a {
  color: $link-color;
}

```
