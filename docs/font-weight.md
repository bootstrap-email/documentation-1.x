---
layout: docs
title:  "Font Weight"
tagline: "Set font weight of text."
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
      {% for weight in site.data.font_weights %}
        <tr><td class="class">.fw-{{ weight }}</td><td class="css">font-weight: {{ weight }};</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
A simple way to adjust the weight of font.
```html
<p class="fw-100">Font weight 100</p>
<p class="fw-200">Font weight 200</p>
<p class="fw-300">Font weight 300</p>
<p class="fw-400">Font weight 400</p>
<p class="fw-500">Font weight 500</p>
<p class="fw-600">Font weight 600</p>
<p class="fw-700">Font weight 700</p>
<p class="fw-800">Font weight 800</p>
<p class="fw-900">Font weight 900</p>
```
<p style="font-weight: 100;">Font weight 100</p>
<p style="font-weight: 200;">Font weight 200</p>
<p style="font-weight: 300;">Font weight 300</p>
<p style="font-weight: 400;">Font weight 400</p>
<p style="font-weight: 500;">Font weight 500</p>
<p style="font-weight: 600;">Font weight 600</p>
<p style="font-weight: 700;">Font weight 700</p>
<p style="font-weight: 800;">Font weight 800</p>
<p style="font-weight: 900;">Font weight 900</p>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<p class="fw-100">Font weight 100</p>
<p class="fw-200">Font weight 200</p>
<p class="fw-300">Font weight 300</p>
<p class="fw-400">Font weight 400</p>
<p class="fw-500">Font weight 500</p>
<p class="fw-600">Font weight 600</p>
<p class="fw-700">Font weight 700</p>
<p class="fw-800">Font weight 800</p>
<p class="fw-900">Font weight 900</p>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<p class="fw-100" style="line-height: 24px; font-size: 16px; font-weight: 100 !important; width: 100%; margin: 0;" align="left">Some text here with some amount of weight</p>
<p class="fw-200" style="line-height: 24px; font-size: 16px; font-weight: 200 !important; width: 100%; margin: 0;" align="left">Some text here with some amount of weight</p>
<p class="fw-300" style="line-height: 24px; font-size: 16px; font-weight: 300 !important; width: 100%; margin: 0;" align="left">Some text here with some amount of weight</p>
<p class="fw-400" style="line-height: 24px; font-size: 16px; font-weight: 400 !important; width: 100%; margin: 0;" align="left">Some text here with some amount of weight</p>
<p class="fw-500" style="line-height: 24px; font-size: 16px; font-weight: 500 !important; width: 100%; margin: 0;" align="left">Some text here with some amount of weight</p>
<p class="fw-600" style="line-height: 24px; font-size: 16px; font-weight: 600 !important; width: 100%; margin: 0;" align="left">Some text here with some amount of weight</p>
<p class="fw-700" style="line-height: 24px; font-size: 16px; font-weight: 700 !important; width: 100%; margin: 0;" align="left">Some text here with some amount of weight</p>
<p class="fw-800" style="line-height: 24px; font-size: 16px; font-weight: 800 !important; width: 100%; margin: 0;" align="left">Some text here with some amount of weight</p>
<p class="fw-900" style="line-height: 24px; font-size: 16px; font-weight: 900 !important; width: 100%; margin: 0;" align="left">Some text here with some amount of weight</p>
```
