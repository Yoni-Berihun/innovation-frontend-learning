# 02-Semantic HTML: Write Meaningful Code

> Use HTML tags that describe what content they contain, not just how it looks.

- [Start Exercises](./Exercises.md)
- [Previous Module: HTML Introduction](../01-introduction/README.md)
- [Next Module: Forms & Validation](../03-forms-validation/README.md)
- [HTML Track Overview](../README.md)

Welcome to Semantic HTML! 🎯 This module teaches you to write HTML that means something, making your code easier to understand and your websites more accessible.

---

## 🧠 What is Semantic HTML?

### The Simple Answer
Semantic HTML means using tags that clearly describe the **meaning** of the content they contain.

### ❌ Non-Semantic (Bad)
```html
<div>Welcome to my website</div>
<div>This is an article about coding</div>
<div>© 2024 My Company</div>
```

### ✅ Semantic (Good)
```html
<header>Welcome to my website</header>
<article>This is an article about coding</article>
<footer>© 2024 My Company</footer>
```

Both look the same in a browser, but semantic HTML:
- **Tells the browser** what each part does
- **Helps screen readers** understand the page
- **Improves SEO** for search engines
- **Makes code more readable** for developers

---

## 🎯 Learning Objectives

By the end of this module, you'll:

✅ Understand semantic vs non-semantic HTML  
✅ Know when to use semantic tags  
✅ Build accessible webpages  
✅ Improve your SEO  
✅ Write more meaningful code  

---

## 🏷️ Essential Semantic Tags

### Document Structure

#### `<header>`
Contains introductory content and navigation.

```html
<header>
    <h1>My Website</h1>
    <nav>
        <ul>
            <li><a href="/">Home</a></li>
            <li><a href="/about">About</a></li>
        </ul>
    </nav>
</header>
```

#### `<nav>`
Contains navigation links.

```html
<nav>
    <ul>
        <li><a href="/">Home</a></li>
        <li><a href="/about">About</a></li>
        <li><a href="/contact">Contact</a></li>
    </ul>
</nav>
```

#### `<main>`
The main content of the page (only one per page).

```html
<main>
    <h1>Welcome</h1>
    <article>Article content</article>
</main>
```

#### `<article>`
A complete, self-contained piece of content (blog post, news story, etc.).

```html
<article>
    <h2>How to Learn Web Development</h2>
    <p>Step 1: Learn HTML...</p>
    <p>Step 2: Learn CSS...</p>
</article>
```

#### `<section>`
A thematic grouping of content.

```html
<section>
    <h2>Skills</h2>
    <ul>
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
    </ul>
</section>
```

#### `<aside>`
Content slightly related to main content (sidebar, footnotes, etc.).

```html
<aside>
    <h3>Related Articles</h3>
    <ul>
        <li><a href="...">Article 1</a></li>
        <li><a href="...">Article 2</a></li>
    </ul>
</aside>
```

#### `<footer>`
Contains footer content (copyright, links, etc.).

```html
<footer>
    <p>© 2024 My Company</p>
    <p><a href="/privacy">Privacy Policy</a></p>
</footer>
```

---

### Text-Level Semantic Tags

#### `<strong>` vs `<b>`
- `<strong>` = This is **important** (semantically bold)
- `<b>` = Just make it **bold** (no semantic meaning)

**Use `<strong>`:**
```html
<p>This is <strong>very important</strong>!</p>
```

#### `<em>` vs `<i>`
- `<em>` = This is **emphasized** (semantically italic)
- `<i>` = Just make it *italic* (no semantic meaning)

**Use `<em>`:**
```html
<p>Please bring the <em>original</em> documents.</p>
```

#### `<mark>`
Highlights/marks important text.

```html
<p>Today's topic is <mark>very important</mark>!</p>
```

#### `<time>`
Marks date/time content (helps search engines).

```html
<p>Published on <time datetime="2024-01-15">January 15, 2024</time></p>
```

#### `<code>` and `<pre>`
For displaying code.

```html
<!-- Inline code -->
<p>Use the <code>console.log()</code> function.</p>

<!-- Code block -->
<pre><code>
function hello() {
    console.log("Hello!");
}
</code></pre>
```

---

## 📐 Common Page Layouts

### Blog Post Layout
```html
<header>
    <nav><!-- Navigation --></nav>
</header>

<main>
    <article>
        <h1>Article Title</h1>
        <p>Published by <author>John Doe</author> on <time>2024-01-15</time></p>
        <img src="featured.jpg" alt="Featured image">
        <p>Article content...</p>
    </article>
    
    <aside>
        <h3>Related Posts</h3>
        <ul>
            <li><a href="...">Post 1</a></li>
        </ul>
    </aside>
</main>

<footer>
    <p>© 2024 My Blog</p>
</footer>
```

### News Website Layout
```html
<header>
    <h1>News Today</h1>
    <nav><!-- Navigation --></nav>
</header>

<main>
    <section>
        <h2>Top Stories</h2>
        <article><!-- Story 1 --></article>
        <article><!-- Story 2 --></article>
    </section>
    
    <section>
        <h2>Local News</h2>
        <article><!-- Story 3 --></article>
    </section>
</main>

<footer>
    <p>© 2024 News Today</p>
</footer>
```

---

## ♿ Accessibility Benefits

Semantic HTML helps people with disabilities:

1. **Screen readers** understand the structure
2. **Keyboard users** can navigate better
3. **Mobile users** get better organization
4. **Everyone** has a better experience

### Example: Without Semantic HTML
```html
<div class="header">
    <div class="logo">My Site</div>
    <div class="menu">
        <span class="menu-item"><a href="/">Home</a></span>
        <span class="menu-item"><a href="/about">About</a></span>
    </div>
</div>
```

### Example: With Semantic HTML
```html
<header>
    <h1>My Site</h1>
    <nav>
        <ul>
            <li><a href="/">Home</a></li>
            <li><a href="/about">About</a></li>
        </ul>
    </nav>
</header>
```

Screen readers announce: "Navigation region with 2 links"

---

## 📊 Semantic HTML vs Divs

| Purpose | Semantic Tag | Or Div? |
|---------|--------------|---------|
| Page header | `<header>` | ❌ No |
| Navigation | `<nav>` | ❌ No |
| Main content | `<main>` | ❌ No |
| Article | `<article>` | ❌ No |
| Section | `<section>` | Only if not semantic |
| Generic grouping | `<div>` | ✅ Yes |
| Sidebar | `<aside>` | ❌ No |
| Page footer | `<footer>` | ❌ No |

---

## 🔍 SEO Benefits

Search engines use semantic HTML to understand your page:

```html
<!-- This helps Google -->
<article>
    <h1>Best Practices for Web Development</h1>
    <p>Published <time datetime="2024-01-15">January 15, 2024</time></p>
    <p>Content describes web development best practices...</p>
</article>
```

Search engines see:
- Clear main topic (h1)
- Publication date (time tag)
- Content about that topic

Result: Better ranking! 📈

---

## ✅ Knowledge Check

### Quick Review Questions

1. **What's the difference between `<header>` and `<head>`?**
2. **When should you use `<section>` vs `<article>`?**
3. **Why use `<strong>` instead of `<b>`?**
4. **Name 5 semantic HTML tags.**
5. **How does semantic HTML help accessibility?**

<details>
<summary>View Answers</summary>

1. `<header>` is visible content at top of page; `<head>` is metadata (invisible)
2. `<article>` is independent content; `<section>` groups related content
3. `<strong>` has semantic meaning (important), `<b>` is just visual
4. header, nav, main, article, section, aside, footer, figure, figcaption
5. Screen readers understand structure, better keyboard navigation

</details>

---

## 🎬 Learning Resources

### 📹 Videos
- [Semantic HTML (Traversy Media)](https://youtu.be/bOUhq46fd5g)
- [HTML5 Semantic Elements (Codecademy)](https://www.codecademy.com/courses/intro-to-web-development/lessons/semantic-html/exercises/intro)

### 📚 Articles & Docs
- [MDN: Semantic HTML](https://developer.mozilla.org/en-US/docs/Glossary/Semantic_HTML)
- [W3Schools Semantic Elements](https://www.w3schools.com/html/html5_semantic_elements.asp)

---

## 🚀 Next Steps

1. Complete the **Exercises** below
2. Review your previous code—can you make it more semantic?
3. Practice identifying semantic tags on real websites
4. Move to [Module 3: Forms & Validation](../03-forms-validation)

---

