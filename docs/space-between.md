---
layout: docs
title:  "Space Between"
tagline: "Evenly space child elements vertically."
sections:
  - Class Reference
  - Usage
  - Compiled Example
responsive: true
---
<a class="anchor" name="class-reference"></a>
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Properties</th>
      </tr>
    </thead>
    <tbody>
      {% for spacing in site.data.spacings %}
        <tr><td class="class">.space-y-{{ spacing }}</td><td class="result">Make a {{ spacing | times: 4 }}px spacer between every child element</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Similar to space between in [Tailwind](https://tailwindcss.com/docs/space), this allows you to space elements evenly vertically. Good for things like paragraphs of text. If you want horizontal spacing between elements or more complex alignment, check out the [Stack](/docs/stack) documentation.
```html
<div class="space-y-3">
  <a class="btn btn-primary" href="http://example.com">Space between these buttons</a>
  <a class="btn btn-primary" href="http://example.com">Space between these buttons</a>
  <a class="btn btn-primary" href="http://example.com">Space between these buttons</a>
</div>

```
<div>
  <a class="btn btn-primary" href="http://example.com">Space between these buttons</a>
</div>
<div class="my-3">
  <a class="btn btn-primary" href="http://example.com">Space between these buttons</a>
</div>
<div>
  <a class="btn btn-primary" href="http://example.com">Space between these buttons</a>
</div>


{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="space-y-3">
  <a class="btn btn-primary" href="http://example.com">Space between these buttons</a>
  <a class="btn btn-primary" href="http://example.com">Space between these buttons</a>
  <a class="btn btn-primary" href="http://example.com">Space between these buttons</a>
</div>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<div class="space-y-3">
  <table class="btn btn-primary" role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-radius: 6px; border-collapse: separate !important;">
    <tbody>
      <tr>
        <td style="line-height: 24px; font-size: 16px; border-radius: 6px; margin: 0;" align="center" bgcolor="#0d6efd">
          <a href="http://example.com" style="color: #ffffff; font-size: 16px; font-family: Helvetica, Arial, sans-serif; text-decoration: none; border-radius: 6px; line-height: 20px; display: inline-block; font-weight: normal; white-space: nowrap; background-color: #0d6efd; padding: 8px 12px; border: 1px solid #0d6efd;">Space between these buttons</a>
        </td>
      </tr>
    </tbody>
  </table>
  <table class="s-3 w-full" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%;" width="100%">
    <tbody>
      <tr>
        <td style="line-height: 12px; font-size: 12px; width: 100%; height: 12px; margin: 0;" align="left" width="100%" height="12">
           
        </td>
      </tr>
    </tbody>
  </table>
    <table class="btn btn-primary" role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-radius: 6px; border-collapse: separate !important;">
    <tbody>
      <tr>
        <td style="line-height: 24px; font-size: 16px; border-radius: 6px; margin: 0;" align="center" bgcolor="#0d6efd">
          <a href="http://example.com" style="color: #ffffff; font-size: 16px; font-family: Helvetica, Arial, sans-serif; text-decoration: none; border-radius: 6px; line-height: 20px; display: inline-block; font-weight: normal; white-space: nowrap; background-color: #0d6efd; padding: 8px 12px; border: 1px solid #0d6efd;">Space between these buttons</a>
        </td>
      </tr>
    </tbody>
  </table>
  <table class="s-3 w-full" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%;" width="100%">
    <tbody>
      <tr>
        <td style="line-height: 12px; font-size: 12px; width: 100%; height: 12px; margin: 0;" align="left" width="100%" height="12">
           
        </td>
      </tr>
    </tbody>
  </table>
  <table class="btn btn-primary" role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-radius: 6px; border-collapse: separate !important;">
    <tbody>
      <tr>
        <td style="line-height: 24px; font-size: 16px; border-radius: 6px; margin: 0;" align="center" bgcolor="#0d6efd">
          <a href="http://example.com" style="color: #ffffff; font-size: 16px; font-family: Helvetica, Arial, sans-serif; text-decoration: none; border-radius: 6px; line-height: 20px; display: inline-block; font-weight: normal; white-space: nowrap; background-color: #0d6efd; padding: 8px 12px; border: 1px solid #0d6efd;">Space between these buttons</a>
        </td>
      </tr>
    </tbody>
  </table>
</div>
```
