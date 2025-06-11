---
marp: true
---

# 📌 CSS `position` Property — Complete Notes with Examples

The `position` property in CSS specifies how an element is positioned in the document.

---

## 🔹 1. `static` (Default)

* Elements are positioned in the **normal flow**.
* `top`, `right`, `bottom`, and `left` have **no effect**.

```html
<div class="box static">Static Position</div>
```

```css
.static {
  position: static;
  background: lightgray;
}
```

✅ **Used when no specific positioning is needed.**

---

## 🔹 2. `relative`

* Element is positioned **relative to its normal position**.
* Can be shifted using `top`, `left`, `right`, `bottom`.

```html
<div class="box relative">Relative Position</div>
```

```css
.relative {
  position: relative;
  top: 10px;
  left: 20px;
  background: lightblue;
}
```

✅ **Useful for offsetting an element slightly without affecting layout flow.**

---

## 🔹 3. `absolute`

* Positioned **relative to the nearest positioned ancestor** (not `static`).
* If none found, positioned relative to the `<html>`.

```html
<div class="parent">
  <div class="box absolute">Absolute Position</div>
</div>
```

```css
.parent {
  position: relative;
  width: 300px;
  height: 150px;
  background: #eee;
}

.absolute {
  position: absolute;
  top: 10px;
  right: 10px;
  background: salmon;
}
```

✅ **Use inside relatively positioned containers for flexible placement.**

---

## 🔹 4. `fixed`

* Positioned **relative to the viewport** (browser window).
* Stays in place during scroll.

```html
<div class="box fixed">Fixed Position</div>
```

```css
.fixed {
  position: fixed;
  bottom: 0;
  right: 0;
  background: lightgreen;
  padding: 10px;
}
```

✅ **Great for sticky headers, footers, or floating buttons.**

---

## 🔹 5. `sticky`

* Switches between **relative and fixed** based on scroll.
* Requires a `top`, `left`, `right`, or `bottom` value.

```html
<h2 class="sticky">Sticky Heading</h2>
```

```css
.sticky {
  position: sticky;
  top: 0;
  background: orange;
  padding: 10px;
}
```

✅ **Used for sticky headers that remain until next section arrives.**

---

## 🧱 Summary Table

| Value      | Description                                | Scroll Behavior               |
| ---------- | ------------------------------------------ | ----------------------------- |
| `static`   | Default, follows normal flow               | Scrolls with page             |
| `relative` | Offset from normal position                | Scrolls with page             |
| `absolute` | Positioned relative to ancestor            | Stays unless ancestor scrolls |
| `fixed`    | Positioned relative to viewport            | Does **not** scroll           |
| `sticky`   | Scrolls until reaching offset, then sticks | Partially scrolls             |

---


