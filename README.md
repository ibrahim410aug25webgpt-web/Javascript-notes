# JavaScript Notes

A complete guide from **Basics to Advanced** 🚀

---

## 📑 Table of Contents

1. Introduction
2. Basics

   * Variables (`var`, `let`, `const`)
   * Data Types (Primitive & Non-Primitive)
   * Operators
   * Conditionals (`if`, `else`, `switch`)
   * Loops (`for`, `while`, `do-while`, `for..in`, `for..of`)
3. Functions

   * Normal Functions
   * Arrow Functions
   * Parameters & Arguments
   * Default Parameters
   * Return Statement
   * Callback Functions
   * IIFE (Immediately Invoked Function Expressions)
4. Scope & Hoisting

   * Global & Local Scope
   * Block Scope
   * Function Scope
   * Hoisting
   * Temporal Dead Zone (TDZ)
5. Objects & Arrays

   * Object Literals
   * Accessing & Modifying Properties
   * Array Methods (`map`, `filter`, `forEach`, `reduce`)
   * Spread & Rest Operator
   * Destructuring
   * Shallow vs Deep Copy
6. Strings

   * String Methods (`charAt`, `indexOf`, `slice`, `substring`, `replace`, `split`, `includes`)
7. ES6+ Features

   * Template Literals
   * Modules (`import` / `export`)
   * Classes & Inheritance
   * Promises
   * Async/Await
8. Advanced Concepts

   * Closures
   * Higher-Order Functions
   * Event Loop
   * `this` keyword
   * Bind, Call, Apply
   * Prototypes & Inheritance
   * Error Handling (`try`, `catch`, `finally`)
9. DOM Manipulation

   * Selecting Elements (`getElementById`, `querySelector`)
   * Events (`addEventListener`)
   * Creating & Removing Elements
   * Modifying Styles & Attributes
10. Asynchronous JavaScript

    * setTimeout & setInterval
    * Callbacks
    * Promises
    * Async/Await
    * Fetch API & AJAX
11. Extra Topics

    * Regular Expressions (Regex)
    * Local Storage & Session Storage
    * JSON (Parse & Stringify)
    * Modules & Bundlers (Webpack, Vite)
    * Best Practices

---

## 1. Introduction

JavaScript is a **high-level, interpreted programming language** used mainly for **web development**.

```js
console.log("Hello, JavaScript!");
```

---

## 2. Basics

### Variables

```js
var a = 10; // Function-scoped
let b = 20; // Block-scoped
const c = 30; // Constant value
```

### Data Types

* Primitive: `string`, `number`, `boolean`, `null`, `undefined`, `symbol`, `bigint`
* Non-Primitive: `object`, `array`, `function`

### Operators

```js
let x = 5;
let y = 2;
console.log(x + y); // 7
console.log(x ** y); // 25 (Exponentiation)
```

### Conditionals

```js
if (x > y) {
  console.log("x is greater");
} else {
  console.log("y is greater");
}
```

### Loops

```js
for (let i = 0; i < 5; i++) {
  console.log(i);
}
```

---

## 3. Functions

### Normal Function

```js
function add(a, b) {
  return a + b;
}
```

### Arrow Function

```js
const add = (a, b) => a + b;
```

### Callback Function

```js
function greet(name, callback) {
  console.log("Hello, " + name);
  callback();
}

greet("Ali", () => console.log("How are you?"));
```

### IIFE

```js
(function(){
  console.log("IIFE executed!");
})();
```

---

## 4. Scope & Hoisting

### Example:

```js
console.log(a); // undefined (hoisted)
var a = 10;
```

---

## 5. Objects & Arrays

```js
let person = { name: "Ali", age: 25 };
console.log(person.name);

let arr = [1, 2, 3];
arr.push(4);
console.log(arr);
```

Array Methods:

```js
let nums = [1, 2, 3, 4];
let doubled = nums.map(n => n * 2);
```

---

## 6. Strings

```js
let str = "JavaScript";
console.log(str.includes("Java"));
```

---

## 7. ES6+ Features

### Template Literals

```js
let name = "Ali";
console.log(`Hello, ${name}!`);
```

### Classes

```js
class Person {
  constructor(name) {
    this.name = name;
  }
  greet() {
    console.log(`Hello, I am ${this.name}`);
  }
}

let p = new Person("Ali");
p.greet();
```

---

## 8. Advanced Concepts

### Closures

```js
function outer() {
  let count = 0;
  return function inner() {
    count++;
    return count;
  };
}

let counter = outer();
console.log(counter()); // 1
console.log(counter()); // 2
```

---

## 9. DOM Manipulation

```js
let btn = document.querySelector("button");
btn.addEventListener("click", () => alert("Button clicked!"));
```

---

## 10. Asynchronous JavaScript

### Promise

```js
let promise = new Promise((resolve, reject) => {
  setTimeout(() => resolve("Done!"), 2000);
});

promise.then(result => console.log(result));
```

### Async/Await

```js
async function fetchData() {
  let response = await fetch("https://jsonplaceholder.typicode.com/posts/1");
  let data = await response.json();
  console.log(data);
}
fetchData();
```

---

## 11. Extra Topics

### Local Storage

```js
localStorage.setItem("key", "value");
console.log(localStorage.getItem("key"));
```

### JSON

```js
let obj = { name: "Ali" };
let json = JSON.stringify(obj);
console.log(json);
```

---

## ✅ Conclusion

Ye notes JavaScript ke **basic se advance** tak ka overview dete hain. Ab tum ise apne GitHub par `README.md` file ke taur par upload kar sakte ho. 🚀
