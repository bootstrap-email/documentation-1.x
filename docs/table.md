---
layout: docs
title:  "Table"
tagline: "Layout data in a tabular view."
sections:
  - Class Reference
  - Usage
  - Compiled Example
badges: true
themeable: false
responsive: false
---
<a class="anchor" name="reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">.table</td><td class="result">applies the basic styles for a table, required for use with classes below</td></tr>
      <tr><td class="class">.table-bordered</td><td class="result">table with border on all size</td></tr>
      <tr><td class="class">.table-striped</td><td class="result">table with every other row striped</td></tr>
      <tr><td class="class">.thead-light</td><td class="result">light table header</td></tr>
      <tr><td class="class">.thead-dark</td><td class="result">dark table header</td></tr>
      {% for item in site.data.theme_colors %}
        <tr><td class="class">.table-{{ item.name }}</td><td class="css">background-color: {{ item.color }};</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
```html
<table class="table table-striped thead-default table-bordered">
  <thead>
    <tr>
      <th>Col 1</th>
      <th>Col 2</th>
      <th>Col 3</th>
      <th>Col 4</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
    <tr>
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
    <tr class="table-success">
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
    <tr>
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
  </tbody>
</table>
```

<table class="table table-striped thead-default table-bordered">
  <thead>
    <tr>
      <th>Col 1</th>
      <th>Col 2</th>
      <th>Col 3</th>
      <th>Col 4</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
    <tr>
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
    <tr class="table-success">
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
    <tr>
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
  </tbody>
</table>

{% include header.html name="Compiled Example" hr="true" %}

<span class="badge rounded-pill badge-input">Input</span>
```html
<table class="table table-striped thead-default table-bordered">
  <thead>
    <tr>
      <th>Col 1</th>
      <th>Col 2</th>
      <th>Col 3</th>
      <th>Col 4</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
    <tr>
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
    <tr class="table-success">
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
    <tr>
      <td>Col Data 1</td>
      <td>Col Data 2</td>
      <td>Col Data 3</td>
      <td>Col Data 4</td>
    </tr>
  </tbody>
</table>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="table table-striped thead-default table-bordered" border="0" cellpadding="0" cellspacing="0" style="width: 100%; max-width: 100%; border: 1px solid #e2e8f0;">
  <thead>
    <tr>
      <th style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border-color: #e2e8f0; border-style: solid; border-width: 1px 1px 2px;" align="left" valign="top">Col 1</th>
      <th style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border-color: #e2e8f0; border-style: solid; border-width: 1px 1px 2px;" align="left" valign="top">Col 2</th>
      <th style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border-color: #e2e8f0; border-style: solid; border-width: 1px 1px 2px;" align="left" valign="top">Col 3</th>
      <th style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border-color: #e2e8f0; border-style: solid; border-width: 1px 1px 2px;" align="left" valign="top">Col 4</th>
    </tr>
  </thead>
  <tbody>
    <tr style="" bgcolor="#f2f2f2">
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 1</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 2</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 3</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 4</td>
    </tr>
    <tr>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 1</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 2</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 3</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 4</td>
    </tr>
    <tr class="table-success" style="" bgcolor="#f2f2f2">
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" bgcolor="#84e8ba" valign="top">Col Data 1</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" bgcolor="#84e8ba" valign="top">Col Data 2</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" bgcolor="#84e8ba" valign="top">Col Data 3</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" bgcolor="#84e8ba" valign="top">Col Data 4</td>
    </tr>
    <tr>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 1</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 2</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 3</td>
      <td style="line-height: 24px; font-size: 16px; margin: 0; padding: 12px; border: 1px solid #e2e8f0;" align="left" valign="top">Col Data 4</td>
    </tr>
  </tbody>
</table>
```
