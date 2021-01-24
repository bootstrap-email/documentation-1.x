---
layout: docs
title:  "Grid"
badges: true
themeable: false
responsive: true
---
Grids work just like they do in Bootstrap, based on a 12 column grid. Make a row and give it columns. By default the grid holds it's structure on every device. It has a default horizontal gutter between elements, to customize horizontal and vertical gutters see the [Gutter Docs](/docs/gutters).

```html
<div class="row">
  <div class="col-3">.col-3</div>
  <div class="col-4">.col-4</div>
  <div class="col-5">.col-5</div>
</div>
```

<div class="row mb-4">
  <div class="col-3"><div class="border">.col-3</div></div>
  <div class="col-4"><div class="border">.col-4</div></div>
  <div class="col-5"><div class="border">.col-5</div></div>
</div>

#### Responsive
You can use the responsive <code>lg</code> modifier to make the grid snap back to vertical stacking on smaller devices.

```html
<div class="row">
  <div class="col-lg-3">.col-3</div>
  <div class="col-lg-4">.col-4</div>
  <div class="col-lg-5">.col-5</div>
</div>
```

<div class="row">
  <div class="col-lg-3"><div class="border">.col-3</div></div>
  <div class="col-lg-4"><div class="border">.col-4</div></div>
  <div class="col-lg-5"><div class="border">.col-5</div></div>
</div>
