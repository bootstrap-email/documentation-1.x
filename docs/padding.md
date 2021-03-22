---
layout: docs
title:  "Padding"
tagline: "Add padding to table cells"
sections:
  - Class Reference
  - Usage
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
        <tr><td class="class">.p-{{ spacing }}</td><td class="css">padding: {{ spacing | times: 4 }}px;</td></tr>
        <tr><td class="class">.px-{{ spacing }}</td><td class="css">padding-left: {{ spacing | times: 4 }}px; padding-right: {{ spacing | times: 4 }}px;</td></tr>
        <tr><td class="class">.py-{{ spacing }}</td><td class="css">padding-top: {{ spacing | times: 4 }}px; padding-bottom: {{ spacing | times: 4 }}px;</td></tr>
        <tr><td class="class">.pt-{{ spacing }}</td><td class="css">padding-top: {{ spacing | times: 4 }}px;</td></tr>
        <tr><td class="class">.pr-{{ spacing }}</td><td class="css">padding-right: {{ spacing | times: 4 }}px;</td></tr>
        <tr><td class="class">.pb-{{ spacing }}</td><td class="css">padding-bottom: {{ spacing | times: 4 }}px;</td></tr>
        <tr><td class="class">.pl-{{ spacing }}</td><td class="css">padding-left: {{ spacing | times: 4 }}px;</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
There are two types of spacing Bootstrap Email supports. Padding (applied to the inside of table cells) and [Margin](/docs/margin) (in the form of vertical spacers which are used to take up space between elements vertically).
```html
<a class="btn btn-primary p-3" href="http://bootstrapemail.com">A Button with lots of padding</a>
```

<a class="btn btn-primary p-3" href="http://bootstrapemail.com">A Button with lots of padding</a>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<a class="btn btn-primary p-5" href="http://example.com">Button with mega padding</a>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="btn btn-primary p-5" role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-radius: 6px; border-collapse: separate !important;">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; border-radius: 6px; margin: 0;" align="center" bgcolor="#0d6efd">
        <a href="http://example.com" style="color: #ffffff; font-size: 16px; font-family: Helvetica, Arial, sans-serif; text-decoration: none; border-radius: 6px; line-height: 20px; display: inline-block; font-weight: normal; white-space: nowrap; background-color: #0d6efd; padding: 20px; border: 1px solid #0d6efd;">Button with mega padding</a>
      </td>
    </tr>
  </tbody>
</table>
```
