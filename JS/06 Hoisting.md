<link rel="stylesheet" href="_styles.css">
### 🔹 What is **Hoisting** in JavaScript?

**Hoisting** is JavaScript's default behavior of **moving declarations to the top of their scope** (either the function or global scope) **before the code is executed**.

But **only the declarations are hoisted**, not the initializations (assignments).

---

### 🔸 How it works:

When JavaScript runs your code, it scans for variable and function **declarations** and brings them to the top of their scope.

---

### ✅ **Examples**

#### 1. **Variable Hoisting with `var`**:

```javascript
console.log(x); // Output: undefined
var x = 5;
```

Behind the scenes, JavaScript treats it like:

```javascript
var x;
console.log(x); // undefined
x = 5;
```

---

#### 2. **Variable Hoisting with `let` and `const`**:

```javascript
console.log(y); // ❌ ReferenceError
let y = 10;
```

* `let` and `const` are **hoisted**, but they are in a **"temporal dead zone" (TDZ)** from the start of the block until their declaration is encountered.
* Accessing them before the line they're declared on causes an error.

---

#### 3. **Function Hoisting**:

```javascript
greet(); // Output: Hello

function greet() {
  console.log("Hello");
}
```

* **Function declarations** are fully hoisted — both their name and body.
* But **function expressions** are **not** hoisted in the same way:

```javascript
sayHi(); // ❌ TypeError: sayHi is not a function

var sayHi = function() {
  console.log("Hi");
};
```

---

### ✅ Summary Table:

| Declaration Type      | Hoisted? | Accessible Before Declaration? | Notes                                  |
| --------------------- | -------- | ------------------------------ | -------------------------------------- |
| `var`                 | ✅ Yes    | ✅ Yes (but `undefined`)        | Hoisted and initialized as `undefined` |
| `let`                 | ✅ Yes    | ❌ No (ReferenceError)          | Hoisted but not initialized (TDZ)      |
| `const`               | ✅ Yes    | ❌ No (ReferenceError)          | Must be initialized when declared      |
| `function` (declared) | ✅ Yes    | ✅ Yes                          | Entire function is hoisted             |
| Function expression   | ✅ (var)  | ❌ No                           | Only variable name is hoisted          |

Let me know if you want visuals or animations to help understand hoisting better!
