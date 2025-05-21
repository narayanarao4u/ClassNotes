Sure! Here's a short explanation of setInterval() with 3 examples in increasing difficulty:

---

## ⏰ What is setInterval()?

setInterval() repeatedly runs a function after a fixed time interval (in milliseconds).

### Syntax:

```javascript
setInterval(function, intervalInMilliseconds);
```

---

## 🟢 Easy Example: Print "Hello" every 1 second

```javascript
setInterval(() => {
  console.log("Hello");
}, 1000);
```

This prints "Hello" every second (forever).

---

## 🟡 Medium Example: Show current time every second

```javascript
setInterval(() => {
  const now = new Date();
  console.log(now.toLocaleTimeString());
}, 1000);
```

Prints the current time (like a clock).

---

## 🔴 Hard Example: Countdown from 5 to 1, then stop

```javascript
let count = 5;

const timerId = setInterval(() => {
  console.log(count);
  count--;

  if (count === 0) {
    clearInterval(timerId);
    console.log("Countdown finished!");
  }
}, 1000);
```

This prints:

```
5  
4  
3  
2  
1  
Countdown finished!
```

---

