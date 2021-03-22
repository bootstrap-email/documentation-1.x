---
layout: docs
title:  "Display"
tagline: "Set the display type of an element."
sections:
  - Class Reference
  - Responsive
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

{% include header.html name="Responsive" hr="false" %}
Here is an example of using the display utility to show and hide an element on mobile and hidden on desktop and vice versus.
```html
<span class="d-lg-none">Hidden on Desktop</span>
<span class="d-none d-lg-inline">Hidden on Mobile</span>
```

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<span class="d-lg-none">Hidden on Desktop</span>
<span class="d-none d-lg-inline">Hidden on Mobile</span>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<!-- The desktop styles are inlined and overridden by a media query in the <head> of the document -->
<span class="d-lg-none" style="display: none;">Hidden on Desktop</span>
<span class="d-none d-lg-inline" style="display: inline;">Hidden on Mobile</span>
```

