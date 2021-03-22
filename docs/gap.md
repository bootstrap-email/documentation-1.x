---
layout: docs
title:  "Gap"
tagline: "Add spacing between elements in a Grid or Stack."
sections:
  - Class Reference
  - Usage
  - Grid
  - Stack
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
      {% for size in site.data.spacings %}
        <tr><td class="class">.gap-{{ size }}</td><td class="result">{{ size | times: 4 }}px gap on all sides</td></tr>
      {% endfor %}
      {% for size in site.data.spacings %}
        <tr><td class="class">.gap-x-{{ size }}</td><td class="result">{{ size | times: 4 }}px horizontal gap</td></tr>
      {% endfor %}
      {% for size in site.data.spacings %}
        <tr><td class="class">.gap-y-{{ size }}</td><td class="result">{{ size | times: 4 }}px vertical gap</td></tr>
      {% endfor %}
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Just like the margin and padding classes, multiply the class number by 4px to get the size. Ex. gap-10 is 40px.

{% include header.html name="Grid" hr="true" %}
By default the grid `.row` class has `24px` horizontal gutters. You can apply these gap classes to the row class to change horizontal and vertical gutters `row gap-4` will add `16px` gutters on all sizes. Top and bottom gutters are useful for when a grid is responsive and stacks columns vertically on mobile. [More about using Gap with Grid](/docs/grid#gap)

{% include header.html name="Stack" hr="true" %}
Use gap here to spread elements in a stack, horizontally if it is a `stack-x` and vertically if it is a `stack-y`. [More about using Gap with Stacks](/docs/grid#gap)
