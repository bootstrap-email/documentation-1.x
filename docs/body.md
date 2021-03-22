---
layout: docs
title:  "Body"
tagline: "Basic page structure for better email compatibility."
sections:
  - Compiled Example
---

There is nothing that you need to do here but good information to know. A table with the class `.body` will **automatically** wrap the email content and applies styles to give more consistent layout to the page. You can put classes on the `<body>` that will be moved onto the body table.

<a class="anchor" name="compiled-example"></a>
<h2 class="h3">Compiled Example</h2>

<span class="badge rounded-pill badge-input">Input</span>
```html
<body class="bg-light">
  ...
</body>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<body>
  <table class="body bg-light">
    ...
  </table>
</body>
```
