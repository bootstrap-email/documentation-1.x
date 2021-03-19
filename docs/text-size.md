---
layout: docs
title:  "Text Size"
tagline: "Utility classes to adjust text size."
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
      {% for size in site.data.font_sizes %}
        <tr><td class="class">.text-{{ size.name }}</td><td class="css">font-size: {{ size.size }}px;</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
These utility classes are good for more fine tuned adjustments of font size.
```html
<p class="text-xs">Text size xs</p>
<p class="text-sm">Text size sm</p>
<p class="text-base">Text size base</p>
<p class="text-lg">Text size lg</p>
<p class="text-xl">Text size xl</p>
<p class="text-2xl">Text size 2xl</p>
<p class="text-3xl">Text size 3xl</p>
<p class="text-4xl">Text size 4xl</p>
<p class="text-5xl">Text size 5xl</p>
<p class="text-6xl">Text size 6xl</p>
<p class="text-7xl">Text size 7xl</p>
```
{% for size in site.data.font_sizes %}
  <p style="font-size: {{ size.size }};">Text size {{ size.name }}</p>
{% endfor %}

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<span class="text-xs">Text size xs</span>
<span class="text-sm">Text size sm</span>
<span class="text-base">Text size base</span>
<span class="text-lg">Text size lg</span>
<span class="text-xl">Text size xl</span>
<span class="text-2xl">Text size 2xl</span>
<span class="text-3xl">Text size 3xl</span>
<span class="text-4xl">Text size 4xl</span>
<span class="text-5xl">Text size 5xl</span>
<span class="text-6xl">Text size 6xl</span>
<span class="text-7xl">Text size 7xl</span>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<span class="text-xs" style="font-size: 12px; line-height: 14.4px;">Text size xs</span>
<span class="text-sm" style="font-size: 14px; line-height: 16.8px;">Text size sm</span>
<span class="text-base" style="font-size: 16px; line-height: 19.2px;">Text size base</span>
<span class="text-lg" style="font-size: 18px; line-height: 21.6px;">Text size lg</span>
<span class="text-xl" style="font-size: 20px; line-height: 24px;">Text size xl</span>
<span class="text-2xl" style="font-size: 24px; line-height: 28.8px;">Text size 2xl</span>
<span class="text-3xl" style="font-size: 30px; line-height: 36px;">Text size 3xl</span>
<span class="text-4xl" style="font-size: 36px; line-height: 43.2px;">Text size 4xl</span>
<span class="text-5xl" style="font-size: 48px; line-height: 57.6px;">Text size 5xl</span>
<span class="text-6xl" style="font-size: 64px; line-height: 76.8px;">Text size 6xl</span>
<span class="text-7xl" style="font-size: 80px; line-height: 96px;">Text size 7xl</span>
```
