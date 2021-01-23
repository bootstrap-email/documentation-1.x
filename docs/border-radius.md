---
layout: docs
title:  "Border Radius"
badges: true
themeable: false
responsive: false
---
<div class="table-utilities">
  <table class="table">
    <thead>
      <tr>
        <th>Class</th>
        <th>Properties</th>
      </tr>
    </thead>
    <tbody>
      <tr><td>.border-0</td><td>border-radius: 0;</td></tr>
      <tr><td>.border-sm</td><td>border-radius: 0;</td></tr>
    </tbody>
  </table>
</div>


@include border-radius-util('.rounded-0') {
  border-radius: 0;
}

@include border-radius-util('.rounded-sm') {
  border-radius: $border-radius-sm;
}

@include border-radius-util('.rounded') {
  border-radius: $border-radius;
}

@include border-radius-util('.rounded-top') {
  border-top-left-radius: $border-radius;
  border-top-right-radius: $border-radius;
}

@include border-radius-util('.rounded-right') {
  border-top-right-radius: $border-radius;
  border-bottom-right-radius: $border-radius;
}

@include border-radius-util('.rounded-bottom') {
  border-bottom-right-radius: $border-radius;
  border-bottom-left-radius: $border-radius;
}

@include border-radius-util('.rounded-left') {
  border-top-left-radius: $border-radius;
  border-bottom-left-radius: $border-radius;
}

@include border-radius-util('.rounded-lg') {
  border-radius: $border-radius-lg;
}

@include border-radius-util('.rounded-xl') {
  border-radius: $border-radius-xl;
}

@include border-radius-util('.rounded-pill') {
  border-radius: $border-radius-pill;
}
