---
layout: docs
title:  "Display"
tagline: "Set the display type of an element."
sections:
  - Class Reference
badges: true
themeable: false
responsive: true
---
<a class="anchor" name="class-reference"></a>
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
        <tr><td class="class">.d-{{ display }}</td><td class="css">display: {{ display }};</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

<div class="alert alert-warning">The documentation on this page is no complete yet, work in progress 👍</div>
