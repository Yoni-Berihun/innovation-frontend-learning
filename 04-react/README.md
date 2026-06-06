# ⚛️ React Learning Track

> **Use the React learning guide content directly here.** This track is based on the existing `react-learning-guide` materials and preserves the same learning path, terminology, and practical examples.

## 🎯 What You'll Learn

- What React is and why it matters
- The component-based architecture
- JSX syntax and React project structure
- State, props, and event handling
- How React updates the DOM using the Virtual DOM
- Building dynamic, reusable UI components
- Setting up and running React projects
- Best practices for organizing React code

---

## 📚 Track Outline

### 01-fundamentals
- Intro to React
- React terminology and tools
- JSX basics
- First React component
- Creating a React environment

### 02-core-concepts
- React project structure
- Components, props, and state
- Handling user events
- Working with forms
- Writing reusable UI

### 03-intermediate
- Virtual DOM and rendering
- Dynamic UIs with state
- Practical examples and component architecture
- Working with multiple components

---

## 🧠 Why React?

React is a JavaScript library for building user interfaces. It helps you write cleaner code by breaking UI into reusable components and updating the page intelligently.

### Core React Advantages

- Component-based structure
- Declarative UI syntax
- Automatic DOM updates through the Virtual DOM
- Better maintainability for larger apps

---

## 📌 Key React Concepts

### Components
A React component is a reusable UI block.

Example:
```jsx
function App() {
  return <h1>Hello World</h1>;
}
```

### JSX
JSX looks like HTML inside JavaScript. It lets you write UI in a readable way.

Example:
```jsx
return (
  <div>
    <h1>Welcome</h1>
    <p>React makes UI easier.</p>
  </div>
);
```

### Props
Props are data passed into components.

Example:
```jsx
function Card({ title }) {
  return <h2>{title}</h2>;
}
```

### State
State is internal component data that changes over time.

Example:
```jsx
import { useState } from "react";

function Counter() {
  const [count, setCount] = useState(0);

  return (
    <button onClick={() => setCount(count + 1)}>
      Count: {count}
    </button>
  );
}
```

---

## 🌍 React Project Structure

A typical React app contains:

```
my-app/
├── node_modules/
├── public/
│   └── index.html
├── src/
│   ├── App.js
│   ├── index.js
│   └── components/
├── package.json
└── README.md
```

### Important Files

- `public/index.html` — the single HTML file that contains the React mount point
- `src/index.js` — starts the React application
- `src/App.js` — main component shell

---

## 🚀 Running React Locally

### Using Vite (recommended)

```bash
npm create vite@latest my-app
cd my-app
npm install
npm run dev
```

### Alternative with Create React App

```bash
npx create-react-app my-app
cd my-app
npm start
```

---

## ⚠️ React Best Practices

- Keep components small and focused
- Use `className` instead of `class`
- Wrap multiple JSX elements in a single parent
- Use `useState` for interactive data
- Keep logic and UI organized using reusable components

---

## 📘 Learning Approach

1. Start with the fundamentals section
2. Learn the React project structure
3. Build simple components first
4. Practice hooks and state
5. Use the intermediate section to deepen your understanding

---

## 📂 Recommended Structure for This Track

```
04-react/
├── 01-fundamentals/
├── 02-core-concepts/
├── 03-intermediate/
├── projects/
└── resources/
```
