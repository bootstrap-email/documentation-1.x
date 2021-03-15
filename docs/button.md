---
layout: docs
title:  "Button"
tagline: "Turn a link into a button."
sections:
  - Class Reference
  - Usage
  - Outline
  - Sizes
  - Compiled Example
badges: true
themeable: true
responsive: false
---
<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">.btn</td><td class="result">the base button class to setup structure</td></tr>
      {% for item in site.data.theme_colors %}
        <tr><td class="class">.btn-{{ item.name }}</td><td class="result">background-color: {{ item.color }};</td></tr>
      {% endfor %}
      {% for item in site.data.palette_colors %}
        <tr><td class="class">.btn-{{ item.name }}</td><td class="result">background-color: {{ item.color }};</td></tr>
      {% endfor %}
      {% for item in site.data.theme_colors %}
        <tr><td class="class">.btn-outline-{{ item.name }}</td><td class="result">border-color: {{ item.color }}; text-color: {{ item.color }}; background-color: transparent;</td></tr>
      {% endfor %}
      {% for item in site.data.palette_colors %}
        <tr><td class="class">.btn-outline-{{ item.name }}</td><td class="result">border-color: {{ item.color }}; text-color: {{ item.color }}; background-color: transparent;</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Buttons are **ONLY** to be used with an anchor `<a>` tag. The there are classes for all the theme and palette colors, so you can use `btn-primary` as well as `btn-blue-300`.

```html
<a class="btn btn-primary" href="https://bootstrapemail.com">Primary</a>
<a class="btn btn-secondary" href="https://bootstrapemail.com">Secondary</a>
<a class="btn btn-success" href="https://bootstrapemail.com">Success</a>
<a class="btn btn-danger" href="https://bootstrapemail.com">Danger</a>
<a class="btn btn-warning" href="https://bootstrapemail.com">Warning</a>
<a class="btn btn-info" href="https://bootstrapemail.com">Info</a>
<a class="btn btn-light" href="https://bootstrapemail.com">Light</a>
<a class="btn btn-dark" href="https://bootstrapemail.com">Dark</a>
```

<a href="#" class="btn btn-primary">Primary</a>
<a href="#" class="btn btn-secondary">Secondary</a>
<a href="#" class="btn btn-success">Success</a>
<a href="#" class="btn btn-danger">Danger</a>
<a href="#" class="btn btn-warning">Warning</a>
<a href="#" class="btn btn-info">Info</a>
<a href="#" class="btn btn-light">Light</a>
<a href="#" class="btn btn-dark">Dark</a>

<div class="alert alert-warning">
  <strong>Warning:</strong> You must supply a url in the href. Using just pound sign is not enough for some emails to render an anchor tag correctly.
</div>

{% include header.html name="Usage" hr="false" %}
You can use *outlined* versions of every button by simply adding the `outline` keyword to the class like `btn-outline-primary` or `btn-outline-green-300`.

```html
<a class="btn btn-outline-primary" href="https://bootstrapemail.com">Primary</a>
<a class="btn btn-outline-green-300" href="https://bootstrapemail.com">Green</a>
```
<a class="btn btn-outline-primary" href="https://bootstrapemail.com">Primary</a>
<a class="btn btn-outline-success" href="https://bootstrapemail.com">Green</a>

{% include header.html name="Sizes" hr="true" %}
You can use `btn-sm` or `btn-lg` for smaller or larger buttons and text respectively. If you want to just adjust the padding size of a button you can use the [Padding](/docs/padding) utility classes.
```html
<a class="btn btn-primary btn-sm" href="https://bootstrapemail.com">Large button</a>
<a class="btn btn-primary btn-lg" href="https://bootstrapemail.com">Large button</a>
```

<a class="btn btn-primary btn-sm" href="https://bootstrapemail.com">Large button</a>
<a class="btn btn-primary btn-lg" href="https://bootstrapemail.com">Large button</a>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<a class="btn btn-primary" href="https://example.com">Click Me</a>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="btn btn-primary" role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-radius: 6px; border-collapse: separate !important;">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; border-radius: 6px; margin: 0;" align="center" bgcolor="#0d6efd">
        <a href="https://example.com" style="color: #ffffff; font-size: 16px; font-family: Helvetica, Arial, sans-serif; text-decoration: none; border-radius: 6px; line-height: 20px; display: inline-block; font-weight: normal; white-space: nowrap; background-color: #0d6efd; padding: 8px 12px; border: 1px solid #0d6efd;">Click Me</a>
      </td>
    </tr>
  </tbody>
</table>
```
