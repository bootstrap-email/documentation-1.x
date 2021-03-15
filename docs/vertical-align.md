---
layout: docs
title:  "Vertical Align"
tagline: "Vertically align the contents of a table cell."
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
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">.valign-top</td><td class="css">vertical-align: top;</td></tr>
      <tr><td class="class">.valign-middle</td><td class="css">vertical-align: middle;</td></tr>
      <tr><td class="class">.valign-bottom</td><td class="css">vertical-align: bottom;</td></tr>
      <tr><td class="class">.valign-baseline</td><td class="css">vertical-align: baseline;</td></tr>
      <tr><td class="class">.valign-text-top</td><td class="css">vertical-align: text-top;</td></tr>
      <tr><td class="class">.valign-text-bottom</td><td class="css">vertical-align: text-bottom;</td></tr>
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Vertical align allows you to vertically align the contents of a table cell. It can only be use in conjunction with a table cell. However most parts of Bootstrap Email are converted into tables so it can feel pretty automatic. You can also apply them directly to the parent `table` to adjust all of the `td` vertical alignments. If you are looking to vertically align child elements of a Stack, check out the [alignment section](/docs/stack#alignment) of the Stack docs.
```html
<table class="h-24">
  <tbody>
    <tr>
      <td class="valign-baseline">baseline</td>
      <td class="valign-top">top</td>
      <td class="valign-middle">middle</td>
      <td class="valign-bottom">bottom</td>
      <td class="valign-text-top">text-top</td>
      <td class="valign-text-bottom">text-bottom</td>
    </tr>
  </tbody>
</table>
```

<table style="height: 96px;">
  <tbody>
    <tr>
      <td class="align-baseline">baseline</td>
      <td class="align-top">top</td>
      <td class="align-middle">middle</td>
      <td class="align-bottom">bottom</td>
      <td class="align-text-top">text-top</td>
      <td class="align-text-bottom">text-bottom</td>
    </tr>
  </tbody>
</table>


{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<table class="h-24">
  <tbody>
    <tr>
      <td class="valign-baseline">baseline</td>
      <td class="valign-top">top</td>
      <td class="valign-middle">middle</td>
      <td class="valign-bottom">bottom</td>
      <td class="valign-text-top">text-top</td>
      <td class="valign-text-bottom">text-bottom</td>
    </tr>
  </tbody>
</table>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="h-24" border="0" cellpadding="0" cellspacing="0" style="height: 96px;" height="96">
  <tbody>
    <tr>
      <td class="valign-baseline" style="line-height: 24px; font-size: 16px; height: 96px; margin: 0;" align="left" valign="baseline" height="96">baseline</td>
      <td class="valign-top" style="line-height: 24px; font-size: 16px; height: 96px; margin: 0;" align="left" valign="top" height="96">top</td>
      <td class="valign-middle" style="line-height: 24px; font-size: 16px; height: 96px; margin: 0;" align="left" valign="middle" height="96">middle</td>
      <td class="valign-bottom" style="line-height: 24px; font-size: 16px; height: 96px; margin: 0;" align="left" valign="bottom" height="96">bottom</td>
      <td class="valign-text-top" style="line-height: 24px; font-size: 16px; height: 96px; margin: 0;" align="left" valign="text-top" height="96">text-top</td>
      <td class="valign-text-bottom" style="line-height: 24px; font-size: 16px; height: 96px; margin: 0;" align="left" valign="text-bottom" height="96">text-bottom</td>
    </tr>
  </tbody>
</table>
```

