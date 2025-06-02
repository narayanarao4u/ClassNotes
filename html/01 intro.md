---
marp: true
theme: gaia
paginate: true
header: 'BSNL Training Point, Visakhapatnam'
# size: 4:3
---

# Introduction to Web Development
 BSNL Training Point, Visakhapatnam


---

## What is HTML

- **HTML**,  stands for **HyperText Markup Language**
- **HTML** is the standard language used to create and structure content on the web
 
- It is not a programming language but a markup language, means it is designed to  "mark up" content so that web browsers can interpret and display it correctly.

- The term "HyperText" refers to the ability to link pages and navigate between them using hyperlinks,
-  "Markup Language" refers to the tags  of content.


---
### **Code Editor: VS Code + Live Server**

- **VS Code**: A powerful, user-friendly code editor.
  - Syntax highlighting, IntelliSense, and debugging.
  - Supports many extensions for enhanced functionality.

- **Live Server Extension**:
  - **Real-Time Preview**: Automatically refreshes the browser when code is saved.
  - **Easy to Use**: Right-click your HTML file and choose "Open with Live Server."

**Why Use It?**  - No need to manually refresh the page.



---
## Brief overview of the most essential parts of an HTML document.
**Key Sections:**
1. **`<!DOCTYPE html>`** – Declares HTML5.
2. **`<html>`** – Root element of the page.
3. **`<head>`** – Metadata and title (appears in the browser tab).
4. **`<body>`** – Visible content (headings, text, etc.). 
---
### **Basic HTML Page Structure**
```html
<!DOCTYPE html>
<html>
  <head>
   

  </head>
  <body>
   
  </body>
</html>
```
---

### **HTML Text Elements**

HTML provides various elements to format and structure text on a web page

- **`<h1>` to `<h6>`**: Headings, with `<h1>` being the largest and `<h6>` the smallest.
- **`<p>`**: Defines a paragraph.
- **`<br>`**: Inserts a line break.
  - Example: `First line<br>Second line`

---
- **`<strong>`**: Defines strong importance (bold text).
- **`<em>`**: Emphasizes text (italicized).
- **`<ins>`** - Inserted text
- **`<del>`** - Deleted text


- **`<blockquote>`**: Defines a block of quoted text.
  - Example: `<blockquote>This is a blockquote.</blockquote>`

- **`<span>`**: An inline container for text and styling without adding structure.
  - Example: `<span style="color: red;">Red text</span>`
---
- **`<b>`** and **`<i>`**: Used for bold (`<b>`) and italic (`<i>`) text, but without semantic importance.
  - Example: `<b>Bold</b> and <i>Italic</i> text`
- **`<sub>`** - - Subscript text
- **`<sup>`** - - Superscript text
- **`<q>`** - tag defines a short quotation.
- **`<mark>`** -  Marked text.


---
## List Elements

 Unordered HTML List

```html
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```
---
Ordered HTML List
```html  
<ol type="I" start="50">
    <li>Coffee</li>
    <li>Tea</li>
    <li>Milk</li>
</ol>
```

type="1"	 numbers (default)
type="A"	uppercase letters
type="a"	lowercase letters
type="I"	uppercase roman numbers
type="i"	lowercase roman numbers

