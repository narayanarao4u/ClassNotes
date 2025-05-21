
## ⏱ What is `setTimeout()`?

`setTimeout()` is a built-in JavaScript function that lets you run code **after a delay**.

### 🧠 Syntax:

```javascript
setTimeout(function, delayInMilliseconds);
```

* `function` → The code to run after the delay (can be a function or arrow function)
* `delayInMilliseconds` → Time to wait before running (1 second = 1000 milliseconds)

---

## ✅ Example:

```javascript
setTimeout(function() {
  console.log("This runs after 2 seconds");
}, 2000);
```

Output after 2 seconds:

```
This runs after 2 seconds
```

✅ You can also use arrow functions:

```javascript
setTimeout(() => {
  console.log("Hello after 1 second");
}, 1000);
```

---

## 🧩 Why use `setTimeout()`?

* To **delay execution**
* To **simulate waiting** for something (like loading or response)
* To **schedule** actions

---

## 📌 Real-life analogy:

> “Hey, remind me in 5 seconds to drink water.”
> That’s `setTimeout()` acting like a timer-based reminder.

---

## 🔄 Cancel a Timeout

If you want to stop the scheduled code, use `clearTimeout()`:

```javascript
let id = setTimeout(() => {
  console.log("This will NOT run");
}, 3000);

clearTimeout(id);
```

The `clearTimeout(id)` cancels the scheduled function.

---

## ❗Important Notes:

| Fact               | Details                                         |
| ------------------ | ----------------------------------------------- |
| Non-blocking       | Code after `setTimeout()` continues immediately |
| Runs once          | It only runs once after the delay               |
| Can pass arguments | Yes, you can pass extra arguments               |
| Not exactly timed  | Delay is minimum, not guaranteed                |

---

## 🧪 Example with Arguments

```javascript
function greet(name) {
  console.log("Hello, " + name);
}

setTimeout(greet, 1500, "Alice"); // Runs after 1.5 seconds
```

---

### Callback Function with SetTimeout and  passing args
```js
// Callback Function Example
function greet(name, myFunction) {
    console.log('Hello world');
    // callback function
    // executed only after the greet() is executed
    myFunction(name);
}
// callback function
function sayName(name) {
    console.log('Hello' + ' ' + name);
}
// calling the function after 2 seconds
setTimeout(greet, 2000, 'John', sayName);
```
