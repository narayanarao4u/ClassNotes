

---

## 📝 HTML Formatting Tags

These tags help in **styling and emphasizing** text visually and semantically.

| Tag            | Meaning / Use                           | Example Output                                      |
| -------------- | --------------------------------------- | --------------------------------------------------- |
| `<b>`          | Bold text (no extra importance)         | **Bold**                                            |
| `<strong>`     | Important text (semantically strong)    | **Strong**                                          |
| `<i>`          | Italic text (no emphasis)               | *Italic*                                            |
| `<em>`         | Emphasized text (with importance)       | *Emphasized*                                        |
| `<mark>`       | Highlighted/marked text                 | <mark>Marked</mark>                                 |
| `<u>`          | Underlined text                         | <u>Underline</u>                                    |
| `<small>`      | Smaller text                            | <small>Small</small>                                |
| `<del>`        | Deleted text (strikethrough)            | <del>Deleted</del>                                  |
| `<ins>`        | Inserted text (underlined)              | <ins>Inserted</ins>                                 |
| `<sub>`        | Subscript text                          | H<sub>2</sub>O                                      |
| `<sup>`        | Superscript text                        | E = mc<sup>2</sup>                                  |
| `<code>`       | Inline computer code                    | <code>let x = 5;</code>                             |
| `<pre>`        | Preformatted text (preserves spacing)   | Pre-formatted block                                 |
| `<abbr>`       | Abbreviation (with tooltip on hover)    | <abbr title="HyperText Markup Language">HTML</abbr> |
| `<blockquote>` | Long quotation                          | Indented quote block                                |
| `<q>`          | Short inline quotation                  | <q>Inline quote</q>                                 |
| `<cite>`       | Citation (e.g. book or article title)   | <cite>Hamlet</cite>                                 |
| `<kbd>`        | Keyboard input                          | <kbd>Ctrl + C</kbd>                                 |
| `<s>`          | No longer accurate text (strikethrough) | <s>Old Price</s>                                    |
| `<var>`        | Variable name in math/code              | <var>x</var> = 5                                    |
| `<dfn>`        | Defines a term                          | <dfn>Browser</dfn>                                  |

---
### Progress
----
```html
<progress  > 32% </progress>
<progress  value="32" max="100"> 32% </progress>
```
<div>Loading</div>
<progress  > 32% </progress>
<hr>
<div>File Download Progress:</div>
<progress  value="32" max="100"> 32% </progress>

### Meter

```html
<meter  value="0.6">60%</meter>

<meter  value="2" min="0" max="10">

```
<div>Disk  Usage:</div>
<meter  value="0.6">60%</meter>
<div>Credits  Used:</div>
<meter  value="2" min="0" max="10">