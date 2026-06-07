# 02 - Flexbox

> Learn how to build flexible, responsive layouts using CSS Flexbox.

- [Start Exercises](./Exercises.md)
- [Previous Module: Fundamentals](../01-fundamentals/README.md)
- [Next Module: Grid](../03-grid/README.md)
- [CSS Track Overview](../README.md)

---

## 🎯 What You Will Learn

- What Flexbox is and when to use it
- The flex container and flex items
- Main axis and cross axis
- Alignment with `justify-content` and `align-items`
- Wrapping and responsive rows
- Common layout patterns with Flexbox

---

## 🧠 What is Flexbox?

Flexbox is a layout mode that makes it easy to align and distribute space among items in a container.

Use Flexbox when you want:

- horizontal or vertical alignment
- equal spacing between items
- centered content
- flexible item sizes

---

## 📦 Flex Container

Set a parent element to `display: flex`:

```css
.container {
    display: flex;
}
```

This makes all direct child elements become flex items.

### Basic example

```html
<div class="container">
    <div class="box">Box 1</div>
    <div class="box">Box 2</div>
    <div class="box">Box 3</div>
</div>
```

---

## 🧭 Main Axis and Cross Axis

- Main axis is the direction flex items flow in.
- Cross axis is perpendicular to the main axis.

By default:
- main axis = row (left to right)
- cross axis = column (top to bottom)

Use `flex-direction` to change it.

```css
.container {
    display: flex;
    flex-direction: column;
}
```

---

## 🔄 Direction and Wrapping

### `flex-direction`

- `row` — horizontal left-to-right
- `row-reverse` — horizontal right-to-left
- `column` — vertical top-to-bottom
- `column-reverse` — vertical bottom-to-top

### `flex-wrap`

- `nowrap` — all items stay on one line
- `wrap` — items wrap to the next line
- `wrap-reverse` — wrap in reverse direction

```css
.container {
    display: flex;
    flex-wrap: wrap;
}
```

---

## 🎯 Alignment

### `justify-content`

Controls alignment along the main axis:

- `flex-start`
- `center`
- `flex-end`
- `space-between`
- `space-around`
- `space-evenly`

### `align-items`

Controls alignment along the cross axis:

- `stretch`
- `flex-start`
- `center`
- `flex-end`
- `baseline`

```css
.container {
    display: flex;
    justify-content: center;
    align-items: center;
}
```

---

## 📏 Flex Item Properties

### `flex-grow`

Lets items grow to fill available space.

```css
.box {
    flex-grow: 1;
}
```

### `flex-shrink`

Lets items shrink when space is limited.

```css
.box {
    flex-shrink: 1;
}
```

### `flex-basis`

Sets the default size before growing or shrinking.

```css
.box {
    flex: 0 0 200px;
}
```

### `order`

Rearrange item order without changing HTML.

```css
.first {
    order: 2;
}

.second {
    order: 1;
}
```

---

## 🧩 Common Layout Patterns

### Center content horizontally and vertically

```css
.container {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 300px;
}
```

### Navigation menu

```css
nav {
    display: flex;
    gap: 16px;
}
```

### Responsive card row

```css
.cards {
    display: flex;
    flex-wrap: wrap;
    gap: 16px;
}
.card {
    flex: 1 1 240px;
}
```

---

## ✅ Flexbox Tips

- Use `gap` instead of margins for consistent spacing
- Use `flex: 1` for equal-width items
- Use `flex-wrap` to make rows responsive
- Combine `align-items` and `justify-content` for centering

---

## 🚀 Continue to Grid

When you are comfortable with Flexbox, move to [Module 3: CSS Grid](../03-grid/README.md).
