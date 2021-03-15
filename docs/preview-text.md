---
layout: docs
title:  "Preview Text"
tagline: "Like a second subject for your emails."
sections:
  - Usage
  - Compiled Example
badges: false
---
If you aren't familiar with preview text, it is the text that shows up in your inbox as a preview of the content inside the email. Here is more info about what it is and how it works on [Litmus.com](https://litmus.com/blog/the-ultimate-guide-to-preview-text-support)
<img class="d-block mx-auto w-50" src="/img/email-preview-text.png"/>

{% include header.html name="Usage" hr="true" %}
Bootstrap Email has a custom `<preview>` tag you can use to define preview text in your emails. This way it will show up as a preview of your email in your inbox but will be completely hidden when viewing the email itself.

```html
<preview>This text will show up as a preview but not in the email!</preview>
```

The message will also be padded with `&nbsp;` at the end of the message so that if you have a short preview text the contents of the email will not flow into the inbox preview.

Note: This element will be moved to just under the `<body>` tag when compiled. I would suggest keeping it in the top of your document for your sake but it can really be anywhere.

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<preview>Act quick before the offer ends!</preview>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<div class="preview" style="display: none; max-height: 0px; overflow: hidden;">
  Act quick before the offer ends&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</div>
```
