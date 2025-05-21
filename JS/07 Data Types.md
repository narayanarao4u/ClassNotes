Here are concise notes with examples for both primitive and non-primitive data types in JavaScript. These are great for teaching students the fundamentals.

---

## 🧠 Primitive Data Types in JavaScript

Primitive types are basic data types that store **single values**. They are immutable and are stored by value.

### 1. String

Represents textual data.

```javascript
let name = "Alice";
```

### 2. Number

Represents both integer and floating-point numbers.

```javascript
let age = 25;
let price = 10.5;
```

### 3. Boolean

Represents true or false.

```javascript
let isStudent = true;
```

### 4. Undefined

A variable that has been declared but not assigned a value.

```javascript
let x;
console.log(x); // undefined
```

### 5. Null

Represents the intentional absence of any value.

```javascript
let result = null;
```

### 6. Symbol (ES6)

Used to create unique identifiers.

```javascript
let id = Symbol("id");
```

### 7. BigInt (ES11)

Used for integers larger than the Number type can hold.

```javascript
let bigNumber = 1234567890123456789012345678901234567890n;
```

---

## 📦 Non-Primitive (Reference) Data Types

Non-primitive types can hold **multiple values** and are stored by reference.

### 1. Object

A collection of key-value pairs.

```javascript
let person = {
  name: "Alice",
  age: 25
};
```

### 2. Array

A list-like object.

```javascript
let colors = ["red", "green", "blue"];
```

### 3. Function

A block of code designed to perform a task.

```javascript
function greet() {
  console.log("Hello!");
}
```

### 4. Date, RegExp, Map, Set, etc.

Other built-in object types.

```javascript
let today = new Date();
let pattern = /abc/;
let map = new Map();
```

---

## 🧪 Quick Comparison

| Feature   | Primitive      | Non-Primitive           |
| --------- | -------------- | ----------------------- |
| Stored by | Value          | Reference               |
| Mutable   | ❌ No           | ✅ Yes                   |
| Examples  | string, number | object, array, function |
----

*Mutable means changeable — the data can be modified after it's created.*

---

* Primitive types are stored by value directly in the variable.

* Non-primitive types (objects, arrays, functions, etc.) are stored by reference. The variable holds a reference (or pointer) to the location in memory where the actual data is stored.

----

| Data Type | Mutable? | Example         |
| --------- | -------- | --------------- |
| String    | ❌ No     | `"Hello"`       |
| Number    | ❌ No     | `42`            |
| Boolean   | ❌ No     | `true`          |
| Object    | ✅ Yes    | `{ name: "A" }` |
| Array     | ✅ Yes    | `[1, 2, 3]`     |
| Function  | ✅ Yes    | `function() {}` |
