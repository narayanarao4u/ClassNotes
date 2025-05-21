Certainly! Below are the complete solutions for the interactive student exercises on setTimeout().

---

# ✅ Solutions for setTimeout() Exercises

---

## 🔧 Task 1: Basic Timeout

Print "Learning JavaScript..." after 2 seconds.

```javascript
setTimeout(() => {
  console.log("Learning JavaScript...");
}, 2000);
```

---

## 🔧 Task 2: Greet After Delay

Call greet(name) after 3 seconds.

```javascript
function greet(name) {
  console.log("Hello, " + name);
}

setTimeout(greet, 3000, "Alice");
```

Or using an arrow function:

```javascript
setTimeout(() => greet("Alice"), 3000);
```

---

## 🔄 Task 3: Multiple Timed Messages

```javascript
setTimeout(() => {
  console.log("First message");
}, 1000);

setTimeout(() => {
  console.log("Second message");
}, 2000);

setTimeout(() => {
  console.log("Third message");
}, 3000);
```

---

## 🧠 Challenge 1: Countdown Timer (No loops)

```javascript
setTimeout(() => console.log(5), 1000);
setTimeout(() => console.log(4), 2000);
setTimeout(() => console.log(3), 3000);
setTimeout(() => console.log(2), 4000);
setTimeout(() => console.log(1), 5000);
```

Or with a loop (optional enhancement):

```javascript
for (let i = 5; i > 0; i--) {
  setTimeout(() => {
    console.log(i);
  }, (6 - i) * 1000);
}
```

---

## 🧠 Challenge 2: Cancel a Timeout

```javascript
let timerId = setTimeout(() => {
  console.log("Too late!");
}, 5000);

setTimeout(() => {
  clearTimeout(timerId);
  console.log("Timeout cancelled.");
}, 2000);
```

---

## ✅ Bonus: Delayed Button Alert

```html
<button onclick="delayedGreet()">Click me</button>

<script>
  function delayedGreet() {
    setTimeout(() => {
      alert("Hello after 2 seconds!");
    }, 2000);
  }
</script>
```

---

## 📝 Reflection Questions – Suggested Answers

1. ❓ What happens if you set the delay to 0 milliseconds?
   ✅ The code runs "as soon as possible" but still after the current call stack is finished — it's still asynchronous.

2. ❓ Can you use setTimeout with arrow functions?
   ✅ Yes. Arrow functions are commonly used with setTimeout for short, anonymous functions.

3. ❓ How can you cancel a scheduled timeout?
   ✅ Use clearTimeout(timerId) where timerId is the return value from setTimeout.
----