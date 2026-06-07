# 🚀 Advanced React

> Learn how to organize and deploy React apps like a professional, with advanced patterns and real-world project structure.

- [Start Exercises](./Exercises.md)
- [Previous Module: Intermediate React](../03-intermediate/README.md)
- [React Track Overview](../README.md)

---

## 🎯 What You Will Learn

- Organize React apps with a clear folder structure
- Understand the `src/` and `public/` files
- Use build tools and deployment workflows
- Learn advanced component patterns
- Improve performance and code reuse
- Use React in real project workflows

---

## 🗂️ React Project Structure Explained

A React app commonly looks like this:

```
my-app/
├── node_modules/
├── public/
│   ├── index.html
│   └── favicon.ico
├── src/
│   ├── App.jsx
│   ├── index.jsx
│   ├── components/
│   ├── pages/
│   ├── styles/
│   └── assets/
├── package.json
├── vite.config.js
└── README.md
```

### What goes in `public/`?

- `index.html` → the page shell React loads into
- static files like icons and manifest
- files here are served as-is

### What goes in `src/`?

- `index.jsx` → app entry point
- `App.jsx` → root component
- `components/` → reusable UI pieces
- `pages/` → full screen or route-based pages
- `styles/` → CSS and styling files
- `assets/` → images, fonts, icons

---

## 🧩 Advanced Component Patterns

### Container / Presentational Pattern

- Container handles data and state
- Presentational component displays UI

```jsx
function UserList({ users }) {
  return (
    <ul>
      {users.map((user) => (
        <li key={user.id}>{user.name}</li>
      ))}
    </ul>
  );
}
```

### Custom Hooks

Create reusable logic with custom hooks.

```jsx
import { useState, useEffect } from "react";

function useFetch(url) {
  const [data, setData] = useState(null);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState(null);

  useEffect(() => {
    async function fetchData() {
      try {
        const response = await fetch(url);
        const json = await response.json();
        setData(json);
      } catch (err) {
        setError(err.message);
      } finally {
        setLoading(false);
      }
    }

    fetchData();
  }, [url]);

  return { data, loading, error };
}
```

---

## 🚀 Deployment Overview

### Build your app

```bash
npm run build
```

This creates a production-ready folder, usually `dist/` or `build/`.

### Common hosts

- Vercel
- Netlify
- GitHub Pages
- Surge

### Basic deployment steps

1. Build the app
2. Upload the output folder
3. Configure the host if needed
4. Visit the live URL

---

## 💡 Advanced Tips

- Keep components small and reusable
- Use folder names that describe features
- Avoid deeply nested props
- Use a `components/` folder for shared UI
- Use a `pages/` folder for full screens or routes

---

## 📚 Resources

- [React Folder Structure Guide](https://react.dev/learn)
- [Deploying Vite apps](https://vitejs.dev/guide/static-deploy.html)
- [React Best Practices](https://reactjs.org/docs/thinking-in-react.html)

---

## ✅ Checklist

- [ ] I understand React folder structure
- [ ] I can explain the difference between `public/` and `src/`
- [ ] I know how to build a React app for production
- [ ] I can use custom hooks for reusable logic
- [ ] I understand common deployment hosts
