Absolutely! In JavaScript, you can write functions in several different ways — each with its own syntax and use cases.

Here are the **main ways to define functions** in JavaScript, with examples:

---

## 1. ✅ Function Declaration (Named Function)

This is the traditional way to define a function.

```javascript
function greet(name) {
  return "Hello, " + name;
}
console.log(greet("Alice")); // Hello, Alice
```

✅ **Hoisted** — you can call it before it's defined.

---

## 2. ✅ Function Expression

Here, the function is stored in a variable.

```javascript
const greet = function(name) {
  return "Hi, " + name;
};
console.log(greet("Bob")); // Hi, Bob
```

🚫 **Not hoisted** — must be defined before it’s used.

---

## 3. ✅ Arrow Function (ES6)

A shorter syntax introduced in ES6.

```javascript
const greet = (name) => {
  return "Hey, " + name;
};
console.log(greet("Charlie")); // Hey, Charlie
```

👉 If the function has a single return statement, you can shorten it:

```javascript
const greet = name => "Hey, " + name;
```

🚫 No `this`, `arguments`, or `super` binding — best for small, simple functions.

---

## 4. ✅ Anonymous Function

A function **without a name**, usually used as a callback or in expressions.

```javascript
setTimeout(function() {
  console.log("This runs after 1 second");
}, 1000);
```

---

## 5. ✅ Immediately Invoked Function Expression (IIFE)

Runs immediately after being defined.

```javascript
(function() {
  console.log("This runs instantly!");
})();
```

🔐 Often used to create private scope.

---

## 6. ✅ Function Constructor (Not recommended for most cases)

```javascript
const sum = new Function("a", "b", "return a + b");
console.log(sum(3, 4)); // 7
```

⚠️ Not recommended due to security and performance issues.

---

## 📝 Summary Table

| Type                 | Syntax Example                  | Hoisted?           | Use Case                            |
| -------------------- | ------------------------------- | ------------------ | ----------------------------------- |
| Function Declaration | `function greet() {}`           | ✅ Yes              | Reusable named functions            |
| Function Expression  | `const greet = function() {}`   | ❌ No               | Assign to variables or pass around  |
| Arrow Function       | `const greet = () => {}`        | ❌ No               | Short, clean syntax (no `this`)     |
| Anonymous Function   | `function() {}`                 | ❌ No               | Inline callbacks, like `setTimeout` |
| IIFE                 | `(function() { })();`           | ✅ Runs immediately | Private scope                       |
| Function Constructor | `new Function("a", "b", "...")` | ❌ No               | Rare, dynamic use cases only        |

---

Would you like a visual chart or practice task on this for students?
