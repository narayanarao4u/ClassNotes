---
marp: true
theme: default
paginate: true
---
**Notes on RGB, HEX, and HSL in CSS:**

These are different ways to define **colors** in CSS:

---

### **1. RGB (Red, Green, Blue)**

* **Format**: `rgb(red, green, blue)`

* Each value ranges from **0 to 255**.

* Example:

  ```css
  color: rgb(255, 0, 0); /* Red */
  ```

* You can also use **RGBA** to include transparency:

  ```css
  color: rgba(0, 0, 255, 0.5); /* Semi-transparent blue */
  ```

---

### **2. HEX (Hexadecimal)**

* **Format**: `#RRGGBB` or shorthand `#RGB`

* Each pair (RR, GG, BB) is a hex number from `00` to `FF` (equivalent to 0–255 in decimal).

* Example:

  ```css
  color: #00FF00; /* Green */
  color: #000;    /* Black (shorthand) */
  ```

* HEX can also support alpha (transparency) as `#RRGGBBAA` in modern browsers.

---

### **3. HSL (Hue, Saturation, Lightness)**

* **Format**: `hsl(hue, saturation, lightness)`

  * Hue: Degree on color wheel (0–360)
  * Saturation: 0% (gray) to 100% (full color)
  * Lightness: 0% (black) to 100% (white)

* Example:

  ```css
  color: hsl(120, 100%, 50%); /* Bright green */
  ```

* HSLA adds transparency:

  ```css
  color: hsla(120, 100%, 50%, 0.5); /* Semi-transparent green */
  ```

---

**Summary**:

| Format | Example               | Transparency Support |
| ------ | --------------------- | -------------------- |
| RGB    | `rgb(0, 0, 255)`      | Yes (`rgba`)         |
| HEX    | `#0000FF`             | Yes (`#RRGGBBAA`)    |
| HSL    | `hsl(240, 100%, 50%)` | Yes (`hsla`)         |

Each format has its use case depending on preference, readability, or need for transparency.


---
### **Hue: Degree on Color Wheel (0–360°) – Explained**

**Hue** represents the **type of color** (like red, green, blue, etc.) and is measured in **degrees** on the **color wheel**, ranging from **0° to 360°**.


| Degree | Color                   |
| ------ | ----------------------- |
| 0°     | Red                     |
| 60°    | Yellow                  |
| 120°   | Green                   |
| 180°   | Cyan                    |
| 240°   | Blue                    |
| 300°   | Magenta                 |
| 360°   | Red (again, same as 0°) |

---

### 🌈 How It Works in HSL:

In CSS, when using `hsl(hue, saturation, lightness)`, the **hue** controls which color you see:

```css
color: hsl(0, 100%, 50%);    /* Bright red */
color: hsl(120, 100%, 50%);  /* Bright green */
color: hsl(240, 100%, 50%);  /* Bright blue */
```

* The **saturation** adjusts how pure or gray the color is.
* The **lightness** controls how dark or light the color appears.

---

### 🎨 Visual Tip:

Imagine a circle where:

* 0°–120° gives **warm colors** (reds, oranges, yellows),
* 120°–240° gives **cool colors** (greens, blues),
* 240°–360° gives **purples to reds** again.

So, **Hue** is like pointing to a position on a rainbow circle to pick the base color.
