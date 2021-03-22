---
layout: docs
title:  "Responsive"
---
This is a list of all the components that are responsive.
<ul>
  {% for page in site.pages %}
    {% if page.responsive == true %}
      <li>
        <a href="/docs/{{ page.title | downcase | replace: ' ', '-' }}">{{ page.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>


When you see the
<span class="d-inline-block">
  <a href="/docs/themeable" class="badge m-0 d-flex align-items-center compatibility-badge">
    <span class="badge-check">
      <img src="/img/icons/check.svg" />
    </span>
    <span>Responsive</span>
  </a>
</span> badge it means the component has responsive breakpoints for different sized screens. The breakpoint is anything 600px or wider is considered `lg` and anything under 600px is `sm`. By default everything is "mobile first" which means the default class is both screen sizes.

A class that uses the `-lg` infix is only large devices. For example `w-full` is `width: 100%` on all screen sizes. But `w-full w-lg-10` is `width: 100%` on small screens and `width: 40px` on large screen sizes.

Note: Some email clients like Gmail mobile do not support any media queries and so some responsive functions do not work on them.

Not everything that is responsive uses these names. For example the `.container` is responsive by default and expands and contracts on different screens.
