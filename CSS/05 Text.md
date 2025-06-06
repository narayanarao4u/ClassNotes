---
marp: true
theme: gaia
paginate: true
header: 'BSNL Training Point, Visakhapatnam'
# size: 4:3
---

# 📝 CSS Text Properties Cheat Sheet

## 🎨 Text Color

```css
color: blue;
```

* Changes the text color.

---

## 📐 Text Alignment

```css
text-align: center;
text-align-last: right;
```

* `text-align`: Aligns text (`left`, `right`, `center`, `justify`).
* `text-align-last`: Aligns the last line in a block.

---

## 🔁 Text Direction

```css
direction: rtl;
unicode-bidi: bidi-override;
```

* `direction`: Sets text flow direction (`ltr` or `rtl`).
* `unicode-bidi`: Used with `direction` for complex layouts.

---

## 🔄 Writing Mode

```css
writing-mode: vertical-rl;
```

* Controls text flow direction:

  * `horizontal-tb` (default)
  * `vertical-rl`
  * `vertical-lr`

---

## 🧭 Vertical Alignment

```css
vertical-align: baseline;
```

* Options: `text-top`, `text-bottom`, `baseline`, `sub`, `super`

---

## ✏️ Text Decoration

```css
text-decoration-line: underline;
text-decoration-color: blue;
text-decoration-style: solid;
text-decoration-thickness: 5px;
```

Or shorthand:

```css
text-decoration: underline red double 5px;
```

* Styles: `underline`, `overline`, `line-through`
* Line style: `solid`, `double`, `dotted`, `dashed`, `wavy`

---

## 🔤 Text Transform

```css
text-transform: uppercase;
```

* Options: `uppercase`, `lowercase`, `capitalize`

---

## ↔️ Spacing and Indents

```css
text-indent: 50px;
letter-spacing: 5px;
word-spacing: 10px;
```

* Negative spacing also allowed:

```css
letter-spacing: -2px;
word-spacing: -2px;
```

---

## 📏 Line Height

```css
line-height: 1.8;
```

* Controls vertical spacing between lines.

---

#### 🌫️ Text Shadow

```css
text-shadow: 2px 2px red;
text-shadow: 2px 2px 5px red;
```
More complex:
```css
text-shadow: 1px 1px 2px black, 0 0 25px blue, 0 0 5px darkblue;
```


#### 🔗 Example with YouTube Link Style

```css
color: white;
text-shadow: 1px 1px 2px black, 0 0 25px blue, 0 0 5px darkblue;
```
* Useful for glowing text effect.

---

## 📹 Youtube

[Watch CSS Box-Shadow tutorial: the basics](https://www.youtube.com/watch?v=-JNRQ5HjNeI)



