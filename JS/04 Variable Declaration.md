Here are the **rules for JavaScript variable declaration**:

---

### 🔹 1. **Use of `var`, `let`, or `const`**

* `var` – Function-scoped (older way).
* `let` – Block-scoped; allows reassignment.
* `const` – Block-scoped; **cannot** be reassigned after declaration.

---

### 🔹 2. **Variable Names (Identifiers) Must:**

* Begin with a **letter**, **underscore (`_`)**, or **dollar sign (`$`)**.
* **Not start with a number**.
* Be **case-sensitive** (`age` and `Age` are different).
* Not be a **reserved keyword** (e.g., `class`, `return`, `if`, etc.).

---

### 🔹 3. **Declaration Before Use**

* Variables declared with `let` and `const` are not accessible before declaration (Temporal Dead Zone).
* `var` is hoisted but initialized as `undefined`.

---

### 🔹 4. **Avoid Redeclaration**

* `let` and `const` **cannot** be redeclared in the same scope.
* `var` **can** be redeclared (not recommended due to confusion).

---

### 🔹 5. **Initialize If Needed**

* `let` and `var` can be declared without initialization.
* `const` **must** be initialized when declared.

---

### ✅ Example:

```javascript
var name = "Alice";     // OK
let age = 25;           // OK
const country = "India"; // OK

let _score = 100;       // OK
let $bonus = 20;        // OK

// let 2num = 10;       // ❌ Invalid: starts with a number
// const class = "A";   // ❌ Invalid: 'class' is a reserved keyword
```

```javascript
// Using var
var name;
console.log(name); // Output: undefined

// Using let
let ;
console.log(age); // Output: undefined

age = 95;
console.log(age); // Output: 95

// Using const (❌ this will cause an error)
const country;     // ❌ SyntaxError: Missing initializer in const declaration

```
