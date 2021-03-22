---
layout: docs
title:  "Line Height"
tagline: "Set line height of text."
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
      </tr>
    </thead>
    <tbody>
      {% for size in site.data.line_heights %}
        <tr><td class="class">.lh-{{ size.name }}</td><td class="css">line-height: {{ size.size }};</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
A simple way to adjust the line height of text.
```html
<p class="lh-1">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-sm">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-base">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-lg">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
```

<p class="lh-1">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-sm">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-base">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-lg">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<p class="lh-1">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-sm">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-base">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-lg">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<p class="lh-1" style="line-height: 1; font-size: 16px; width: 100%; margin: 0;" align="left">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-sm" style="line-height: 1.25; font-size: 16px; width: 100%; margin: 0;" align="left">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-base" style="line-height: 1.5; font-size: 16px; width: 100%; margin: 0;" align="left">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
<p class="lh-lg" style="line-height: 2; font-size: 16px; width: 100%; margin: 0;" align="left">This is test of text with different amounts of line height. What do you think of the line height for this text? Is it too large? Too small? The world may never know but I do hope that this works.</p>
```
