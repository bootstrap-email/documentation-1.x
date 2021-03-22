---
layout: docs
title:  "Border"
tagline: "Set the border width on an element."
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
      {% for border in site.data.border_widths %}
        <tr><td class="class">.border{{ border.name }}</td><td class="css">border: {{ border.width }}px solid #dee2e6;</td></tr>
        <tr><td class="class">.border-top{{ border.name }}</td><td class="css">border-top: {{ border.width }}px solid #dee2e6;</td></tr>
        <tr><td class="class">.border-right{{ border.name }}</td><td class="css">border-right: {{ border.width }}px solid #dee2e6;</td></tr>
        <tr><td class="class">.border-bottom{{ border.name }}</td><td class="css">border-bottom: {{ border.width }}px solid #dee2e6;</td></tr>
        <tr><td class="class">.border-left{{ border.name }}</td><td class="css">border-left: {{ border.width }}px solid #dee2e6;</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

<div class="alert alert-warning">The documentation on this page is no complete yet, work in progress 👍</div>
