# 04 - Asynchronous Programming

> Learn how JavaScript handles time, network calls, and other tasks that happen later.

- [Start Exercises](./Exercises.md)
- [Previous Module: ES6+ Modern JavaScript](../03-es6-plus/README.md)
- [JavaScript Track Overview](../README.md)

---

## 🎯 What You Will Learn

- How asynchronous code works in JavaScript
- How callbacks work and why they can be tricky
- How Promises provide cleaner async code
- How `async` / `await` makes async code readable
- How to load data from APIs with `fetch`
- How to handle errors in async code

---

## ⏳ Synchronous vs Asynchronous

### Synchronous example

```js
console.log('First');
console.log('Second');
console.log('Third');
```

Output:

```
First
Second
Third
```

### Asynchronous example

```js
console.log('First');
setTimeout(() => {
  console.log('Second');
}, 1000);
console.log('Third');
```

Output:

```
First
Third
Second
```

### Async timeline

```
Start → first log → timer starts → next code runs → timer finishes → callback runs
```

---

## 🔁 Callbacks

A callback is a function passed into another function.

```js
function greet(name, callback) {
  callback(`Hello, ${name}`);
}

greet('Ava', message => {
  console.log(message);
});
```

### Callback problem

Callbacks can get hard to read when nested:

```js
doStep1(() => {
  doStep2(() => {
    doStep3(() => {
      console.log('done');
    });
  });
});
```

This is often called "callback hell" because it becomes difficult to understand.

---

## 💡 Promises

### Promise states

A Promise has three states:
- `pending` — waiting for result
- `fulfilled` — completed successfully
- `rejected` — failed with an error

```
Promise pending -> fulfilled or rejected
```

A Promise is a value that will arrive later.

```js
const promise = new Promise((resolve, reject) => {
  const success = true;
  if (success) {
    resolve('Done');
  } else {
    reject('Error');
  }
});

promise
  .then(result => console.log(result))
  .catch(error => console.error(error));
```

---

## 🚀 `async` / `await`

Use `await` to wait for a Promise nicely.

```js
async function loadData() {
  const response = await fetch('https://api.example.com/data');
  const data = await response.json();
  console.log(data);
}

loadData();
```

---

## 🌐 Fetch API

```js
fetch('https://jsonplaceholder.typicode.com/posts/1')
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error('Error:', error));
```

---

## ✅ Error Handling

### Promise catch

```js
fetch('https://api.example.com/data')
  .then(response => response.json())
  .catch(error => console.error(error));
```

### Try / catch with async

```js
async function loadData() {
  try {
    const response = await fetch('https://api.example.com/data');
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error('Error loading data:', error);
  }
}
```

---

## 🚀 Next

After this module, move to [Module 05: Advanced JavaScript](../05-advanced-js/README.md) to learn debugging, browser storage, timers, and better application structure.

Once you finish the advanced module, use JavaScript with HTML/CSS to build real app projects.
