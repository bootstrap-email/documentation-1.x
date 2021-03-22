---
layout: docs
title:  "Card"
tagline: "White wrapper with a default gray border."
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
      <tr><td class="class">.card</td><td class="css">background-color: white; border: 1px solid #e2e8f0; border-radius: 6px;</td></tr>
      <tr><td class="class">.card-body</td><td class="css">padding: 20px;</td></tr>
    </tbody>
  </table>
</div>


{% include header.html name="Usage" hr="false" %}
Use to wrap content in a solid gray bordered container with rounded corners. Works well sitting on top of an email body with a `.bg-light` class and inside of a `.container`.

By default `.card` has no padding, you can use a card with or without a `.card-body`. Just like in Bootstrap a `.card-body` is just used to give `20px` padding to the card, you can also use a [padding](/docs/padding) utility to customize padding.

```html
<div class="card">
  <div class="card-body">
    This is some text within a card body.
  </div>
</div>
```

<div class="card">
  <div class="card-body">
    This is some text within a card body.
  </div>
</div>


{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<div class="card">
  <div class="card-body">
    Some quick example text to build on the card title and make up the bulk of the card's content.
  </div>
</div>

```

<span class="badge rounded-pill badge-output">Output</span>
```html
<table class="card" role="presentation" border="0" cellpadding="0" cellspacing="0" style="border-radius: 6px; border-collapse: separate !important; width: 100%; overflow: hidden; border: 1px solid #e2e8f0;" bgcolor="#ffffff">
  <tbody>
    <tr>
      <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0;" align="left" bgcolor="#ffffff">
        <table class="card-body" role="presentation" border="0" cellpadding="0" cellspacing="0" style="width: 100%;">
          <tbody>
            <tr>
              <td style="line-height: 24px; font-size: 16px; width: 100%; margin: 0; padding: 20px;" align="left">
                Some quick example text to build on the card title and make up the bulk of the card's content.
              </td>
            </tr>
          </tbody>
        </table>
      </td>
    </tr>
  </tbody>
</table>
```
