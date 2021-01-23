---
layout: docs
title:  "Text Size"
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
      </tr>
    </thead>
    <tbody>
      {% for size in site.data.font_sizes %}
        <tr><td>.text-{{ size.name }}</td><td>font-size: {{ size.size }}px;</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>
