---
layout: docs
title:  "Text Align"
tagline: "Give text alignment."
sections:
  - Class Reference
  - Usage
  - Compiled Example
badges: true
themeable: false
responsive: false
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
      <tr><td class="class">.text-left</td><td class="css">text-align: left;</td></tr>
      <tr><td class="class">.text-right</td><td class="css">text-align: right;</td></tr>
      <tr><td class="class">.text-center</td><td class="css">text-align: center;</td></tr>
      <tr><td class="class">.text-justify</td><td class="css">text-align: justify;</td></tr>
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
A simple way to adjust the line height of text.
```html
<div class="text-left">This text is to the left</div>
<div class="text-center">This text is to the center</div>
<div class="text-right">This text is to the right</div>
<div class="text-justify">This text is justified which means it fills the whole line when it wraps so the start and end of the text with touch both the left and right side.</div>
```

<div class="text-start">This text is to the left</div>
<div class="text-center">This text is to the center</div>
<div class="text-end">This text is to the right</div>
<div style="text-align: justify;">This text is justified which means it fills the whole line when it wraps so the start and end of the text with touch both the left and right side.</div>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="text-left">This text is to the left</div>
<div class="text-center">This text is to the center</div>
<div class="text-right">This text is to the right</div>
<div class="text-justify">This text is justified which means it fills the whole line when it wraps so the start and end of the text with touch both the left and right side.</div>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<div class="text-left" style="" align="left">This text is to the left</div>
<div class="text-center" style="" align="center">This text is to the center</div>
<div class="text-right" style="" align="right">This text is to the right</div>
<div class="text-justify" style="" align="justify">This text is justified which means it fills the whole line when it wraps so the start and end of the text with touch both the left and right side.</div>
```
