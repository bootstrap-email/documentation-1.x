---
layout: docs
title:  "Spacing"
badges: true
themeable: false
responsive: true
---
There are three types of spacing Bootstrap Email supports. Padding (applied to the inside of table cells) and Margin (in the form of vertical spacers) and Spacers which are used to take up space between elements vertically.
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
        <tr><td>.p-{{ spacing }}</td><td>padding: {{ spacing | times: 4 }}px;</td></tr>
        <tr><td>.px-{{ spacing }}</td><td>padding-left: {{ spacing | times: 4 }}px; padding-right: {{ spacing | times: 4 }}px;</td></tr>
        <tr><td>.py-{{ spacing }}</td><td>padding-top: {{ spacing | times: 4 }}px; padding-bottom: {{ spacing | times: 4 }}px;</td></tr>
        <tr><td>.pt-{{ spacing }}</td><td>padding-top: {{ spacing | times: 4 }}px;</td></tr>
        <tr><td>.pr-{{ spacing }}</td><td>padding-right: {{ spacing | times: 4 }}px;</td></tr>
        <tr><td>.pb-{{ spacing }}</td><td>padding-bottom: {{ spacing | times: 4 }}px;</td></tr>
        <tr><td>.pl-{{ spacing }}</td><td>padding-left: {{ spacing | times: 4 }}px;</td></tr>
      {% endfor %}
      {% for spacing in site.data.spacings %}
        <tr><td>.my-{{ spacing }}</td><td>Make a {{ spacing | times: 4 }}px spacer above and below</td></tr>
        <tr><td>.mt-{{ spacing }}</td><td>Make a {{ spacing | times: 4 }}px spacer above</td></tr>
        <tr><td>.mb-{{ spacing }}</td><td>Make a {{ spacing | times: 4 }}px spacer below</td></tr>
      {% endfor %}
      {% for spacing in site.data.spacings %}
        <tr><td>.s-{{ spacing }}</td><td>Make a spacer {{ spacing | times: 4 }}px tall</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

List of supported classes:
```css
.p-{0-5}  /* padding on all sides */
.pt-{0-5} /* padding top */
.pr-{0-5} /* padding right */
.pb-{0-5} /* padding bottom */
.pl-{0-5} /* padding left */
.px-{0-5} /* padding left and right */
.py-{0-5} /* padding top and bottom */

.mt-{0-5} /* margin top */
.mb-{0-5} /* margin bottom */
.my-{0-5} /* margin top and bottom */

.s-{0-5} /* spacer with size */
```

Note: Margin is only supported on the top and bottom.

#### Responsive
By default these classes target all devices. However you you just wanted to target desktop you could do `.w-lg-25`. For all of these classes you can apply a `lg-` to the middle to make it just apply to desktop devices. Or say you want a 100% button on mobile and a 50% width centered button on desktop. That would look like this:
```html
<a class="w-100 w-lg-25 mx-auto btn btn-primary btn-lg" href="https://bootstrapemail.com">Tada</a>
```

That is the power of Bootstrap email right there!
<div class="alert alert-info">
  <strong>Neato!</strong> All of the above classes are responsive so putting `mt-1 mt-lg-3` on a element with have a spacing of 1 on mobile and a spacing of 3 on desktop.
</div>

#### Padding
```html
<a class="btn btn-primary p-3" href="http://bootstrapemail.com">A Button with lots of padding</a>
```

<a class="btn btn-primary p-3" href="http://bootstrapemail.com">A Button with lots of padding</a>

#### Margin
The margin classes just create spacers above and/or below and element for simpler syntax like Bootstrap.
```html
<div class="card card-body">Top Card</div>
<div class="card card-body my-3">Middle Card (with margin above and below)</div>
<div class="card card-body">Bottom Card</div>
```

<div class="card card-body">Top Card</div>
<div class="card card-body my-3">Middle Card (with margin about and below)</div>
<div class="card card-body">Bottom Card</div>

#### Spacer
```html
<div class="s-3"></div>
```

Spacers hold not content, they are just put into the document to sit between elements in a vertical flow.
