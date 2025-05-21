## Recursive function
```js
function sumofNaturalNumbers(n) {
  if (n === 0) return 0;
  return n + sumofNaturalNumbers(n - 1);
}
```

### example 2 
```js
function factorial(n) {
  if (n === 0) return 1;
  return n * factorial(n - 1);

// return n === 0 ? 1 : n * factorial(n - 1);
  
}
console.log(sumofNaturalNumbers(5));
console.log(factorial(5));
```



---

## 🔁 Example 3 Recursive Function to Reverse a String

Let’s write a function that reverses a string using recursion.

### ✅ Code:

```javascript
function reverseString(str) {
  if (str === "") {
    return "";
  } else {
    return reverseString(str.slice(1)) + str[0];
  }
}

console.log(reverseString("hello")); // "olleh"
```

---

### 🔍 How It Works:

* The function takes the first character (`str[0]`) and puts it at the **end**.
* Then it **recursively** calls itself with the rest of the string (`str.slice(1)`).
* The base case is when the string is empty (`""`).

---

### 📦 Step-by-Step:

```text
reverseString("hello")
= reverseString("ello") + "h"
= reverseString("llo") + "e" + "h"
= reverseString("lo") + "l" + "e" + "h"
= reverseString("o") + "l" + "l" + "e" + "h"
= reverseString("") + "o" + "l" + "l" + "e" + "h"
= "" + "o" + "l" + "l" + "e" + "h"
= "olleh"
```

---

Certainly! Here's a classic example of a recursive function to calculate the Fibonacci number without using loops.

---

## 🔁 Fibonacci Series using Recursion (No Loops)

### 🔢 What is Fibonacci?

The Fibonacci series is:

```
0, 1, 1, 2, 3, 5, 8, 13, 21, ...
```

Each number is the sum of the two previous numbers:

* F(0) = 0
* F(1) = 1
* F(n) = F(n-1) + F(n-2) for n ≥ 2

---

## ✅ Recursive JavaScript Function:

```javascript
function fibonacci(n) {
  if (n === 0) return 0;
  if (n === 1) return 1;
  return fibonacci(n - 1) + fibonacci(n - 2);
}
```

---

### 🧪 Example Calls:

```javascript
console.log(fibonacci(0)); // 0
console.log(fibonacci(1)); // 1
console.log(fibonacci(5)); // 5
console.log(fibonacci(8)); // 21
```

---

### 📌 How It Works:

Let’s trace `fibonacci(5)`:

```
fibonacci(5)
= fibonacci(4) + fibonacci(3)
= (fibonacci(3) + fibonacci(2)) + (fibonacci(2) + fibonacci(1))
= ...
```

It keeps calling itself until it reaches the base cases: `fibonacci(1)` and `fibonacci(0)`.

---


