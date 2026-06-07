# Exercises: Asynchronous Programming

> Practice async JavaScript patterns and working with remote data.

---

## 🟢 Easy Exercises

### Exercise 1.1: Use `setTimeout`
**Objective:** Practice asynchronous timing.

**Instructions:**
- Print `Start`.
- Use `setTimeout` to print `Done` after 2 seconds.
- Print `End` immediately after.

### Exercise 1.2: Build a Callback
**Objective:** Understand callback order.

**Instructions:**
- Create a function `delayMessage(message, callback)`.
- Use `setTimeout` inside to show the message after 1 second.
- Call `delayMessage` with a callback that prints `All done`.

---

## 🟡 Medium Exercises

### Exercise 2.1: Create a Promise
**Objective:** Build a Promise that resolves or rejects.

**Instructions:**
- Create a Promise that resolves after 1 second.
- Use `.then()` to print a success message.
- Add `.catch()` to handle errors.

### Exercise 2.2: Use `async` / `await`
**Objective:** Convert `.then()` to async/await.

**Instructions:**
- Create an async function `loadMessage`.
- Use `await` with a Promise that resolves to a text message.
- Print the message.

---

## 🔴 Challenging Exercises

### Exercise 3.1: Fetch API Data
**Objective:** Load data from a real API.

**Instructions:**
- Use `fetch('https://jsonplaceholder.typicode.com/posts/1')`.
- Convert the response to JSON.
- Print the title and body.
- Handle errors with `try/catch`.

### Exercise 3.2: Build a Data List
**Objective:** Show API data in HTML.

**Instructions:**
- Create a page with an empty list.
- Fetch posts from `https://jsonplaceholder.typicode.com/posts`.
- Add the first 5 post titles to the list.
- Show a loading message while the data loads.
