---
layout: docs
title:  "Block"
tagline: "A simple way to generate a table element."
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
      <tr><td class="class">&lt;block&gt;, .to-table</td><td class="result">turn the current element into a table and move the classes onto the table.</td></tr>
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Since many email clients have poor support for block elements such as `div`s, `table`s are usually used in their place. Much of Bootstrap Email automatically builds things into tables automatically and applies the correct styles. However there are certain time when that is not the case and you want to easy make something into a table without having to write out the full table structure.

This is where `block` or `.to-table` come in. `block` is an HTML element and `to-table` is a class but both have the same result of turning the current element into a table.
```html
<!-- these two examples are equivalent -->
<div class="to-table w-full border-3 border-red-300">Hello</div>
<block class="w-full border-3 border-red-300">Hello</block>
```

Tip: Use the `w-full` class to make a table `width: 100%` to make it work like a div or block element.

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="to-table w-full border-3 border-red-300">Hello</div>
<block class="w-full border-3 border-red-300">Hello</block>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="to-table w-full border-3 border-red-300" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%; border: 3px solid #ea868f;" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" width="100%">
        Hello
      </td>
    </tr>
  </tbody>
</table>
<table class="w-full border-3 border-red-300 to-table" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%; border: 3px solid #ea868f;" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" width="100%">
        Hello
      </td>
    </tr>
  </tbody>
</table>
```
