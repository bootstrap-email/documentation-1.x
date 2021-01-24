---
layout: docs
title:  "Color"
badges: true
themeable: true
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
      {% for item in site.data.theme_colors %}
        <tr><td>.text-{{ item.name }}</td><td>color: {{ item.color }};</td><td style="color: {{ item.color  }};">Email</td></tr>
      {% endfor %}
      {% for item in site.data.palette_colors %}
        <tr><td>.text-{{ item.name }}</td><td>color: {{ item.color }};</td><td style="color: {{ item.color  }};">Email</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>
