---
layout: docs
title:  "Stack"
tagline: "Similar to flexbox but built with tables."
sections:
  - Class Reference
  - Usage
  - Gap
  - Alignment
  - Compiled Example
responsive: true
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
      <tr><td class="class">.stack-x</td><td class="result">generate a horizontals stack</td></tr>
      <tr><td class="class">.stack-y</td><td class="result">generate a vertical stack</td></tr>
      <tr><td class="class">.stack-align-left</td><td class="css">text-align: left;</td></tr>
      <tr><td class="class">.stack-align-center</td><td class="css">text-align: center;</td></tr>
      <tr><td class="class">.stack-align-right</td><td class="css">text-align: right;</td></tr>
      <tr><td class="class">.stack-valign-top</td><td class="css">vertical-align: top;</td></tr>
      <tr><td class="class">.stack-valign-middle</td><td class="css">vertical-align: middle;</td></tr>
      <tr><td class="class">.stack-valign-bottom</td><td class="css">vertical-align: bottom;</td></tr>
      <tr><td class="class">.stack-valign-baseline</td><td class="css">vertical-align: baseline;</td></tr>
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Stacks work similar to the way flexbox does to lay children elements out in a row or a column. To use a stack, all you need to do a wrap children elements in either a `stack-x` for row or a `stack-y` for a column.

```html
<div class="stack-x">
  <div>Lay a group of things</div>
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
  <div>Out horizontally</div>
</div>
```

<div class="d-flex">
  <div>Lay a group of things</div>
  <img style="width: 40px;" src="/img/icons/logo.png" />
  <div>Out horizontally</div>
</div>

{% include header.html name="Gap" hr="true" %}
Stacks are made really useful when combined with [Gaps](/docs/gap). Using a gap you can space a few icons out.

```html
<div class="stack-x gap-4">
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
</div>
<div class="stack-x gap-16">
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
</div>
```

<div class="d-flex">
  <img style="width: 40px; margin-right: 16px;" src="/img/icons/logo.png" />
  <img style="width: 40px; margin-right: 16px;" src="/img/icons/logo.png" />
  <img style="width: 40px;" src="/img/icons/logo.png" />
</div>
<div class="d-flex">
  <img style="width: 40px; margin-right: 64px;" src="/img/icons/logo.png" />
  <img style="width: 40px; margin-right: 64px;" src="/img/icons/logo.png" />
  <img style="width: 40px;" src="/img/icons/logo.png" />
</div>

{% include header.html name="Alignment" hr="true" %}
Stacks use HTMl tables to generate their layouts, that means we can use the power of table cells to align their contents horizontally and vertically. The classes `stack-align-left`, `stack-align-center`, and `stack-align-right` center contents horizontally (**Note: you must either you an inline or inline-block child element for this to work as expected**). The classes `stack-valign-top`, `stack-valign-middle`, `stack-valign-bottom`, and `stack-valign-baseline` are for vertical alignment of child elements. By default everything defaults to top left alignment.

```html
<div class="stack-x gap-4">
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-20" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
</div>
<div class="stack-x gap-4 stack-valign-bottom">
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-20" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
</div>
<div class="stack-x gap-4 stack-valign-middle">
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-20" src="https://bootstrapemail.com/some/image.jpg" />
  <img class="w-10" src="https://bootstrapemail.com/some/image.jpg" />
</div>
```
<div class="d-flex align-items-start">
  <img style="width: 40px; margin-right: 16px;" src="/img/icons/logo.png" />
  <img style="width: 80px; margin-right: 16px;" src="/img/icons/logo.png" />
  <img style="width: 40px;" src="/img/icons/logo.png" />
</div>
<div class="d-flex align-items-end">
  <img style="width: 40px; margin-right: 16px;" src="/img/icons/logo.png" />
  <img style="width: 80px; margin-right: 16px;" src="/img/icons/logo.png" />
  <img style="width: 40px;" src="/img/icons/logo.png" />
</div>
<div class="d-flex align-items-center">
  <img style="width: 40px; margin-right: 16px;" src="/img/icons/logo.png" />
  <img style="width: 80px; margin-right: 16px;" src="/img/icons/logo.png" />
  <img style="width: 40px;" src="/img/icons/logo.png" />
</div>


{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="stack-x gap-10">
  <div>stack item 1</div>
  <div>stack item 2</div>
  <div>stack item 3</div>
  <div>stack item 4</div>
  <div>stack item 5</div>
  <div>stack item 6</div>
</div>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="stack-x gap-10" role="presentation" border="0" cellpadding="0" cellspacing="0">
  <tbody>
    <tr>
      <td class="stack-cell" style="line-height: 24px; font-size: 16px; padding-right: 40px; margin: 0;" align="left" valign="top">
        <div>stack item 1</div>
      </td>
      <td class="stack-cell" style="line-height: 24px; font-size: 16px; padding-right: 40px; margin: 0;" align="left" valign="top">
        <div>stack item 2</div>
      </td>
      <td class="stack-cell" style="line-height: 24px; font-size: 16px; padding-right: 40px; margin: 0;" align="left" valign="top">
        <div>stack item 3</div>
      </td>
      <td class="stack-cell" style="line-height: 24px; font-size: 16px; padding-right: 40px; margin: 0;" align="left" valign="top">
        <div>stack item 4</div>
      </td>
      <td class="stack-cell" style="line-height: 24px; font-size: 16px; padding-right: 40px; margin: 0;" align="left" valign="top">
        <div>stack item 5</div>
      </td>
      <td class="stack-cell" style="line-height: 24px; font-size: 16px; padding-right: 0; margin: 0;" align="left" valign="top">
        <div>stack item 6</div>
      </td>
    </tr>
  </tbody>
</table>
```
