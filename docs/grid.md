---
layout: docs
title:  "Grid"
tagline: "A responsive 12 column grid system."
sections:
  - Class Reference
  - Usage
  - Responsive
  - Gap
  - Compiled Example
badges: true
themeable: false
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
      <tr><td class="class">.row</td><td class="result">parent element to build a grid</td></tr>
      {% for item in site.data.grid_cols %}
        <tr><td class="class">.col-{{ item.name }}</td><td class="css">width: {{ item.width }};</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Grids work just like they do in Bootstrap, based on a 12 column grid. Make a row and give it columns. By default the grid holds it's structure on every device. It has a default horizontal gutter between elements of `24px`.

```html
<div class="row">
  <div class="col-3">.col-3</div>
  <div class="col-4">.col-4</div>
  <div class="col-5">.col-5</div>
</div>
```

<div class="row mb-4">
  <div class="col-3"><div class="border">.col-3</div></div>
  <div class="col-4"><div class="border">.col-4</div></div>
  <div class="col-5"><div class="border">.col-5</div></div>
</div>

{% include header.html name="Responsive" hr="true" %}
You can use the responsive <code>lg</code> modifier to make the grid snap back to vertical stacking on smaller devices.

```html
<div class="row">
  <div class="col-lg-3">.col-3</div>
  <div class="col-lg-4">.col-4</div>
  <div class="col-lg-5">.col-5</div>
</div>
```

{% include header.html name="Gap" hr="true" %}
To customize horizontal and vertical gutters see the [Gap Docs](/docs/gap) for more details. For example `row gap-0` would remove the gap between cells. In the example below, the `gap-12` adds a `48px` gap between all cells. The default gap between cells is `24px`.

```html
<div class="row gap-12">
  <div class="col-3">.col-3</div>
  <div class="col-4">.col-4</div>
  <div class="col-5">.col-5</div>
</div>
```

<div class="row g-5">
  <div class="col-lg-3"><div class="border">.col-3</div></div>
  <div class="col-lg-4"><div class="border">.col-4</div></div>
  <div class="col-lg-5"><div class="border">.col-5</div></div>
</div>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="row">
  <div class="col-3">This is a 1/4 of the row</div>
  <div class="col-3">This is a 1/4 of the row</div>
  <div class="col-6">This is a 1/2 of the row</div>
</div>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="row" role="presentation" border="0" cellpadding="0" cellspacing="0" style="table-layout: fixed; width: 100%;" width="100%">
  <tbody>
    <tr>
      <td class="col-3" style="line-height: 24px; font-size: 16px; min-height: 1px; font-weight: normal; padding-right: 30px; width: 25%; margin: 0;" align="left" valign="top">
        This is a 1/4 of the row
      </td>
      <td class="col-3" style="line-height: 24px; font-size: 16px; min-height: 1px; font-weight: normal; padding-right: 30px; width: 25%; margin: 0;" align="left" valign="top">
        This is a 1/4 of the row
      </td>
      <td class="col-6" style="line-height: 24px; font-size: 16px; min-height: 1px; font-weight: normal; padding-right: 30px; width: 50%; margin: 0;" align="left" valign="top">
        This is a 1/2 of the row
      </td>
    </tr>
  </tbody>
</table>
```
