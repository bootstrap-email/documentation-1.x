---
layout: docs
title:  "Badge"
tagline: "An inline way to show a status or count."
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
      <tr><td class="class">.badge</td><td class="result">the base badge class to setup structure</td></tr>
      {% for item in site.data.theme_colors %}
        <tr><td class="class">.badge-{{ item.name }}</td><td class="result">{{ item.name }} theme color</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>


{% include header.html name="Usage" hr="false" %}
Use the [Background Color](/docs/background-color), [Text Color](/docs/text-color), and [Border Radius](/docs/border-radius) classes to style badges.

```html
<span class="badge bg-primary">Primary</span>
<span class="badge bg-secondary">Secondary</span>
<span class="badge bg-success">Success</span>
<span class="badge bg-danger">Danger</span>
<span class="badge bg-warning text-dark">Warning</span>
<span class="badge bg-info text-dark">Info</span>
<span class="badge bg-light text-dark rounded-full">Light</span>
<span class="badge bg-dark rounded-full">Dark</span>
```

<span class="badge bg-primary">Primary</span>
<span class="badge bg-secondary">Secondary</span>
<span class="badge bg-success">Success</span>
<span class="badge bg-danger">Danger</span>
<span class="badge bg-warning text-dark">Warning</span>
<span class="badge bg-info text-dark">Info</span>
<span class="badge bg-light text-dark rounded-pill">Light</span>
<span class="badge bg-dark rounded-pill">Dark</span>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<span class="badge badge-primary">Badge</span>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="badge badge-primary" align="left" role="presentation" border="0" cellpadding="0" cellspacing="0">
  <tbody>
    <tr>
      <td style="line-height: 1; font-size: 75%; display: inline-block; font-weight: 700; white-space: nowrap; border-radius: 4px; margin: 0; padding: 4px 6.4px;" align="center" valign="baseline">
        <span>Badge</span>
      </td>
    </tr>
  </tbody>
</table>
```
