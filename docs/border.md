---
layout: docs
title:  "Border"
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
      {% for border in site.data.border_widths %}
        <tr><td>.border{{ border.name }}</td><td>border: {{ border.width }}px solid #dee2e6;</td></tr>
        <tr><td>.border-top{{ border.name }}</td><td>border-top: {{ border.width }}px solid #dee2e6;</td></tr>
        <tr><td>.border-right{{ border.name }}</td><td>border-right: {{ border.width }}px solid #dee2e6;</td></tr>
        <tr><td>.border-bottom{{ border.name }}</td><td>border-bottom: {{ border.width }}px solid #dee2e6;</td></tr>
        <tr><td>.border-left{{ border.name }}</td><td>border-left: {{ border.width }}px solid #dee2e6;</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>
