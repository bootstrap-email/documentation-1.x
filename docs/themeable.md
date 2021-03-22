---
layout: docs
title:  "Themeable"
---
When you see the
<span class="d-inline-block">
  <a href="/docs/themeable" class="badge m-0 d-flex align-items-center compatibility-badge">
    <span class="badge-check">
      <img src="/img/icons/check.svg" />
    </span>
    <span>Themeable</span>
  </a>
</span> badge it means the component has the following classes that you can use color the component. Just like Bootstrap, the convention is `{component}-{theme-color}`.

```html
{component}-primary
{component}-secondary
{component}-success
{component}-danger
{component}-warning
{component}-info
{component}-light
{component}-dark
```

Bootstrap Email uses the same default color scheme that Bootstrap 4 does.
<div class="themable-example text-white bg-primary">primary</div>
<div class="themable-example text-white bg-secondary">secondary</div>
<div class="themable-example text-white bg-success">success</div>
<div class="themable-example text-white bg-danger">danger</div>
<div class="themable-example bg-warning">warning</div>
<div class="themable-example text-white bg-info">info</div>
<div class="themable-example bg-light">light</div>
<div class="themable-example text-white bg-dark">dark</div>

<style>
  .themable-example{
    width: 100px;
    height: 100px;
    border-radius: 10px;
    display: inline-block;
    margin: 0 1rem 1rem 0;
    padding: 2.25rem 0;
    text-align: center;
  }
</style>

#### Customize Theme

Bootstrap Email makes is really easy to customize the theme colors. You can override each color in your sass file before the `bootstrap-email` import:
```scss
$theme-primary: #007bff;
$theme-secondary: #868e96;
$theme-success: #28a745;
$theme-danger: #dc3545;
$theme-warning: #ffc107;
$theme-info: #17a2b8;
$theme-light: #f8f9fa;
$theme-dark: #343a40;

@import 'bootstrap-email';
```

Note: These are the current defaults for the theme colors.
