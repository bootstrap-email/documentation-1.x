---
layout: docs
title:  "Images"
badges: true
themeable: false
responsive: true
---
Images can be very complicated in emails. Luckily Bootstrap email makes it easy. To keep an element full width of it's container, give it the `img-fluid`. Doing so will set properties like the `width="100%"` attribute on the img tag which is reguired for Outlook rendering. For more options on sizing images check out the [Sizing Docs](/docs/sizing).

```html
<img class="img-fluid" src="https://bootstrapemail.com/some/image.png" alt="Some Image" />
```
