---
layout: docs
title:  "Hr"
tagline: "Horizontal rule that looks the same in every email client."
sections:
  - Class Reference
  - Usage
  - Compiled Example
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
      <tr><td class="class">&lt;hr&gt;</td><td class="result">gray horizontal rule full width</td></tr>
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Add a horizontal rule to separate content. A consistent one that works and looks good in all email clients. By default it has top and bottom spacing of 20px, to use different top and bottom margin us a [margin](/docs/spacing) utility class.

```html
<hr>
Hello
<hr class="my-0"> <!-- no top or bottom margin -->
```
<hr>
Hello
<hr class="my-0"> <!-- no top or bottom margin -->

{% include header.html name="Compiled Example" hr="false" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<hr>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="s-5 w-full" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%;" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 20px; font-size: 20px; width: 100%; height: 20px; margin: 0;" align="left" width="100%" height="20">
         
      </td>
    </tr>
  </tbody>
</table>
<table class="hr" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%;">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; border-top-width: 1px; border-top-color: #e2e8f0; border-top-style: solid; height: 1px; width: 100%; margin: 0;" align="left">
      </td>
    </tr>
  </tbody>
</table>
<table class="s-5 w-full" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%;" width="100%">
  <tbody>
    <tr>
      <td style="line-height: 20px; font-size: 20px; width: 100%; height: 20px; margin: 0;" align="left" width="100%" height="20">
         
      </td>
    </tr>
  </tbody>
</table>
```
