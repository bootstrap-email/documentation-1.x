---
layout: docs
title:  "Border Radius"
tagline: "Set the border radius on an element."
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
      {% for border in site.data.border_radiuses %}
        <tr><td class="class">.rounded{{ border.name }}</td><td class="css">border-radius: {{ border.radius }}px;</td></tr>
        <tr><td class="class">.rounded-top{{ border.name }}</td><td class="css">border-top-left-radius: {{ border.radius }}px;<br>border-top-right-radius: {{ border.radius }}px;</td></tr>
        <tr><td class="class">.rounded-right{{ border.name }}</td><td class="css">border-top-right-radius: {{ border.radius }}px;<br>border-bottom-right-radius: {{ border.radius }}px;</td></tr>
        <tr><td class="class">.rounded-bottom{{ border.name }}</td><td class="css">border-bottom-left-radius: {{ border.radius }}px;<br>border-bottom-right-radius: {{ border.radius }}px;</td></tr>
        <tr><td class="class">.rounded-left{{ border.name }}</td><td class="css">border-top-left-radius: {{ border.radius }}px;<br>border-bottom-left-radius: {{ border.radius }}px;</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

<div class="alert alert-warning">The documentation on this page is no complete yet, work in progress 👍</div>
