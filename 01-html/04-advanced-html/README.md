# 04-Advanced HTML: Structure, Media, Accessibility, and Best Practices

> Take your HTML skills further with advanced page structure, multimedia, accessibility, and SEO-friendly markup.

- [Start Exercises](./Exercises.md)
- [Previous Module: Forms & Validation](../03-forms-validation/README.md)
- [HTML Track Overview](../README.md)

This module bridges beginner-level HTML with practical real-world patterns. You'll learn how to build pages that are not only correct, but also usable, searchable, and ready for modern web development.

---

## 🎯 What You Will Learn

- Advanced HTML page structure and best practices
- HTML for responsive layouts and content sections
- Multimedia embedding with images, video, and audio
- Accessible HTML and ARIA basics
- SEO-friendly metadata and structured data
- Advanced form markup and usability patterns
- Clean, maintainable HTML for real websites

---

## 📚 Module Sections

1. [Advanced Page Structure](#advanced-page-structure)
2. [Multimedia and Embedded Content](#multimedia-and-embedded-content)
3. [Accessibility and Screen Reader Support](#accessibility-and-screen-reader-support)
4. [Metadata, SEO, and Structured Data](#metadata-seo-and-structured-data)
5. [Advanced Form Patterns](#advanced-form-patterns)
6. [Best Practices, Performance, and Validation](#best-practices-performance-and-validation)

---

## 🔧 Advanced Page Structure

Use HTML to organize content clearly, not just visually. This helps readers, browsers, search engines, and assistive technology.

### Common layout pattern

```html
<header>
    <nav>...</nav>
</header>

<main>
    <section>
        <h1>Page Title</h1>
        <p>Intro paragraph...</p>
    </section>

    <section>
        <h2>Features</h2>
        <article>...</article>
        <article>...</article>
    </section>
</main>

<aside>
    <h2>Quick Links</h2>
    <ul>...</ul>
</aside>

<footer>...</footer>
```

### Layout notes

- `header` holds page brand and navigation
- `main` includes the page's primary content
- `aside` holds secondary content, like related links or adverts
- `footer` is very useful for legal info, links, and contact details
- Use `section` to group related content and `article` for independent pieces

---

## 🎥 Multimedia and Embedded Content

### Images with accessibility

```html
<img src="hero.jpg" alt="A student learning HTML on a laptop" width="1200" height="675">
```

### Video embedding

```html
<video controls>
    <source src="video.mp4" type="video/mp4">
    Your browser does not support the video tag.
</video>
```

### Audio embedding

```html
<audio controls>
    <source src="audio.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
</audio>
```

### Embedding external content

Use `<iframe>` for maps, forms, or embedded content, but keep accessibility in mind.

```html
<iframe src="https://www.example.com/embed" title="Example embedded content" width="600" height="400"></iframe>
```

---

## ♿ Accessibility and Screen Reader Support

Accessibility is not optional. It makes websites usable for everyone.

### Keyboard-friendly forms

- Use `<label>` for every input
- Use `fieldset` and `legend` to group related fields
- Use `aria-label` when a visible label is not possible

### Accessible landmarks

Landmarks help users navigate pages quickly.

- `<header>`
- `<nav>`
- `<main>`
- `<aside>`
- `<footer>`

### ARIA basics

Use ARIA only when native HTML elements are not enough.

```html
<button aria-expanded="false" aria-controls="menu-list">Menu</button>
<ul id="menu-list" hidden>...</ul>
```

---

## 🧠 Metadata, SEO, and Structured Data

### Essential metadata

```html
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Learn advanced HTML structure, accessibility, and best practices.">
<title>Advanced HTML Guide</title>
```

### Open Graph for social sharing

```html
<meta property="og:title" content="Advanced HTML Guide">
<meta property="og:description" content="A beginner-friendly course on advanced HTML techniques.">
<meta property="og:image" content="https://example.com/preview.jpg">
```

### Structured data with JSON-LD

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Course",
  "name": "Advanced HTML Guide",
  "description": "A detailed HTML course from beginner to advanced.",
  "provider": {
    "@type": "Organization",
    "name": "Innovation Frontend Learning"
  }
}
</script>
```

---

## 🧾 Advanced Form Patterns

### Example: grouped fields

```html
<form>
    <fieldset>
        <legend>Personal details</legend>
        <label for="name">Full name</label>
        <input id="name" name="name" type="text" required>

        <label for="email">Email address</label>
        <input id="email" name="email" type="email" required>
    </fieldset>

    <fieldset>
        <legend>Preferences</legend>
        <label>
            <input type="checkbox" name="newsletter"> Subscribe to newsletter
        </label>
    </fieldset>

    <button type="submit">Submit</button>
</form>
```

### Improve usability

- Add helpful placeholder text
- Group related inputs
- Use `autocomplete` attributes for browser autofill
- Use visible error messages when validation fails

---

## ✅ Best Practices, Performance, and Validation

### Clean HTML habits

- Always close tags
- Nest elements correctly
- Keep indentation consistent
- Use meaningful class names when needed

### Performance tips

- Use optimized images
- Prefer SVG for icons when possible
- Avoid unnecessary `iframe` embeds

### Validation

Check your HTML with tools like:
- [W3C Markup Validation Service](https://validator.w3.org)
- [HTMLHint](https://htmlhint.com)

---

## 📌 Next Steps

After this module, move to the project challenges in the `projects/` folder:

- [Beginner projects](./projects/beginner)
- [Intermediate projects](./projects/intermediate)
- [Advanced projects](./projects/advanced)

This module prepares you to build real websites with strong structure, accessibility, and modern markup.
