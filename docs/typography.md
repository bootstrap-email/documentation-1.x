---
layout: docs
title:  "Typography"
tagline: "Basic building blocks of text."
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
      <tr><td class="class">&lt;h1&gt;, .h1</td><td class="css">font-size: 36px;</td></tr>
      <tr><td class="class">&lt;h2&gt;, .h2</td><td class="css">font-size: 32px;</td></tr>
      <tr><td class="class">&lt;h3&gt;, .h3</td><td class="css">font-size: 28px;</td></tr>
      <tr><td class="class">&lt;h4&gt;, .h4</td><td class="css">font-size: 24px;</td></tr>
      <tr><td class="class">&lt;h5&gt;, .h5</td><td class="css">font-size: 20px;</td></tr>
      <tr><td class="class">&lt;h6&gt;, .h6</td><td class="css">font-size: 16px;</td></tr>
      <tr><td class="class">&lt;strong&gt;</td><td class="css">font-weight: bold;</td></tr>
      <tr><td class="class">&lt;em&gt;</td><td class="css">font-style: italic;</td></tr>
      <tr><td class="class">.underline, &lt;u&gt;</td><td class="css">text-decoration: underline;</td></tr>
      <tr><td class="class">.no-underline</td><td class="css">text-decoration: none;</td></tr>
      <tr><td class="class">.line-through, &lt;s&gt;</td><td class="css">text-decoration: line-through;</td></tr>
    </tbody>
  </table>
</div>

{% include header.html name="Usage" hr="false" %}
Many basic typography options. If you want more text control check out [Text Align](/docs/text-align), [Text Color](/docs/text-color), [Text Size](/docs/text-size), [Font Weight](/docs/font-weight), and [Line Height](/docs/line-height).
```html
<h1>h1</h1>
<h2>h2</h2>
<h3>h3</h3>
<h4>h4</h4>
<h5>h5</h5>
<h6>h6</h6>
<div class="h1">any tag as h1</div>
<div class="h2">any tag as h2</div>
<div class="h3">any tag as h3</div>
<div class="h4">any tag as h4</div>
<div class="h5">any tag as h5</div>
<div class="h6">any tag as h6</div>
<h1 class="display-1">Display 1</h1>
<h1 class="display-2">Display 2</h1>
<h1 class="display-3">Display 3</h1>
<h1 class="display-4">Display 4</h1>
<h1 class="display-5">Display 5</h1>
<h1 class="display-6">Display 6</h1>
<strong>bold text</strong>
<u>underlined text</u>
<em>italicized text</em>
<s>strike through text</s>
```

# h1
## h2
### h3
#### h4
##### h5
###### h6
# any tag as h1
## any tag as h2
### any tag as h3
#### any tag as h4
##### any tag as h5
###### any tag as h6
<strong>bold text</strong>
<u>underlined text</u>
<em>italicized text</em>
<s>strike through text</s>

{% include header.html name="Compiled Example" hr="true" %}
<span class="badge rounded-pill badge-input">Input</span>
```html
<h1>This is an h1</h1>
<h2>This is an h2</h2>
<h3>This is an h3</h3>
<h4>This is an h4</h4>
<h5>This is an h5</h5>
<h6>This is an h6</h6>
<strong>Bold Text</strong>
<strong>Bold Text</strong>
<u>Underlined Text</u>
<em>Italic Text</em>
<s>Strike Through Text</s>
```

<span class="badge rounded-pill badge-output">Output</span>
```html
<h1 style="padding-top: 0; padding-bottom: 0; font-weight: 500; vertical-align: baseline; font-size: 36px; line-height: 43.2px; margin: 0;" align="left">This is an h1</h1>
<h2 style="padding-top: 0; padding-bottom: 0; font-weight: 500; vertical-align: baseline; font-size: 32px; line-height: 38.4px; margin: 0;" align="left">This is an h2</h2>
<h3 style="padding-top: 0; padding-bottom: 0; font-weight: 500; vertical-align: baseline; font-size: 28px; line-height: 33.6px; margin: 0;" align="left">This is an h3</h3>
<h4 style="padding-top: 0; padding-bottom: 0; font-weight: 500; vertical-align: baseline; font-size: 24px; line-height: 28.8px; margin: 0;" align="left">This is an h4</h4>
<h5 style="padding-top: 0; padding-bottom: 0; font-weight: 500; vertical-align: baseline; font-size: 20px; line-height: 24px; margin: 0;" align="left">This is an h5</h5>
<h6 style="padding-top: 0; padding-bottom: 0; font-weight: 500; vertical-align: baseline; font-size: 16px; line-height: 19.2px; margin: 0;" align="left">This is an h6</h6>
<strong>Bold Text</strong>
<strong>Bold Text</strong>
<u>Underlined Text</u>
<em>Italic Text</em>
<s>Strike Through Text</s>
```
