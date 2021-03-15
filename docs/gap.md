---
layout: docs
title:  "Gap"
badges: true
themeable: false
responsive: true
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
      {% for size in site.data.sizings %}
        <tr><td>.g-{{ size }}</td><td>{{ size | times: 4 }}px gutters on all sides</td></tr>
        <tr><td>.gx-{{ size }}</td><td>{{ size | times: 4 }}px gutters on left and right sides</td></tr>
        <tr><td>.gy-{{ size }}</td><td>{{ size | times: 4 }}px gutters on top and bottom sides</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

By default the grid `.row` class has 30px horizontal gutters. You can apply these gutter classes to the row class to change horizontal and vertical gutters `row g-4` will add 16px gutters on all sizes. Top and bottom gutters are useful for when a grid is responsive and stacks columns vertically on mobile.
