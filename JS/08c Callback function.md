## 🔁 What is a Callback Function?

A **callback function** is:

> A function passed as an argument to another function, and it is called (or “called back”) later inside that function.

✅ In simple words:

> You give a function to another function — and it decides when to run it.

---

## 🧠 Why Use Callbacks?

* To control the **order of execution**
* To **run code after something else finishes** (like a delay or a task)
* To make your code **more flexible and reusable**

---

```js
//Callback Function

function greet(name, callback) {
    console.log('Hi' + ' ' + name);
    callback();
}
// callback function
function callMe() {
    console.log('Call me ....');
}

// callback function
function sayGoodBye(name="") {
    console.log(`Good Bye .... ${name}`);
}
// passing function as an argument
greet('Peter', callMe);
greet('Peter', sayGoodBye);
```

### Example 2
```js
  function cmToIn(length) {
    return length / 2.54;
  }
  
  function inToCm(length) {
    return length * 2.54;
  }
  
  function convert(fn, length) {
    return fn(length);
  }
  
  let inches = convert(cmToIn, 10);
  console.log(inches);
  
  let cm = convert(inToCm, 10);
  console.log(cm);
```