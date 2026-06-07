# 05 - Advanced JavaScript

> Build smarter web applications with advanced JavaScript patterns, browser APIs, and debugging skills.

- [Start Exercises](./Exercises.md)
- [Previous Module: Asynchronous Programming](../04-asynchronous/README.md)
- [JavaScript Track Overview](../README.md)

---

## 🎯 What You Will Learn

- How to debug JavaScript using the browser console
- How to handle errors and write safer code
- How to use browser storage with `localStorage`
- How to organize code with functions and modules
- How to use built-in browser APIs for dates, timers, and validation
- How to plan and build larger JavaScript features

---

## 🧠 Debugging JavaScript

When code does not work, use the browser console.

### Common tools

- `console.log()` — print values
- `console.error()` — show errors
- `debugger` — pause execution

Example:

```js
const name = 'Mia';
console.log('Current name:', name);

if (!name) {
  console.error('Name is missing');
}
```

### Debugging flow

```
Code runs → browser console logs values → find issue → fix code → refresh page
```

---

## 🧩 Error Handling

Use `try` / `catch` to recover from problems.

```js
try {
  const data = JSON.parse('invalid');
  console.log(data);
} catch (error) {
  console.error('Parsing failed:', error.message);
}
```

Use `throw` when your code detects something wrong:

```js
function divide(a, b) {
  if (b === 0) {
    throw new Error('Cannot divide by zero');
  }
  return a / b;
}
```

---

## 💾 Browser Storage: `localStorage`

Use `localStorage` to save data in the browser between refreshes.

```js
localStorage.setItem('username', 'Ava');
const storedName = localStorage.getItem('username');
console.log(storedName); // Ava
```

Remove or clear storage:

```js
localStorage.removeItem('username');
localStorage.clear();
```

---

## 🧱 Structuring Larger JavaScript

### Organize code by responsibility

- Data logic: store and update values
- UI logic: update the page
- Event logic: handle clicks and input

### Example pattern

```js
function getItems() { ... }
function renderItems(items) { ... }
function handleAddItem(event) { ... }
```

### Simple module concept

```js
// utils.js
export function formatName(name) {
  return name.trim().toUpperCase();
}

// app.js
import { formatName } from './utils.js';
console.log(formatName('Ava'));
```

---

## ⏳ Browser APIs and Timers

### `setTimeout`

Run code after a delay:

```js
setTimeout(() => {
  console.log('Run later');
}, 1000);
```

### `setInterval`

Run code repeatedly:

```js
const timer = setInterval(() => {
  console.log('Tick');
}, 1000);

clearInterval(timer);
```

---

## 📆 Date and Time

```js
const now = new Date();
console.log(now.toLocaleString());
```

Format a date:

```js
const birthday = new Date('2000-01-01');
console.log(birthday.toDateString());
```

---

## 🧠 Advanced Tips for Beginners

- Write small functions with one purpose
- Keep names simple and meaningful
- Test each change in the browser
- Use comments to explain hard logic
- Read errors carefully and search them if needed

---

## 🚀 Build Better Apps

This module helps you move from small examples to real features. After finishing, use the project guides to build apps with JavaScript, HTML, and CSS.
