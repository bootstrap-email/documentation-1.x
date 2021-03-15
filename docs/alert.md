---
layout: docs
title:  "Alert"
tagline: "Bring attention or notice to a message."
sections:
  - Class Reference
  - Usage
  - Compiled Example
badges: true
themeable: true
responsive: false
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
      <tr><td class="class">.alert</td><td class="result">the base alert class to setup structure</td></tr>
      {% for item in site.data.theme_colors %}
        <tr><td class="class">.alert-{{ item.name }}</td><td class="result">{{ item.name }} theme color</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
```html
<div class="alert alert-primary">
  This is a primary alert—check it out!
</div>
<div class="alert alert-secondary">
  This is a secondary alert—check it out!
</div>
<div class="alert alert-success">
  This is a success alert—check it out!
</div>
<div class="alert alert-danger">
  This is a danger alert—check it out!
</div>
<div class="alert alert-warning">
  This is a warning alert—check it out!
</div>
<div class="alert alert-info">
  This is a info alert—check it out!
</div>
<div class="alert alert-light">
  This is a light alert—check it out!
</div>
<div class="alert alert-dark">
  This is a dark alert—check it out!
</div>
```

<div class="alert alert-primary">
  This is a primary alert—check it out!
</div>
<div class="alert alert-secondary">
  This is a secondary alert—check it out!
</div>
<div class="alert alert-success">
  This is a success alert—check it out!
</div>
<div class="alert alert-danger">
  This is a danger alert—check it out!
</div>
<div class="alert alert-warning">
  This is a warning alert—check it out!
</div>
<div class="alert alert-info">
  This is a info alert—check it out!
</div>
<div class="alert alert-light">
  This is a light alert—check it out!
</div>
<div class="alert alert-dark">
  This is a dark alert—check it out!
</div>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="alert alert-primary"><strong>Well done!</strong> You successfully read this important alert message.</div>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="alert alert-primary" role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-collapse: separate !important; width: 100%; border: 0;">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; border-radius: 4px; color: #012e70; margin: 0; padding: 12px 20px; border: 1px solid transparent;" align="left" bgcolor="#d7e7ff">
        <div>
          <strong>Well done!</strong> You successfully read this important alert message.
        </div>
      </td>
    </tr>
  </tbody>
</table>
```
