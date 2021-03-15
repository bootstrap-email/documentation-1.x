---
layout: docs
title:  "Container"
tagline: "Give the email center aligned structure."
sections:
  - Class Reference
  - Usage
  - Compiled Example
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
      <tr><td class="class">.container</td><td class="result">center aligned, max width 600px, left and right padding</td></tr>
      <tr><td class="class">.container-fluid</td><td class="result">full width, left and right padding</td></tr>
    </tbody>
  </table>
</div>

<a class="anchor" name="usage"></a>
<h2 class="h3">Usage</h2>

Using the `container` class is the most common default email structure recommended. It should be used to wrap your entire pages contents. It has a 600px max-width which is standard for broad email support. It will be responsive on mobile devices.

```html
<div class="container">
  <!-- Content here -->
</div>
```

A `container-fluid` is unlike a container in that it doesn't have it's max-width set. It does however still have padding on the edges to give the content better spacing towards the edge of the email.

```html
<div class="container-fluid">
  <!-- Content here -->
</div>
```

<hr class="my-5">
<a class="anchor" name="compiled-example"></a>
<h2 class="h3">Compiled Example</h2>

<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="container">
  <!-- Content here -->
</div>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="container" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%;">
  <tbody>
    <tr>
      <td align="center" style="line-height: 24px; font-size: 16px; margin: 0; padding: 0 16px;">
        <!--[if (gte mso 9)|(IE)]>
          <table align="center" role="presentation">
            <tbody>
              <tr>
                <td width="600">
        <![endif]-->
        <table align="center" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%; max-width: 600px; margin: 0 auto;">
          <tbody>
            <tr>
              <td style="line-height: 24px; font-size: 16px; margin: 0;" align="left">
                <!-- Content here -->
              </td>
            </tr>
          </tbody>
        </table>
        <!--[if (gte mso 9)|(IE)]>
                </td>
              </tr>
            </tbody>
          </table>
        <![endif]-->
      </td>
    </tr>
  </tbody>
</table>
```
