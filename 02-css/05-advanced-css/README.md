# 05 - Advanced CSS

> Master modern CSS features, transitions, animations, and advanced styling patterns.

- [Start Exercises](./Exercises.md)
- [Previous Module: Responsive Design](../04-responsive-design/README.md)
- [CSS Track Overview](../README.md)

---

## 🎯 What You Will Learn

- CSS custom properties (variables)
- Transitions and animations
- Transforms and hover effects
- Pseudo-classes and pseudo-elements
- Advanced selectors and specificity
- CSS functions: `calc()`, `clamp()`, `min()`, `max()`
- Dark mode and theming
- Performance-friendly CSS

---

## 🧠 CSS Custom Properties

Create reusable variables with `--`.

```css
:root {
    --primary-color: #2563eb;
    --bg-color: #f8fbff;
    --text-color: #1f2937;
    --card-radius: 16px;
}

body {
    background-color: var(--bg-color);
    color: var(--text-color);
}

.button {
    background-color: var(--primary-color);
    border-radius: var(--card-radius);
}
```

---

## 🔁 Transitions and Transforms

### Transitions

Smoothly animate property changes.

```css
.button {
    transition: background-color 0.3s ease, transform 0.3s ease;
}

.button:hover {
    background-color: #1d4ed8;
    transform: translateY(-2px);
}
```

### Transforms

Move, scale, rotate, or skew.

```css
.card {
    transform: scale(1.02);
}

.card:hover {
    transform: translateY(-10px);
}
```

---

## 🎬 Animations

Create custom keyframe animations.

```css
@keyframes fadeIn {
    from {
        opacity: 0;
        transform: translateY(16px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.card {
    animation: fadeIn 0.8s ease forwards;
}
```

---

## 🌿 Pseudo-classes and Pseudo-elements

### Common pseudo-classes

- `:hover`
- `:focus`
- `:active`
- `:nth-child()`
- `:first-child`

Example:

```css
button:hover {
    background-color: #1e40af;
}

.menu li:nth-child(odd) {
    background-color: #eff6ff;
}
```

### Pseudo-elements

- `::before`
- `::after`
- `::placeholder`

Example:

```css
.card::before {
    content: "";
    position: absolute;
    inset: 0;
    background: rgba(59, 130, 246, 0.08);
}
```

---

## 🧠 Advanced Selectors

### Attribute selectors

```css
input[type="email"] {
    border-color: blue;
}
```

### Grouping selectors

```css
h1,
h2,
h3 {
    margin-bottom: 0.75rem;
}
```

### Descendant vs child selectors

```css
nav a { }      /* descendant */
nav > a { }    /* direct child */
```

---

## 📏 CSS Functions

### `calc()`

```css
.container {
    width: calc(100% - 40px);
}
```

### `clamp()`

```css
h1 {
    font-size: clamp(2rem, 4vw, 3.5rem);
}
```

### `min()` and `max()`

```css
.section {
    padding: min(5vw, 40px);
}
```

---

## 🌙 Dark Mode and Theming

Use a media query or CSS class.

```css
@media (prefers-color-scheme: dark) {
    body {
        background-color: #111827;
        color: #f9fafb;
    }
}
```

Use variables for fast theme switching:

```css
:root {
    --bg: #ffffff;
    --text: #111827;
}

body.dark-mode {
    --bg: #111827;
    --text: #f9fafb;
}

body {
    background: var(--bg);
    color: var(--text);
}
```

---

## 🧠 CSS Architecture Tips

- Keep styles modular and reusable
- Use class names rather than tag selectors for layout
- Group related rules together
- Use variables for repeated values
- Keep specificity low and simple

---

## 🚀 Next Steps

After advanced CSS, practice by building project layouts in the `projects/` folder.
