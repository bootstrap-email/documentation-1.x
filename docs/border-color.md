---
layout: docs
title:  "Border Color"
badges: true
themeable: false
responsive: false
---
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
        <tr><td>.border-{{ color.name }}</td><td>border-color: {{ color.color }};</td><td><div style="width: 40px; height: 20px; border: 2px solid {{ color.color  }};"></div></td></tr>
      {% endfor %}
      {% for color in site.data.palette_colors %}
        <tr><td>.border-{{ color.name }}</td><td>border-color: {{ color.color }};</td><td><div style="width: 40px; height: 20px; border: 2px solid {{ color.color  }};"></div></td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>
