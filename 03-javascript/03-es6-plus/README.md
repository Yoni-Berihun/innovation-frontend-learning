# 03 - ES6+ Modern JavaScript

> Learn the modern JavaScript features used in today's web applications.

- [Start Exercises](./Exercises.md)
- [Previous Module: DOM Manipulation](../02-dom-manipulation/README.md)
- [Next Module: Asynchronous Programming](../04-asynchronous/README.md)
- [JavaScript Track Overview](../README.md)

---

## 🎯 What You Will Learn

- `let` and `const` for safer variables
- Template strings for easier text
- Arrow functions for shorter code
- Object and array destructuring
- Spread and rest syntax
- Classes and modules
- Useful modern array methods

---

## 🌟 Modern JavaScript Syntax

### Why ES6+ matters

Modern JavaScript makes code easier to read and less error-prone.

```
Old JS -> longer and harder to maintain
Modern JS -> cleaner, shorter, and faster to write
```

### `let` and `const`

Use `const` when the variable does not change. Use `let` when it does.

```js
const name = 'Alex';
let score = 0;
score += 1;
```

---

## 📝 Template Literals

Use backticks for strings with variables.

```js
const firstName = 'Ava';
const message = `Hello, ${firstName}!`;
```

---

## 🧠 Arrow Functions

Standard function:

```js
function add(a, b) {
  return a + b;
}
```

Arrow function:

```js
const add = (a, b) => a + b;
```

---

## 📦 Destructuring

### Object destructuring

```js
const user = { name: 'Mia', age: 24 };
const { name, age } = user;
```

### Array destructuring

```js
const numbers = [10, 20, 30];
const [first, second] = numbers;
```

---

## 🔁 Spread and Rest

### Spread

```js
const colors = ['red', 'blue'];
const moreColors = [...colors, 'green'];
```

### Rest

```js
function sum(...values) {
  return values.reduce((total, value) => total + value, 0);
}
```

---

## 🧩 Array Methods

- `map()` — transform each item
- `filter()` — keep matching items
- `find()` — find one item
- `reduce()` — build one result from all items

Example:

```js
const numbers = [1, 2, 3];
const doubled = numbers.map(n => n * 2);
```

---

## 🧱 Classes

Create reusable blueprints.

```js
class Person {
  constructor(name) {
    this.name = name;
  }

  greet() {
    return `Hello, ${this.name}`;
  }
}

const user = new Person('Liam');
console.log(user.greet());
```

---

## 🗂 Modules

Use `export` and `import` to split code.

```js
// math.js
export function add(a, b) {
  return a + b;
}

// app.js
import { add } from './math.js';
console.log(add(2, 3));
```

---

## ✅ Modern JavaScript Tips

- Prefer `const` when possible
- Use arrow functions for short callbacks
- Use template strings for readable text
- Choose `map`, `filter`, and `reduce` for array work

---

## 🚀 Next

After this module, move to [Asynchronous Programming](../04-asynchronous/README.md).
