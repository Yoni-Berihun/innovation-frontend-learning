# 01 - JavaScript Basics

> Learn the foundation of JavaScript in a clear, beginner-friendly way.

- [Start Exercises](./Exercises.md)
- [Next Module: DOM Manipulation](../02-dom-manipulation/README.md)
- [JavaScript Track Overview](../README.md)

---

## 🎯 What You Will Learn

- What JavaScript is and how it works with HTML
- How to use variables, values, and data types
- How to write expressions and use operators
- How to make decisions with `if`, `else`, and `switch`
- How to repeat code with loops
- How functions work and why they matter
- How scope, arrays, and objects work

---

## 🌱 What is JavaScript?

JavaScript is the language that makes web pages interactive.

- HTML creates structure
- CSS adds style
- JavaScript adds behavior and logic

Example: make a button change text when clicked.

---

## 🧩 JavaScript in the Browser

A simple HTML page with JavaScript:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>JavaScript Basics</title>
</head>
<body>
  <h1 id="title">Hello!</h1>
  <button id="changeBtn">Change text</button>

  <script>
    const button = document.getElementById('changeBtn');
    button.addEventListener('click', function() {
      document.getElementById('title').textContent = 'JavaScript is working!';
    });
  </script>
</body>
</html>
```

---

## 🧠 How JavaScript Runs

JavaScript runs top to bottom in the browser, one line at a time.

```
HTML loads → JavaScript is read → browser runs code → page updates
```

### Comment example

Use comments to explain code:

```js
// This is a single-line comment
/* This is a
   multi-line comment */
```

---

## 🔤 Variables and Data Types

### Variables

```js
let name = 'Sara';
const age = 21;
```

### Data types

- `string` — text
- `number` — 123 or 3.14
- `boolean` — `true` or `false`
- `null` — empty value
- `undefined` — value not set
- `object` — grouped data

### Example

```js
let title = 'JavaScript Basics';
let isLoaded = true;
```

---

## ➕ Operators and Expressions

### Arithmetic

```js
let total = 5 + 3;
let product = 4 * 2;
```

### Comparison

```js
console.log(5 > 3); // true
console.log(4 === '4'); // false
```

### Logical

```js
let isReady = true && false;
```

---

## 🧠 Decisions: `if`, `else`, `switch`

### `if` example

```js
let score = 80;
if (score >= 90) {
  console.log('Great!');
} else {
  console.log('Keep practicing.');
}
```

### `switch` example

```js
let day = 'Monday';
switch (day) {
  case 'Monday':
    console.log('Start of week');
    break;
  case 'Friday':
    console.log('Weekend soon');
    break;
  default:
    console.log('Regular day');
}
```

---

## 🔁 Loops

### `for` loop

```js
for (let i = 1; i <= 5; i++) {
  console.log(i);
}
```

### `while` loop

```js
let count = 1;
while (count <= 5) {
  console.log(count);
  count++;
}
```

---

## 🧩 Functions

A function groups code to use again.

```js
function greet(name) {
  return `Hello, ${name}!`;
}

console.log(greet('Sara'));
```

### Function diagram

```
Input -> [ function ] -> Output
```

---

## 📦 Arrays and Objects

### Array

```js
const colors = ['red', 'blue', 'green'];
console.log(colors[0]);
```

### Object

```js
const user = {
  name: 'Mia',
  age: 24,
  active: true
};
console.log(user.name);
```

---

## ✅ Beginner Tips

- Keep code short and clear
- Name variables clearly
- Practice one concept at a time
- Use `console.log()` to see values
- Save and refresh your browser often

---

## 🚀 Next

After this module, move to [DOM Manipulation](../02-dom-manipulation/README.md).
