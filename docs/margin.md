---
layout: docs
title:  "Margin"
tagline: 'Set vertical "margin" between elements.'
sections:
  - Class Reference
  - Margin Usage
  - Spacer Usage
  - Compiled Example
responsive: true
---
<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Properties</th>
      </tr>
    </thead>
    <tbody>
      {% for spacing in site.data.spacings %}
        <tr><td class="class">.my-{{ spacing }}</td><td class="result">Make a {{ spacing | times: 4 }}px spacer above and below</td></tr>
        <tr><td class="class">.mt-{{ spacing }}</td><td class="result">Make a {{ spacing | times: 4 }}px spacer above</td></tr>
        <tr><td class="class">.mb-{{ spacing }}</td><td class="result">Make a {{ spacing | times: 4 }}px spacer below</td></tr>
      {% endfor %}
      {% for spacing in site.data.spacings %}
        <tr><td class="class">.s-{{ spacing }}</td><td class="result">Make a spacer {{ spacing | times: 4 }}px tall</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>
Note: Margin is only supported on the top and bottom.

{% include header.html name="Margin Usage" hr="false" %}
There are two types of spacing Bootstrap Email supports. [Padding](/docs/padding) (applied to the inside of table cells) and [Margin](/docs/margin) (in the form of vertical spacers which are used to take up space between elements vertically).

Margin is very inconsistently supported in email clients. Instead of using `margin` in css the margin classes create spacers above and/or below and element for simpler syntax like Bootstrap. This example adds a spacer of 12px above and below the middle card. See [space between](/docs/space-between) for more info on adding spacers between elements.
```html
<div class="card card-body">Top Card</div>
<div class="card card-body my-3">Middle Card (with margin above and below)</div>
<div class="card card-body">Bottom Card</div>
```

<div class="card card-body">Top Card</div>
<div class="card card-body my-3">Middle Card (with margin about and below)</div>
<div class="card card-body">Bottom Card</div>

{% include header.html name="Spacer Usage" hr="true" %}
```html
<div class="s-3"></div>
```
Spacers hold not content, they are just put into the document to sit between elements in a vertical flow.

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<a class="btn btn-primary my-3" href="http://example.com">Button with mega margin</a>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="s-3 w-full" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%;" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 12px; font-size: 12px; width: 100%; height: 12px; margin: 0;" align="left" width="100%" height="12">
         
      </td>
    </tr>
  </tbody>
</table>
<table class="btn btn-primary" role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-radius: 6px; border-collapse: separate !important;">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; border-radius: 6px; margin: 0;" align="center" bgcolor="#0d6efd">
        <a href="http://example.com" style="color: #ffffff; font-size: 16px; font-family: Helvetica, Arial, sans-serif; text-decoration: none; border-radius: 6px; line-height: 20px; display: inline-block; font-weight: normal; white-space: nowrap; background-color: #0d6efd; padding: 8px 12px; border: 1px solid #0d6efd;">Button with mega margin</a>
      </td>
    </tr>
  </tbody>
</table>
<table class="s-3 w-full" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%;" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 12px; font-size: 12px; width: 100%; height: 12px; margin: 0;" align="left" width="100%" height="12">
         
      </td>
    </tr>
  </tbody>
</table>
```
