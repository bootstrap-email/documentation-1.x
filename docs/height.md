---
layout: docs
title:  "Height"
tagline: "Set the height or max height of an element."
sections:
  - Class Reference
  - Usage
  - Responsive
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
      <tr><td class="class">.h-full</td><td class="css">height: 100%;</td></tr>
      <tr><td class="class">.h-auto</td><td class="css">height: auto</td></tr>
      {% for size in site.data.sizings %}
        <tr><td class="class">.h-{{ size }}</td><td class="css">height: {{ size | times: 4 }}px;</td></tr>
      {% endfor %}
      <tr><td class="class">.max-h-full</td><td class="css">max-height: 100%;</td></tr>
      {% for size in site.data.sizings %}
        <tr><td class="class">.max-h-{{ size }}</td><td class="css">max-height: {{ size | times: 4 }}px;</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Like the [padding utilities](/docs/padding) it uses `4px` as the increment size for each number. So `h-10` is `10 * 4px` which is `40px`. To do 100% height you can use `h-full`. These height and max-height utilities are really useful for images because **images need a width and/or a height** for them to be rendered properly in many versions of Outlook.
```html
<img src="#" class="max-h-12 h-full" /> /* image 48px width */
<img src="#" class="max-h-150 h-full" /> /* image 600px width, use this for an image that is "full width" in a container in an email */
```

In combination with the [width](/docs/width) utilities you can do things like make a circle with number in it.
```html
<div class="h-10 w-10 rounded-full bg-blue-500 text-white text-center valign-middle">1</div>
```
<div class="rounded-pill bg-primary text-white d-flex justify-content-center align-items-center" style="width: 40px; height: 40px;"><span>1</span></div>


{% include header.html name="Responsive" hr="true" %}
By default these classes target all devices. However if you just wanted to target desktop you could do `.h-lg-4`. For all of these classes you can apply a `lg-` to the middle to make it just apply to desktop devices. Or say you want a 100% button on mobile and a 40px height centered button on desktop. That would look like this:
```html
<a class="h-full h-lg-10 align-center btn btn-primary btn-lg" href="https://bootstrapemail.com">Tada</a>
```

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="h-10 w-10 rounded-full bg-blue-500 text-white text-center valign-middle">1</div>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="h-10 w-10 rounded-full bg-blue-500 text-white text-center valign-middle w-full" role="presentation" style="border-radius: 9999px; color: #ffffff; width: 40px; height: 40px; text-align: center !important; vertical-align: middle !important;" bgcolor="#0d6efd" width="40" height="40">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; border-radius: 9999px; color: #ffffff; width: 40px; height: 40px; margin: 0;" align="center" bgcolor="#0d6efd" valign="middle" width="40" height="40">
        1
      </td>
    </tr>
  </tbody>
</table>
```
