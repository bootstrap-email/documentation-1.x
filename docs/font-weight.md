---
layout: docs
title:  "Text Weight"
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
      {% for weight in site.data.font_weights %}
        <tr><td>.fw-{{ weight }}</td><td>font-weight: {{ weight }};</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>
