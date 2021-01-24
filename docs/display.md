---
layout: docs
title:  "Display"
badges: true
themeable: false
responsive: true
---

<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Result</th>
      </tr>
    </thead>
    <tbody>
      {% for display in site.data.displays %}
        <tr><td>.d-{{ display }}</td><td>display: {{ display }};</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>
