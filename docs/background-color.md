---
layout: docs
title:  "Background Color"
tagline: "Set a custom background color."
sections:
  - Class Reference
  - Usage
  - Customize
  - Compiled Example
---
<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Properties</th>
        <th></th>
      </tr>
    </thead>
    <tbody>
      {% for item in site.data.theme_colors %}
        <tr><td class="class">.bg-{{ item.name }}</td><td class="css">background-color: {{ item.color }};</td><td style="background-color: {{ item.color  }};"></td></tr>
      {% endfor %}
      {% for item in site.data.palette_colors %}
        <tr><td class="class">.bg-{{ item.name }}</td><td class="css">background-color: {{ item.color }};</td><td style="background-color: {{ item.color  }};"></td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>


{% include header.html name="Usage" hr="false" %}
Since emails render mostly consistently with tables, many of the components are built into tables. These color classes apply to the current element as well as the child `<td>` so you can use it on a component it will still work if the component is compiled into a table. It also uses the `bgcolor` property for support for old email clients. If a background color utility class is used on a `<div>` it will automatically be converted to a table with 100% width since divs don't have good background color support in many email clients.
```html
<div class="bg-primary text-white">.bg-primary</div>
<div class="bg-secondary text-white">.bg-secondary</div>
<div class="bg-success text-white">.bg-success</div>
<div class="bg-red-500 text-white">.bg-red-500</div>
<div class="bg-yellow-500 text-white">.bg-yellow-500</div>
```

<div class="bg-primary text-white">.bg-primary</div>
<div class="bg-secondary text-white">.bg-secondary</div>
<div class="bg-success text-white">.bg-success</div>
<div class="bg-danger text-white">.bg-red-500</div>
<div class="bg-warning text-white">.bg-yellow-500</div>

{% include header.html name="Customize" hr="true" %}
See the [Customize](/docs/customize) docs to learn more about customizing the color palette.

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="bg-blue-100">Blue 100</div>
<div class="bg-blue-200">Blue 200</div>
<div class="bg-blue-300">Blue 300</div>
<div class="bg-blue-400">Blue 400</div>
<div class="bg-blue-500">Blue 500</div>
<div class="bg-blue-600">Blue 600</div>
<div class="bg-blue-700">Blue 700</div>
<div class="bg-blue-800">Blue 800</div>
<div class="bg-blue-900">Blue 900</div>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="bg-blue-100 w-full" role="presentation" style="width: 100%;" bgcolor="#cfe2ff" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#cfe2ff" width="100%">
        Blue 100
      </td>
    </tr>
  </tbody>
</table>
<table class="bg-blue-200 w-full" role="presentation" style="width: 100%;" bgcolor="#9ec5fe" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#9ec5fe" width="100%">
        Blue 200
      </td>
    </tr>
  </tbody>
</table>
<table class="bg-blue-300 w-full" role="presentation" style="width: 100%;" bgcolor="#6ea8fe" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#6ea8fe" width="100%">
        Blue 300
      </td>
    </tr>
  </tbody>
</table>
<table class="bg-blue-400 w-full" role="presentation" style="width: 100%;" bgcolor="#3d8bfd" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#3d8bfd" width="100%">
        Blue 400
      </td>
    </tr>
  </tbody>
</table>
<table class="bg-blue-500 w-full" role="presentation" style="width: 100%;" bgcolor="#0d6efd" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#0d6efd" width="100%">
        Blue 500
      </td>
    </tr>
  </tbody>
</table>
<table class="bg-blue-600 w-full" role="presentation" style="width: 100%;" bgcolor="#0a58ca" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#0a58ca" width="100%">
        Blue 600
      </td>
    </tr>
  </tbody>
</table>
<table class="bg-blue-700 w-full" role="presentation" style="width: 100%;" bgcolor="#084298" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#084298" width="100%">
        Blue 700
      </td>
    </tr>
  </tbody>
</table>
<table class="bg-blue-800 w-full" role="presentation" style="width: 100%;" bgcolor="#052c65" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#052c65" width="100%">
        Blue 800
      </td>
    </tr>
  </tbody>
</table>
<table class="bg-blue-900 w-full" role="presentation" style="width: 100%;" bgcolor="#031633" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#031633" width="100%">
        Blue 900
      </td>
    </tr>
  </tbody>
</table>
```
