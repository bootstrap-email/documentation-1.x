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

#### Example

There are two visibility classes you can apply to elements to show or hide it on a mobile vs desktop device. These are different than how this works in Bootstrap.

`.d-desktop` will show an element on desktop and hide it on mobile.

`.d-mobile` will show an element on mobile and hide it on desktop.
