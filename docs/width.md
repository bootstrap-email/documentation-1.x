---
layout: docs
title:  "Width"
tagline: "Set the width or max width of an element."
sections:
  - Class Reference
  - Usage
  - Responsive
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
        <th>Properties</th>
      </tr>
    </thead>
    <tbody>
      <tr><td class="class">.w-full</td><td class="css">width: 100%;</td></tr>
      <tr><td class="class">.w-auto</td><td class="css">width: auto</td></tr>
      {% for size in site.data.sizings %}
        <tr><td class="class">.w-{{ size }}</td><td class="css">width: {{ size | times: 4 }}px;</td></tr>
      {% endfor %}
      <tr><td class="class">.max-w-full</td><td class="css">width: 100%;</td></tr>
      {% for size in site.data.sizings %}
        <tr><td class="class">.max-w-{{ size }}</td><td class="css">max-width: {{ size | times: 4 }}px;</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Like the [spacing utilities](/docs/spacing) it uses `4px` as the increment size for each number. So `w-10` is `10 * 4px` which is `40px`. To do 100% width you can use `w-full`. These width and max-width utilities are really useful for images because **images need a width and/or a height** for them to be rendered properly in many versions of Outlook.
```html
<img src="#" class="max-w-12 w-full" /> /* image 48px width */
<img src="#" class="max-w-150 w-full" /> /* image 600px width, use this for an image that is "full width" in a container in an email */
```

{% include header.html name="Responsive" hr="true" %}
By default these classes target all devices. However if you just wanted to target desktop you could do `.w-lg-4`. For all of these classes you can apply a `lg-` to the middle to make it just apply to desktop devices. Or say you want a 100% button on mobile and a auto width centered button on desktop. That would look like this:
```html
<a class="w-full w-lg-auto align-center btn btn-primary btn-lg" href="https://bootstrapemail.com">Tada</a>
```
