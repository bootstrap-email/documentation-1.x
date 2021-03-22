---
layout: docs
title:  "Border Color"
tagline: "Set the border color on an element."
sections:
  - Class Reference
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
      {% for color in site.data.theme_colors %}
        <tr><td class="class">.border-{{ color.name }}</td><td class="css">border-color: {{ color.color }};</td><td><div style="width: 40px; height: 20px; border: 2px solid {{ color.color  }};"></div></td></tr>
      {% endfor %}
      {% for color in site.data.palette_colors %}
        <tr><td class="class">.border-{{ color.name }}</td><td class="css">border-color: {{ color.color }};</td><td><div style="width: 40px; height: 20px; border: 2px solid {{ color.color  }};"></div></td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

<div class="alert alert-warning">The documentation on this page is no complete yet, work in progress 👍</div>
