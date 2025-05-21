Absolutely! Here's a fun and interactive student exercise set focused on practicing and understanding setTimeout() in JavaScript. It includes guided tasks, mini-challenges, and questions.

---

# 🧪 JavaScript setTimeout() – Interactive Student Exercises

### 👨‍🏫 Objective:

Help students understand how `setTimeout()` works and how to apply it in real-world code.

---

## 🔧 Task 1: Basic Timeout

📝 Instruction: Write code that prints "Learning JavaScript..." after 2 seconds.

✅ Starter:

```javascript
// Your code here
```

💡 Hint: Use setTimeout and an anonymous or arrow function.

---

## 🔧 Task 2: Greet After Delay

📝 Instruction: Create a function `greet(name)` that logs `Hello, <name>`.
Use `setTimeout` to call it after 3 seconds.

✅ Example:

```javascript
greet("Alice"); // Output after 3 sec: Hello, Alice
```

---

## 🔄 Task 3: Multiple Timed Messages

📝 Instruction: Display three messages with delays:

* "First message" after 1 second
* "Second message" after 2 seconds
* "Third message" after 3 seconds

✅ Example Output:

```
(After 1s): First message  
(After 2s): Second message  
(After 3s): Third message
```

---

## 🧠 Challenge 1: Countdown Timer

📝 Instruction: Create a countdown from 5 to 1 using `setTimeout()` (no loops yet).
Each number should print 1 second apart.

✅ Output:

```
5
4
3
2
1
```

💡 Hint: Use multiple setTimeout calls with increasing delays.

---

## 🧠 Challenge 2: Cancel a Timeout

📝 Instruction: Schedule a message for 5 seconds later, but cancel it after 2 seconds using `clearTimeout()`.

✅ Steps:

* Schedule `console.log("Too late!")` with setTimeout
* Use `setTimeout()` again to cancel it before it runs

---

## ✅ Bonus: Create a Simple Delayed Button

📝 HTML + JS Mini Task:

1. Create a button: “Click me”
2. When clicked, wait 2 seconds then show an alert: “Hello after 2 seconds!”

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

## 📝 Reflection Questions

1. What happens if you set the delay to 0 milliseconds?
2. Can you use setTimeout with arrow functions?
3. How can you cancel a scheduled timeout?


---

