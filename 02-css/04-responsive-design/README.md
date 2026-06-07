# 04 - Responsive Design

> Learn how to make websites look great on phones, tablets, and desktop screens.

- [Start Exercises](./Exercises.md)
- [Previous Module: Grid](../03-grid/README.md)
- [Next Module: Advanced CSS](../05-advanced-css/README.md)
- [CSS Track Overview](../README.md)

---

## 🎯 What You Will Learn

- The mobile-first approach
- Media queries and breakpoints
- Responsive typography and spacing
- Fluid layouts and flexible images
- Basic responsive patterns for real websites

---

## 📱 What is Responsive Design?

Responsive design means your website adapts to different screen sizes and devices.

A mobile-first workflow starts with styles for small screens and adds larger layouts as the screen grows.

---

## 🌍 Viewport and Meta Tag

Add this to your HTML `<head>`:

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

This tells the browser to size the page to the device width.

---

## 🧠 Media Queries

Media queries apply CSS only when the screen meets certain conditions.

Example:

```css
body {
    font-size: 16px;
}

@media (min-width: 768px) {
    body {
        font-size: 18px;
    }
}
```

### Common breakpoints

- `480px` — small phones
- `768px` — tablets
- `1024px` — small desktops
- `1200px+` — large screens

---

## 📐 Fluid Layouts

Use flexible widths to let content grow and shrink.

```css
.container {
    width: min(100%, 1200px);
    margin: 0 auto;
    padding: 0 16px;
}
```

### Responsive images

```css
img {
    max-width: 100%;
    height: auto;
}
```

---

## 🔧 Responsive Typography

Use relative units for text size.

```css
html {
    font-size: 100%; /* 16px */
}

body {
    font-size: 1rem;
}

h1 {
    font-size: clamp(2rem, 4vw, 3rem);
}
```

### `clamp()` example

```css
h1 {
    font-size: clamp(2rem, 5vw, 3.5rem);
}
```

---

## 🧩 Common Responsive Patterns

### Stacked cards on small screens

```css
.cards {
    display: grid;
    grid-template-columns: 1fr;
    gap: 16px;
}

@media (min-width: 768px) {
    .cards {
        grid-template-columns: repeat(2, 1fr);
    }
}
```

### Two-column layout turns single-column

```css
.section {
    display: grid;
    grid-template-columns: 1fr;
    gap: 24px;
}

@media (min-width: 900px) {
    .section {
        grid-template-columns: 1fr 1fr;
    }
}
```

---

## ✅ Accessibility and Usability

- Keep buttons and links large enough to tap
- Use readable font sizes on small screens
- Avoid using fixed widths
- Provide enough space between elements

---

## 🚀 Ready for Advanced CSS?

When you have a strong responsive workflow, move to [Module 5: Advanced CSS](../05-advanced-css/README.md).
