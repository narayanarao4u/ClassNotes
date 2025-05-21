
----
## function Arguments
* arguments is a built-in object available inside all regular functions (not arrow functions).

* It holds all the arguments passed to the function — even if they’re not listed as parameters.

* It's array-like (you can use .length, index values, and loop through it), but it is not a real array.
* Inside a function, you can access an object called arguments 
```js
function add() {
    let sum = 0;
    for (let i = 0; i < arguments.length; i++) {
        sum += arguments[i];
    }
    return sum;
}

console.log(add(1, 2)); // 3
console.log(add(1, 2, 3, 4, 5)); // 15
```
## function Name
* sum is a reference to the add function.

* .name returns the original function name → ✅ "add"
```js
let sum = add;
console.log(sum.name) // add
```


### arguments.length
```js
function addNumber(n) {
  console.log('Number of arguments: ' + arguments.length);
  for (let i = 0; i < arguments.length; i++) {
    n += arguments[i];
  }
  return n;
}
console.log(addNumber(1, 2, 3));
console.log(addNumber(1, 2, 3, 4, 5));
```