# 02 - DOM Manipulation

> Learn how JavaScript controls web pages by changing HTML and responding to user actions.

- [Start Exercises](./Exercises.md)
- [Previous Module: Basics](../01-basics/README.md)
- [Next Module: ES6+ Modern JavaScript](../03-es6-plus/README.md)
- [JavaScript Track Overview](../README.md)

---

## 🎯 What You Will Learn

- How the DOM represents HTML in JavaScript
- How to find elements on a page
- How to change content and styles dynamically
- How to handle clicks and keyboard events
- How to build interactive UI using JavaScript

---

## 🌳 What is the DOM?

DOM means Document Object Model.

It is a tree structure that represents the page:

```
html
 ├── head
 └── body
      ├── h1
      ├── p
      └── button
```

JavaScript can walk this tree and change elements.

---

## 🔎 Selecting Elements

### `querySelector`

```js
const title = document.querySelector('h1');
```

### `getElementById`

```js
const button = document.getElementById('myButton');
```

### `querySelectorAll`

```js
const items = document.querySelectorAll('.item');
```

---

## ✏️ Updating HTML and Text

### Change text

```js
title.textContent = 'New title';
```

### Change HTML

```js
const box = document.querySelector('.box');
box.innerHTML = '<strong>Hello</strong>';
```

---

## 🎨 Change Styles

```js
title.style.color = 'crimson';
button.style.backgroundColor = '#4f46e5';
```

### Add or remove classes

```js
box.classList.add('active');
box.classList.remove('hidden');
box.classList.toggle('open');
```

---

## 🧠 Events

Events let JavaScript react to user actions.

```js
button.addEventListener('click', function() {
  alert('Button clicked!');
});
```

### Common events

- `click`
- `input`
- `submit`
- `keydown`
- `mouseover`

---

## 📦 Example: Simple Counter

```html
<button id="addBtn">Add</button>
<p id="count">0</p>
```

```js
let count = 0;
const countEl = document.getElementById('count');
const addBtn = document.getElementById('addBtn');
addBtn.addEventListener('click', () => {
  count += 1;
  countEl.textContent = count;
});
```

---

## ✅ DOM Tips

- Select elements once and reuse them
- Use classes to control styles from CSS
- Keep JavaScript separate from HTML when possible
- Use event listeners for interactive behavior

---

## 🚀 Next

After this module, move to [ES6+ Modern JavaScript](../03-es6-plus/README.md).
