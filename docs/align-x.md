---
layout: docs
title:  "Align X"
tagline: "Align any content horizontally on the X axis."
sections:
  - Class Reference
  - Usage
  - Compiled Example
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
      <tr><td class="class">.ax-left</td><td class="result">align horizontally left</td></tr>
      <tr><td class="class">.ax-right</td><td class="result">align horizontally right</td></tr>
      <tr><td class="class">.ax-center</td><td class="result">align horizontally center</td></tr>
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Align uses the `align="left|center|right` property on `table` to align anything horizontally. When it is used with a `table` or `td` it will put that property directly on them, however if it is used on any other tag it will wrap that element with a `table` and align it accordingly.
```html
<div class="ax-left">Align left on all viewport sizes</div><br>
<div class="ax-right">Align right on all viewport sizes</div><br>
<div class="ax-center">Align center on all viewport sizes</div>
<a class="btn btn-primary ax-right" href="http://bootstrapemail.com">Right Aligned Button</a>
```

<div class="float-start">Align left on all viewport sizes</div><br>
<div class="float-end">Align right on all viewport sizes</div><br>
<div class="d-table mx-auto position-relative">Align center on all viewport sizes</div>
<a class="btn btn-primary float-end" href="http://bootstrapemail.com">Right Aligned Button</a>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="ax-left">Hello</div>
<div class="ax-center">WOWWWWW</div>
<div class="ax-right">Goodbye</div>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="ax-left" role="presentation" align="left">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; margin: 0;" align="left">
        <div class="">Hello</div>
      </td>
    </tr>
  </tbody>
</table>

<table class="ax-center" role="presentation" align="center" style="margin: 0 auto;">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; margin: 0;" align="left">
        <div class="">WOWWWWW</div>
      </td>
    </tr>
  </tbody>
</table>

<table class="ax-right" role="presentation" align="right">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; margin: 0;" align="left">
        <div class="">Goodbye</div>
      </td>
    </tr>
  </tbody>
</table>
```

