---
layout: docs
title:  "Sizing"
badges: true
themeable: false
responsive: true
---
There are two types of sizing utilities Bootstrap Email supports. One for width and one for height. Like the [spacing utilities](#) it uses `4px` as the increment size for each number. So `w-10` is `10 * 4px` which is `40px`. To do 100% width you can use `w-full`.

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
        <tr><td>.w-{{ size }}</td><td>width: {{ size | times: 4 }}px;</td></tr>
      {% endfor %}
      <tr><td>.w-full</td><td>width: 100%;</td></tr>
      {% for size in site.data.sizings %}
        <tr><td>.h-{{ size }}</td><td>height: {{ size | times: 4 }}px;</td></tr>
      {% endfor %}
      <tr><td>.h-full</td><td>height: 100%;</td></tr>
    </tbody>
  </table>
</div>

#### Example
These width and height utilities are really useful for images because **images need a width and/or a height** for them to be rendered properly in many versions of Outlook.
```html
<img src="#" class="w-12" /> /* image 48px width */
<img src="#" class="w-150" /> /* image 600px width, use this for an image that is "full width" in a container in an email */
```

#### Responsive
By default these classes target all devices. However if you just wanted to target desktop you could do `.w-lg-4`. For all of these classes you can apply a `lg-` to the middle to make it just apply to desktop devices. Or say you want a 100% button on mobile and a 50% width centered button on desktop. That would look like this:
```html
<a class="w-100 w-lg-25 align-center btn btn-primary btn-lg" href="https://bootstrapemail.com">Tada</a>
```
