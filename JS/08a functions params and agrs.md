Here's the Markdown representation of the text in the image:

```markdown
## Declare a function and paraments
```
```javascript
function functionName(parameters) {
    // ... body
}
```

## Calling a function

```javascript
functionName(arguments);
```

## Parameters vs. Arguments

## Returning a value

### Every function in JavaScript implicitly returns `undefined` unless you explicitly specify a return value.



----

Sure! Let’s break down the difference between **parameters** and **arguments** in JavaScript functions — a concept often confused by beginners.

---

## 🧠 Basic Idea

* **Parameters** are the names listed in the **function definition**.
* **Arguments** are the actual values passed to the function **when it is called**.

---

## ✅ Example:

```javascript
function greet(name, age) {
  console.log("Hello " + name + ", age: " + age);
}

greet("Alice", 25);
```

* `name` and `age` → **Parameters** (placeholders in function definition)
* `"Alice"` and `25` → **Arguments** (actual values passed to the function)

---

## 🎯 Think of it like this:

> Parameters are like **empty boxes**.
> Arguments are the **things you put in the boxes** when calling the function.

---

## 📌 Summary Table

| Term      | Where It Appears       | Example              |
| --------- | ---------------------- | -------------------- |
| Parameter | In function definition | `function add(a, b)` |
| Argument  | In function call       | `add(5, 3)`          |

---

## 🔄 Multiple Parameters & Arguments

You can pass multiple arguments to match multiple parameters:

```javascript
function fullName(first, last) {
  return first + " " + last;
}

console.log(fullName("John", "Doe")); // John Doe
```

---

## 🔥 Bonus: Default Parameters

You can give default values to parameters:

```javascript
function greet(name = "Guest") {
  console.log("Hello " + name);
}

greet();           // Hello Guest
greet("Charlie");  // Hello Charlie
```

---

Let me know if you'd like some interactive student exercises or a quiz on this!
