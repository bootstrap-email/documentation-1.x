---
layout: docs
title:  "Text Color"
tagline: "Give text any color you want."
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
        <th>Properties</th>
        <th></th>
      </tr>
    </thead>
    <tbody>
      {% for item in site.data.theme_colors %}
        <tr><td class="class">.text-{{ item.name }}</td><td class="css">color: {{ item.color }};</td><td style="color: {{ item.color  }};">Email</td></tr>
      {% endfor %}
      {% for item in site.data.palette_colors %}
        <tr><td class="class">.text-{{ item.name }}</td><td class="css">color: {{ item.color }};</td><td style="color: {{ item.color  }};">Email</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
A simple way to adjust the line height of text.
```html
<span class="text-primary">Primary Text color</span>
<span class="text-muted">Muted Text color</span>
<span class="text-danger">Danger Text color</span>
<span class="text-green-500">Green 500 Text color</span>
<span class="text-yellow-500">Yellow 500 Text color</span>
```

<span class="text-primary">Primary Text color</span>
<span class="text-muted">Muted Text color</span>
<span class="text-danger">Danger Text color</span>
<span class="text-success">Green 500 Text color</span>
<span class="text-warning">Yellow 500 Text color</span>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<span class="text-primary">Primary Text color</span>
<span class="text-muted">Muted Text color</span>
<span class="text-danger">Danger Text color</span>
<span class="text-green-500">Green 500 Text color</span>
<span class="text-yellow-500">Yellow 500 Text color</span>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<span class="text-primary" style="color: #0d6efd;">Primary Text color</span>
<span class="text-muted" style="color: #718096;">Muted Text color</span>
<span class="text-danger" style="color: #dc3545;">Danger Text color</span>
<span class="text-green-500" style="color: #198754;">Green 500 Text color</span>
<span class="text-yellow-500" style="color: #ffc107;">Yellow 500 Text color</span>
```
