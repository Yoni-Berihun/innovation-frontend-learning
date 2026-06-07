# 01 - CSS Fundamentals

> Learn the building blocks of CSS and how to style HTML from the ground up.

- [Start Exercises](./Exercises.md)
- [Next Module: Flexbox](../02-flexbox/README.md)
- [CSS Track Overview](../README.md)

---

## 🎯 What You Will Learn

- What CSS is and why it matters
- How to link CSS to HTML
- CSS syntax: selectors, properties, and values
- The box model and element spacing
- Color, typography, and backgrounds
- Display modes and layout basics
- Best practices for clean CSS

---

## 🧠 What is CSS?

CSS stands for **Cascading Style Sheets**. It controls the visual appearance of HTML.

- HTML builds the structure of a page
- CSS makes that structure look good
- CSS controls color, size, spacing, layout, and typography

Think of HTML as the skeleton and CSS as the clothes, paint, and design.

---

## 🔗 Linking CSS to HTML

Create a file named `styles.css`, then add this inside your HTML `<head>`:

```html
<link rel="stylesheet" href="styles.css">
```

Example:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>My Styled Page</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <h1>Hello CSS</h1>
    <p>This page uses an external stylesheet.</p>
</body>
</html>
```

---

## 🎯 CSS Basics: Selectors, Properties, Values

A CSS rule has three parts:

```css
selector {
    property: value;
}
```

Example:

```css
h1 {
    color: darkblue;
    font-size: 2rem;
}
```

### Common selectors

- Element selector: `p { }`
- Class selector: `.card { }`
- ID selector: `#header { }`
- Descendant selector: `nav a { }`
- Attribute selector: `input[type="email"] { }`

---

## 📦 The Box Model

Every element is a box with four parts:

- `content` — the text or image
- `padding` — inside space around content
- `border` — the line around the padding
- `margin` — outside space between elements

```css
.box {
    margin: 20px;
    border: 2px solid #333;
    padding: 16px;
}
```

Use `box-sizing: border-box;` so padding and border are included in width.

```css
* {
    box-sizing: border-box;
}
```

---

## 🎨 Colors and Backgrounds

### Color values

- Named color: `red`
- Hex: `#1a73e8`
- RGB: `rgb(26, 115, 232)`
- HSL: `hsl(211, 82%, 53%)`

### Example:

```css
body {
    background-color: #f4f7fb;
    color: #1f1f1f;
}

h1 {
    color: #2a6ad9;
}
```

### Backgrounds

```css
body {
    background-color: #f8fafc;
    background-image: linear-gradient(180deg, #ffffff 0%, #e0f2fe 100%);
}
```

---

## 🔤 Typography

### Font settings

```css
body {
    font-family: Arial, sans-serif;
    font-size: 16px;
    line-height: 1.6;
}

h1 {
    font-size: 2.5rem;
}
```

### Text styling

```css
p {
    color: #333333;
}

a {
    color: #1256dd;
    text-decoration: none;
}

a:hover {
    text-decoration: underline;
}
```

---

## 🧩 Layout Basics: Display and Positioning

### `display` values

- `block` — fills the available width
- `inline` — flows inside text
- `inline-block` — inline with width/height support
- `none` — hides the element

Example:

```css
button {
    display: inline-block;
    padding: 12px 24px;
}
```

### `position`

- `static` — default
- `relative` — moves relative to original position
- `absolute` — positioned relative to the nearest positioned ancestor
- `fixed` — positioned relative to the viewport

```css
.box {
    position: relative;
    top: 10px;
}
```

---

## ✅ Best Practices for Beginners

- Keep your CSS organized
- Use classes for reusable styles
- Avoid inline styles when possible
- Use meaningful class names like `.card`, `.hero`, `.main-title`
- Comment sections in your CSS when needed

---

## 🚀 Ready to Continue?

Continue to [Module 2: Flexbox](../02-flexbox/README.md) once you have practiced these basics.
