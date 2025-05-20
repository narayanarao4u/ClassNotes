---
marp: true
theme: default
paginate: true
---



# Three different way of writing  css

There are three different ways to write and apply CSS to an HTML document:
1. **Inline CSS**
2. **Internal CSS (Embedded CSS)**
3. **External CSS**
----
1. **Inline CSS**
    - CSS rules are written directly inside an HTML element using the `style` attribute.
    - This method applies styles to a single element only.
    - Example: `<h1 style="color: blue;">A Blue Heading</h1>`
    - Inline CSS is generally discouraged for maintainability reasons, as it mixes content with presentation and can be inefficient for larger projects
    
---

2. **Internal CSS (Embedded CSS)**
    - CSS rules are placed inside a `<style>` element within the `<head>` section of the HTML document.
    - This method applies styles to the entire page and is useful for styling a single HTML document.
    - Example:

```html
<head>
  <style>
    body { background-color: blue; }
    h1 { color: red; padding: 60px; }
  </style>
</head>
```

    - Internal CSS allows the use of classes and IDs and keeps styles centralized for that page but can increase page size if overused

---

3. **External CSS**
    - CSS rules are written in a separate `.css` file which is linked to the HTML document using the `<link>` element inside the `<head>`.
    - This method allows one CSS file to style multiple HTML pages, promoting reusability and easier maintenance.
    - Example:

```html
<head>
  <link rel="stylesheet" href="styles.css">
</head>
```

- External CSS is the most common and recommended way to write CSS for larger websites due to its modularity and efficiency

In summary, the three ways to write CSS are **inline**, **internal (embedded)**, and **external** stylesheets, each with its own scope and use cases.

