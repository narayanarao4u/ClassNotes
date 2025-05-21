Here's a table of common **JavaScript Array methods** with examples and their **output**, clearly separated into columns:

| **Method**    | **Example Code**                                  | **Output**                    |
| ------------- | ------------------------------------------------- | ----------------------------- |
| `push()`      | `let a = [1, 2]; a.push(3);`                      | `[1, 2, 3]`                   |
| `pop()`       | `let a = [1, 2, 3]; a.pop();`                     | `[1, 2]`                      |
| `shift()`     | `let a = [1, 2, 3]; a.shift();`                   | `[2, 3]`                      |
| `unshift()`   | `let a = [2, 3]; a.unshift(1);`                   | `[1, 2, 3]`                   |
| `length`      | `let a = [1, 2, 3]; a.length;`                    | `3`                           |
| `indexOf()`   | `let a = ["a", "b", "c"]; a.indexOf("b");`        | `1`                           |
| `includes()`  | `let a = [1, 2, 3]; a.includes(2);`               | `true`                        |
| `slice()`     | `let a = [1, 2, 3, 4]; a.slice(1, 3);`            | `[2, 3]`                      |
| `splice()`    | `let a = [1, 2, 3]; a.splice(1, 1, 99);`          | `[1, 99, 3]`                  |
| `forEach()`   | `let a = [1, 2]; a.forEach(x => console.log(x));` | `1\n2` *(printed to console)* |
| `map()`       | `let a = [1, 2]; let b = a.map(x => x * 2);`      | `[2, 4]`                      |
| `filter()`    | `let a = [1, 2, 3]; a.filter(x => x > 1);`        | `[2, 3]`                      |
| `reduce()`    | `let a = [1, 2, 3]; a.reduce((x, y) => x + y);`   | `6`                           |
| `reverse()`   | `let a = [1, 2, 3]; a.reverse();`                 | `[3, 2, 1]`                   |
| `sort()`      | `let a = [3, 1, 2]; a.sort();`                    | `[1, 2, 3]`                   |
| `join()`      | `let a = [1, 2, 3]; a.join("-");`                 | `"1-2-3"`                     |
| `concat()`    | `let a = [1]; a.concat([2, 3]);`                  | `[1, 2, 3]`                   |
| `find()`      | `let a = [1, 2, 3]; a.find(x => x > 1);`          | `2`                           |
| `findIndex()` | `let a = [1, 2, 3]; a.findIndex(x => x > 1);`     | `1`                           |
| `every()`     | `let a = [1, 2, 3]; a.every(x => x > 0);`         | `true`                        |
| `some()`      | `let a = [1, 2, 3]; a.some(x => x > 2);`          | `true`                        |


-----

Sure! Here's a detailed explanation with **3 examples each** of the `slice()` and `splice()` methods in JavaScript, along with **code** and **expected output**.

---

## 🟦 `slice()` – Extracts a portion of an array **without changing** the original array.

### 🔹 Syntax:

```js
array.slice(start, end);
```

* `start`: starting index (inclusive)
* `end`: ending index (exclusive)

| **Example**                      | **Code**                                           | **Output**      |
| -------------------------------- | -------------------------------------------------- | --------------- |
| **1. Basic slice**               | `let a = [10, 20, 30, 40]; let b = a.slice(1, 3);` | `b = [20, 30]`  |
| **2. Slice from index to end**   | `let a = [1, 2, 3, 4, 5]; let b = a.slice(2);`     | `b = [3, 4, 5]` |
| **3. Slice with negative index** | `let a = [10, 20, 30, 40]; let b = a.slice(-2);`   | `b = [30, 40]`  |

🔸 *Original array is unchanged in all cases.*

---

## 🟨 `splice()` – **Changes** the original array by **adding/removing** elements.

### 🔹 Syntax:

```js
array.splice(start, deleteCount, item1, item2, ...)
```

* `start`: index to start changing
* `deleteCount`: number of elements to remove
* `item1, item2,...`: elements to add

| **Example**             | **Code**                                  | **Output**         |
| ----------------------- | ----------------------------------------- | ------------------ |
| **1. Remove elements**  | `let a = [1, 2, 3, 4]; a.splice(1, 2);`   | `a = [1, 4]`       |
| **2. Add elements**     | `let a = [1, 4]; a.splice(1, 0, 2, 3);`   | `a = [1, 2, 3, 4]` |
| **3. Replace elements** | `let a = [1, 2, 3]; a.splice(1, 1, "x");` | `a = [1, "x", 3]`  |

🔸 *Splice modifies the array directly.*

---

Would you like visual diagrams or animations for better understanding?


-----
Here's a clear explanation of the JavaScript array methods **`every()`** and **`some()`**, with syntax, usage, and examples.

---

## 🟩 `every()` Method

**Purpose:**
Checks if **all elements** in the array **pass a test** (return `true`).
✅ Returns `true` **only if all elements pass**.

### 🔹 Syntax:

```javascript
array.every(callback);
```

* `callback` is a function that returns `true` or `false` for each element.

### 🔹 Examples:

| **Example**        | **Code**                                              | **Output** |
| ------------------ | ----------------------------------------------------- | ---------- |
| ✅ All pass         | `let nums = [2, 4, 6]; nums.every(n => n % 2 === 0);` | `true`     |
| ❌ One fails        | `let nums = [2, 3, 6]; nums.every(n => n % 2 === 0);` | `false`    |
| All greater than 0 | `let a = [1, 2, 3]; a.every(x => x > 0);`             | `true`     |

---

## 🟨 `some()` Method

**Purpose:**
Checks if **at least one element** passes the test.
✅ Returns `true` if **any** element passes.

### 🔹 Syntax:

```javascript
array.some(callback);
```

* `callback` is a function that returns `true` or `false` for each element.

### 🔹 Examples:

| **Example**              | **Code**                                             | **Output** |
| ------------------------ | ---------------------------------------------------- | ---------- |
| ✅ One passes             | `let nums = [1, 3, 4]; nums.some(n => n % 2 === 0);` | `true`     |
| ❌ None pass              | `let nums = [1, 3, 5]; nums.some(n => n % 2 === 0);` | `false`    |
| Check if any is negative | `let a = [5, -1, 7]; a.some(x => x < 0);`            | `true`     |

---

### ✅ Summary:

| Method    | Returns `true` if...             | Changes array? |
| --------- | -------------------------------- | -------------- |
| `every()` | **All** elements pass the test   | ❌ No           |
| `some()`  | **At least one** passes the test | ❌ No           |

----

