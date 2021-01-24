---
layout: docs
title:  "Border Radius"
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
      {% for border in site.data.border_radiuses %}
        <tr><td>.rounded{{ border.name }}</td><td>border-radius: {{ border.radius }}px;</td></tr>
        <tr><td>.rounded-top{{ border.name }}</td><td>border-top-left-radius: {{ border.radius }}px;<br>border-top-right-radius: {{ border.radius }}px;</td></tr>
        <tr><td>.rounded-right{{ border.name }}</td><td>border-top-right-radius: {{ border.radius }}px;<br>border-bottom-right-radius: {{ border.radius }}px;</td></tr>
        <tr><td>.rounded-bottom{{ border.name }}</td><td>border-bottom-left-radius: {{ border.radius }}px;<br>border-bottom-right-radius: {{ border.radius }}px;</td></tr>
        <tr><td>.rounded-left{{ border.name }}</td><td>border-top-left-radius: {{ border.radius }}px;<br>border-bottom-left-radius: {{ border.radius }}px;</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>
