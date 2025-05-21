Absolutely! Let's explore both `BigInt` and `Symbol` in JavaScript with clear explanations and 5 examples each.

---

## 🔢 BigInt in JavaScript

`BigInt` is a special numeric type introduced in ES2020 that can represent **integers larger than `Number.MAX_SAFE_INTEGER`** (which is 2⁵³ - 1).

### ✅ How to create a BigInt:

* Add `n` at the end of a number
* Or use the `BigInt()` constructor

### 🔗 5 Examples of BigInt:

1. **Declaring a BigInt**

```javascript
let big = 1234567890123456789012345678901234567890n;
console.log(big);
```

2. **Using BigInt constructor**

```javascript
let big = BigInt("987654321987654321987654321");
console.log(big);
```

3. **Arithmetic with BigInt**

```javascript
let a = 10000000000000000000n;
let b = 20000000000000000000n;
console.log(a + b); // 30000000000000000000n
```

4. **Comparing BigInt with Number**

```javascript
let num = 42;
let big = 42n;

console.log(big == num);  // true (loose equality)
console.log(big === num); // false (strict equality)
```

5. **Using BigInt in a loop**

```javascript
for (let i = 1n; i <= 5n; i++) {
  console.log(i); // 1n, 2n, 3n, 4n, 5n
}
```

🔴 Note: BigInt cannot be mixed directly with Number types in math operations (e.g., `BigInt + Number` throws an error).

---

## 🧿 Symbol in JavaScript

`Symbol` is a **unique and immutable** primitive value, often used as **object property keys** to avoid name collisions.

### ✅ How to create a Symbol:

* `Symbol("description")`

### 🔗 5 Examples of Symbol:

1. **Creating Symbols**

```javascript
let sym1 = Symbol("id");
let sym2 = Symbol("id");

console.log(sym1 === sym2); // false — each Symbol is unique
```

2. **Using Symbol as object key**

```javascript
let id = Symbol("userID");
let user = {
  name: "Alice",
  [id]: 123
};

console.log(user[id]); // 123
```

3. **Hiding properties using Symbol**

```javascript
let secret = Symbol("secret");
let obj = {
  [secret]: "hidden value",
  visible: "shown"
};

console.log(obj.visible);       // "shown"
console.log(obj[secret]);       // "hidden value"
```

4. **Symbols are not listed in `for...in` or `Object.keys()`**

```javascript
let id = Symbol("id");
let person = {
  name: "Bob",
  [id]: 999
};

for (let key in person) {
  console.log(key); // Only "name", not Symbol key
}

console.log(Object.keys(person)); // ["name"]
```

5. **Using `Symbol.for()` for shared symbols**

```javascript
let globalSym1 = Symbol.for("globalID");
let globalSym2 = Symbol.for("globalID");

console.log(globalSym1 === globalSym2); // true — same global symbol
```

---


