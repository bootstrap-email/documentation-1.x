---
layout: docs
title:  "Images"
tagline: "Images are made simple with Bootstrap Email."
sections:
  - Class Reference
  - Usage
  - Accessibility
  - Compiled Example
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
      <tr><td class="class">.img-fluid</td><td class="css">
        height: auto;<br>
        max-width: 100%;<br>
        width: 100%;
      </td></tr>
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Images can be very complicated in emails. Luckily Bootstrap email makes it easy. Images need to have at leave have either a width or a height for them to render properly in something like Outlook. To keep an element full width of it's container, give it the `img-fluid`. Doing so will set properties like the `width="100%"` attribute on the img tag which is required for Outlook rendering.

```html
<img class="img-fluid" src="https://bootstrapemail.com/some/image.png" alt="Some Image" />
```

For doing something other than 100% image with, use the sizing width and height utility classes with your images: [Sizing Docs](/docs/sizing).

{% include header.html name="Accessibility" hr="true" %}
Make sure you include a descriptive `alt` property on every image, not only does this help with accessibility but it's not uncommon for images to be blocked in an email client and this helps user see what image is being blocked. [More on alt tags](https://moz.com/learn/seo/alt-text)

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<img class="img-fluid" src="https://bootstrapemail.com/some/image.png" alt="Some Image" />
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<img class="img-fluid" src="https://bootstrapemail.com/some/image.png" alt="Some Image" style="height: auto; line-height: 100%; outline: none; text-decoration: none; display: block; max-width: 100%; width: 100%; border: 0 none;" width="100%">
```
