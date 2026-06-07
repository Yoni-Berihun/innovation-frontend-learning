# 03 - CSS Grid

> Build powerful page layouts with CSS Grid.

- [Start Exercises](./Exercises.md)
- [Previous Module: Flexbox](../02-flexbox/README.md)
- [Next Module: Responsive Design](../04-responsive-design/README.md)
- [CSS Track Overview](../README.md)

---

## 🎯 What You Will Learn

- What CSS Grid is and when to use it
- Grid container and grid items
- Columns, rows, and gaps
- Template areas and named lines
- Auto layout and responsive grids
- Combining Grid with Flexbox

---

## 🧠 What is CSS Grid?

CSS Grid is a two-dimensional layout system. It works by dividing a container into rows and columns and placing items into that grid.

Use Grid when you want:

- complex page layouts
- precise placement of items
- responsive grids that adapt automatically
- column and row control together

---

## 📦 Grid Container

Set a parent element to `display: grid`:

```css
.grid {
    display: grid;
}
```

### Example:

```css
.grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 16px;
}
```

---

## 📏 Columns and Rows

### `grid-template-columns`

Define columns:

```css
.grid {
    grid-template-columns: 200px 1fr 100px;
}
```

### `grid-template-rows`

Define rows:

```css
.grid {
    grid-template-rows: 100px auto 80px;
}
```

### `gap`

Add space between items:

```css
.grid {
    gap: 16px;
}
```

---

## 🎯 Grid Item Placement

### `grid-column`

```css
.item-a {
    grid-column: 1 / 3;
}
```

### `grid-row`

```css
.item-a {
    grid-row: 1 / 2;
}
```

### `grid-area`

Assign a named area:

```css
.grid {
    grid-template-areas:
        "header header"
        "sidebar main"
        "footer footer";
}

.header { grid-area: header; }
.sidebar { grid-area: sidebar; }
.main { grid-area: main; }
.footer { grid-area: footer; }
```

---

## 🧠 Auto Layout Helpers

### `repeat()`

```css
.grid {
    grid-template-columns: repeat(4, 1fr);
}
```

### `minmax()`

```css
.grid {
    grid-template-columns: repeat(3, minmax(200px, 1fr));
}
```

### `auto-fit` and `auto-fill`

```css
.grid {
    grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
}
```

---

## 📐 Responsive Grid Patterns

### Simple responsive cards

```css
.cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    gap: 24px;
}
```

### Dashboard layout

```css
.dashboard {
    display: grid;
    grid-template-columns: 1fr 2fr;
    gap: 24px;
}
```

---

## ✅ Grid Tips

- Use `grid-template-areas` for clear layout structure
- Use `minmax()` for flexible columns
- Use `auto-fit` for responsive grids
- Combine Grid for page layout and Flexbox for smaller item alignment

---

## 🚀 Continue to Responsive Design

When you are ready, move to [Module 4: Responsive Design](../04-responsive-design/README.md).
