# Exercises: Semantic HTML

> Practice using semantic tags to write meaningful HTML!

---

## 🟢 Easy Exercises

### Exercise 1.1: Identify Semantic vs Non-Semantic
**Objective:** Learn to recognize semantic tags

**Look at these two versions. Identify which one is semantic and why:**

Version A:
```html
<div>
    <div>My Website</div>
    <div>
        <a href="/">Home</a>
        <a href="/about">About</a>
    </div>
</div>
```

Version B:
```html
<header>
    <h1>My Website</h1>
    <nav>
        <a href="/">Home</a>
        <a href="/about">About</a>
    </nav>
</header>
```

**Answer questions:**
1. Which is semantic?
2. What semantic tags does it use?
3. Why is it better?

---

### Exercise 1.2: Replace Divs with Semantic Tags
**Objective:** Convert non-semantic code to semantic

**Convert this code to use semantic tags:**

```html
<div class="header">
    <div class="title">Welcome</div>
    <div class="links">
        <a href="/">Home</a>
        <a href="/about">About</a>
    </div>
</div>

<div class="content">
    <div class="article">
        <div class="heading">My Article</div>
        <p>Content here...</p>
    </div>
</div>

<div class="footer">
    <p>© 2024</p>
</div>
```

**Requirements:**
- Replace all divs with semantic tags
- Keep the same content
- Maintain proper HTML structure

---

### Exercise 1.3: Mark Up a Paragraph
**Objective:** Practice text-level semantic tags

**Take this plain text and add semantic HTML tags where appropriate:**

```
Published on January 15, 2024 by John Doe

This is a very important announcement. Please pay close attention. The deadline is May 1st. We recommend using the alert() function for notifications. You must follow this rule carefully.
```

**Requirements:**
- Mark the publication date with `<time>`
- Mark the author name appropriately
- Use `<strong>` for important content
- Use `<code>` for code
- Use `<em>` for emphasis

---

## 🟡 Medium Exercises

### Exercise 2.1: Build a Blog Post Structure
**Objective:** Create a semantically structured blog post

**Create an HTML file with:**
- A header with site title and navigation
- A main section containing:
  - An article with:
    - Title (h1)
    - Author and publish date
    - Featured image
    - Content (multiple paragraphs)
    - Code examples (using `<code>` and `<pre>`)
  - An aside with related posts
- A footer

**Template to build from:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Blog Post</title>
</head>
<body>
    <header>
        <!-- Add header content -->
    </header>
    
    <main>
        <article>
            <!-- Add article content -->
        </article>
        
        <aside>
            <!-- Add related posts -->
        </aside>
    </main>
    
    <footer>
        <!-- Add footer content -->
    </footer>
</body>
</html>
```

---

### Exercise 2.2: Create a News Website Layout
**Objective:** Build complex semantic structure

**Create an HTML news website with:**
- Header with site name and main navigation
- Multiple sections:
  - "Top Stories" section with 3 articles
  - "Local News" section with 2 articles
  - "Sports" section with 2 articles
- Each article should have:
  - Heading
  - Author and publication date
  - Thumbnail image
  - Summary paragraph
- Sidebar with categories
- Footer with copyright and links

**Requirements:**
- Use `<section>` to group articles by category
- Use `<article>` for each story
- Use `<time>` for dates
- Use `<aside>` for sidebar
- Proper semantic structure throughout

---

### Exercise 2.3: Refactor a Messy Website
**Objective:** Improve existing code with semantic HTML

**Here's a poorly structured webpage. Refactor it to use semantic tags:**

```html
<html>
<body>
<div>
    <div>
        <p>Welcome to My Website</p>
        <a href="/">Home</a>
        <a href="/about">About</a>
    </div>
</div>

<div>
    <div>
        <p>Article Title</p>
        <p>By John Doe on January 1, 2024</p>
        <p>Article content goes here. This is important information.</p>
        <p>Use the console.log() function to debug.</p>
    </div>
    
    <div>
        <p>Related Reading:</p>
        <a href="/">Post 1</a>
        <a href="/">Post 2</a>
    </div>
</div>

<div>
    <p>© 2024 My Site</p>
</div>
</body>
</html>
```

**Requirements:**
- Add proper semantic tags
- Add missing HTML structure (`<!DOCTYPE>`, `<head>`, etc.)
- Use appropriate tags for each section
- Mark important text with `<strong>`
- Mark code with `<code>`
- Mark the date with `<time>`

---

## 🔴 Challenging Exercises

### Exercise 3.1: Create an E-commerce Product Page
**Objective:** Build a complex semantic layout

**Create a product page with semantic structure:**
- Header with site name and navigation
- Main content with:
  - Product title (h1)
  - Product images gallery
  - Product details section:
    - Price
    - Rating
    - In stock/out of stock status
    - Description
    - Features (as a list)
  - Reviews section:
    - Multiple review cards with:
      - Reviewer name
      - Rating
      - Date
      - Review text
  - Related products sidebar
- Footer

**Requirements:**
- All content properly marked with semantic tags
- Appropriate use of heading hierarchy (h1, h2, h3)
- Logical section organization
- Accessibility in mind

---

### Exercise 3.2: Build a Documentation Site Structure
**Objective:** Create a comprehensive documentation layout

**Create a documentation page with:**
- Header with site name and search bar
- Main content with:
  - Introductory section
  - Multiple guide sections:
    - Getting Started
    - Installation
    - Configuration
    - API Reference
    - Examples
    - FAQ
  - Each section contains:
    - Main heading
    - Explanation paragraphs
    - Code examples
    - Links to related sections
- Sidebar with:
  - Quick navigation
  - Related resources
- Footer

**Requirements:**
- Proper semantic structure
- Use `<code>` for code snippets
- Use `<time>` for version dates
- Use `<nav>` for navigation
- Proper heading hierarchy
- Clear visual structure through HTML alone

---

### Exercise 3.3: Create a Portfolio Website
**Objective:** Build a portfolio with semantic structure

**Create a multi-page portfolio website:**

**Pages to create:**
1. index.html - Home page
2. about.html - About page
3. portfolio.html - Portfolio/projects page
4. contact.html - Contact page

**Content requirements:**
- Consistent header and navigation on all pages
- Proper semantic structure on each page
- About page: Personal intro, skills, experience timeline
- Portfolio page: Project showcases with descriptions
- Contact page: Contact form (just HTML, no functionality)
- Footer on all pages

**Requirements:**
- Use semantic tags throughout
- Proper HTML structure
- Navigation menu links to all pages
- Use `<time>` for dates
- Use `<article>` for project descriptions
- Use `<section>` to organize content

---

## 📚 Extra Challenge: Accessibility Review

### Exercise: Test for Accessibility

**For any previous exercise:**

1. Open in your browser
2. Press `F12` to open Developer Tools
3. Go to "Accessibility" tab
4. Check for:
   - Proper heading hierarchy (no skipped levels)
   - Images with alt text
   - Semantic structure
   - Color contrast
5. Fix any issues found

**What you're learning:** How to test and improve accessibility.

---

## 📋 Exercise Checklist

- [ ] Completed Exercise 1.1
- [ ] Completed Exercise 1.2
- [ ] Completed Exercise 1.3
- [ ] Completed Exercise 2.1
- [ ] Completed Exercise 2.2
- [ ] Completed Exercise 2.3
- [ ] Completed Exercise 3.1
- [ ] Completed Exercise 3.2
- [ ] Completed Exercise 3.3
- [ ] Performed accessibility review
- [ ] All code uses semantic tags
- [ ] All code validates

---

## ✅ Success Criteria

You've mastered Semantic HTML when you can:

✅ Identify semantic vs non-semantic code  
✅ Choose correct semantic tag for any content  
✅ Build accessible webpages  
✅ Understand SEO benefits  
✅ Refactor existing code to be semantic  
✅ Explain why semantic HTML matters  

---

## 🚀 Next Steps

1. Review [Module 3: Forms & Validation](../03-forms-validation)
2. Start the HTML Projects
3. Continue building semantic HTML!

---

