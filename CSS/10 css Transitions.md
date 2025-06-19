---
marp: true
theme: default
paginate: true
---


# 🎬 CSS Transitions – Smoothly Animate Changes

CSS Transitions allow you to change property values **smoothly over a duration** — instead of instantly.

---

## ✅ Syntax

```css
selector {
  transition: property duration timing-function delay;
}
```

### ✨ Example:

```css
.box {
  background-color: blue;
  transition: background-color 0.5s ease;
}

.box:hover {
  background-color: red;
}
```

🟦 When you hover over the `.box`, it **gradually changes** color from blue to red.

---

## 🔹 Transition Properties

| Property                     | Description                                          |
| ---------------------------- | ---------------------------------------------------- |
| `transition-property`        | The CSS property to animate (`width`, `color`, etc.) |
| `transition-duration`        | How long the transition lasts (`s` or `ms`)          |
| `transition-timing-function` | Acceleration curve (`ease`, `linear`, etc.)          |
| `transition-delay`           | Wait time before transition starts                   |

---

## 🔸 Common Timing Functions

| Function                | Description                        |
| ----------------------- | ---------------------------------- |
| `ease`                  | Starts slow, speeds up, then slows |
| `linear`                | Same speed from start to finish    |
| `ease-in`               | Starts slow                        |
| `ease-out`              | Ends slow                          |
| `ease-in-out`           | Slow start and end                 |
| `cubic-bezier(n,n,n,n)` | Custom curve                       |

---

## 🧪 Multi-property Example

```css
.box {
  width: 100px;
  height: 100px;
  background: orange;
  transition: width 0.5s, background 0.3s ease-in;
}

.box:hover {
  width: 200px;
  background: teal;
}
```

✅ **Multiple properties** can be animated together with different durations.

---

## 🧰 Real-life Use Cases

* Button hover effects
* Menu slide-ins
* Form field highlighting
* Tooltip fade-ins

---

## 🔍 Summary

* Transitions make UI changes feel **natural** and **responsive**
* Works only on properties that can be **interpolated** (e.g., color, size, position)
* Simple to use with just a few lines of CSS

