---
layout: docs
title:  "Line Height"
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
      {% for size in site.data.line_heights %}
        <tr><td>.text-{{ size.name }}</td><td>line-height: {{ size.size }};</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>
