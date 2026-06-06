# Exercises: HTML Introduction

> Practice your HTML skills with these hands-on exercises!

---

## 🟢 Easy Exercises

### Exercise 1.1: Create Your First Webpage
**Objective:** Create a basic HTML document

**Instructions:**
1. Create a new file called `my-first-page.html`
2. Add the complete HTML structure (DOCTYPE, html, head, body)
3. Add a title in the `<head>`
4. Add a heading and a paragraph in the `<body>`
5. Open in your browser and verify it displays

**Starter Template:**
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>???</title>
</head>
<body>
    <!-- Add content here -->
</body>
</html>
```

**Expected Output:** A webpage with your title visible in the browser tab and your heading and paragraph visible on the page.

---

### Exercise 1.2: Add Multiple Elements
**Objective:** Practice using different HTML tags

**Create a webpage that includes:**
- A main heading (h1)
- At least 2 subheadings (h2)
- At least 3 paragraphs
- An unordered list with 4-5 items
- An ordered list with 3-4 steps

**Example structure:**
```html
<h1>Topic Name</h1>
<p>Introduction paragraph...</p>

<h2>Section 1</h2>
<p>Content...</p>
<ul>
    <li>Item 1</li>
    <!-- more items -->
</ul>

<h2>Section 2</h2>
<p>Content...</p>
<ol>
    <li>Step 1</li>
    <!-- more steps -->
</ol>
```

**Tip:** Use proper indentation to keep your code organized.

---

### Exercise 1.3: Add Links and Images
**Objective:** Practice adding interactive elements

**Create a webpage with:**
- At least 2 links to external websites (use `<a href="">`)
- At least 1 link to another HTML file (you can create a simple second page)
- At least 2 images with proper `alt` text

**Example:**
```html
<a href="https://example.com">Visit Example</a>
<img src="image.jpg" alt="Description of the image">
```

**Tip:** For images, you can download free images from [Pexels](https://www.pexels.com) or [Unsplash](https://unsplash.com)

---

## 🟡 Medium Exercises

### Exercise 2.1: Build a Personal Profile Page
**Objective:** Create a more complex webpage with multiple sections

**Create a personal profile page including:**
- Your name as the main heading (h1)
- A profile photo with alt text
- "About Me" section (paragraph)
- "Skills" section (unordered list)
- "Experience" section (ordered list or details)
- "Contact" section (links to social media or contact form links)
- Proper HTML structure and indentation

**Requirements:**
- Use all appropriate HTML tags
- Include alt text for all images
- Make sure all sections are clearly organized
- Use semantic structure

**Example sections:**
```html
<h1>John Doe</h1>
<img src="profile.jpg" alt="My profile photo">

<h2>About Me</h2>
<p>I am a student learning web development...</p>

<h2>Skills</h2>
<ul>
    <li>HTML</li>
    <li>Problem Solving</li>
</ul>
```

---

### Exercise 2.2: Create a Multi-Page Website
**Objective:** Practice linking pages together

**Create a 3-page website with:**
- `index.html` - Home page with overview and navigation
- `about.html` - About page with your story
- `portfolio.html` - Portfolio page with project links

**Each page should have:**
- Navigation menu with links to all 3 pages
- Appropriate headings
- Content specific to that page
- Same structure on all pages

**Example structure for index.html:**
```html
<h1>Welcome</h1>
<ul>
    <li><a href="index.html">Home</a></li>
    <li><a href="about.html">About</a></li>
    <li><a href="portfolio.html">Portfolio</a></li>
</ul>
<p>Welcome to my website!</p>
```

---

### Exercise 2.3: Create a Resume Page
**Objective:** Practice structuring complex content

**Create an HTML resume including:**
- Your name as main heading
- Contact information (email, phone, LinkedIn)
- Professional summary
- Work experience (company, position, dates, responsibilities)
- Education (school, degree, graduation date)
- Skills (organized by category)

**Structure suggestion:**
```html
<h1>Your Name</h1>
<!-- Contact info -->
<p>Email: example@email.com | Phone: 123-456-7890</p>

<h2>Professional Summary</h2>
<!-- Summary paragraph -->

<h2>Experience</h2>
<h3>Job Title at Company</h3>
<p>Dates: Jan 2023 - Present</p>
<ul>
    <li>Responsibility 1</li>
    <li>Responsibility 2</li>
</ul>
```

---

## 🔴 Challenging Exercises

### Exercise 3.1: Create a Blog Homepage
**Objective:** Practice complex layouts and nested elements

**Create a blog homepage with:**
- Site header with title and tagline
- Navigation menu
- Featured article preview
- List of 3-5 blog post previews
- Each preview should include:
  - Title (as a link to a post page)
  - Publication date
  - Thumbnail image
  - Excerpt/summary
  - "Read More" link
- Sidebar with categories
- Footer with copyright info

**Challenge:** Organize everything with proper HTML structure and semantic meaning.

---

### Exercise 3.2: Create a Product Catalog Page
**Objective:** Practice organizing complex data with HTML

**Create a product catalog including:**
- Page title and description
- Filter/category section
- Product grid/list with:
  - Product image (with alt text)
  - Product name
  - Price
  - Brief description
  - "Add to Cart" button (can be a fake link)
  - Rating (stars or number)
- At least 8-10 different products
- Footer with company info

**Example product structure:**
```html
<div class="product">
    <img src="product.jpg" alt="Product name">
    <h3>Product Name</h3>
    <p class="price">$19.99</p>
    <p class="description">Brief description...</p>
    <p class="rating">⭐⭐⭐⭐⭐ (47 reviews)</p>
    <a href="#cart">Add to Cart</a>
</div>
```

---

### Exercise 3.3: Create a Documentation Page
**Objective:** Practice creating complex navigation and structure

**Create comprehensive documentation for a fictional tool/library:**
- Table of contents (internal links)
- Multiple sections (Introduction, Getting Started, API Reference, Examples, FAQ)
- Code examples in each section
- Nested headings (h1, h2, h3)
- Internal links that jump to different sections
- External links to related resources
- Search placeholder

**Requirements:**
- Use proper heading hierarchy
- Make it easy to navigate
- Include at least 20 sections
- Use anchor links (`<a href="#section-id">`)

**Example structure:**
```html
<h1>Documentation</h1>

<nav>
    <ul>
        <li><a href="#intro">Introduction</a></li>
        <li><a href="#setup">Setup</a></li>
        <li><a href="#api">API Reference</a></li>
    </ul>
</nav>

<section id="intro">
    <h2>Introduction</h2>
    <p>Content...</p>
</section>
```

---

## 🎯 Bonus Challenges

### Bonus 1: Validate Your HTML
**Objective:** Learn to validate HTML code

1. Go to [W3C Validator](https://validator.w3.org/)
2. Upload or paste your HTML from any of the above exercises
3. Fix any errors reported
4. Validate until all errors are gone

**What you're learning:** How to write valid, standards-compliant HTML.

---

### Bonus 2: Browser Developer Tools
**Objective:** Learn to inspect websites

1. Open any website in your browser
2. Press `F12` or `Ctrl+Shift+I` to open Developer Tools
3. Click the "Inspector" or "Elements" tab
4. Hover over different parts of the page to see their HTML
5. Try to identify:
   - Semantic tags used
   - Class and ID attributes
   - Image sources
   - Link destinations

**What you're learning:** How professionals inspect and debug websites.

---

### Bonus 3: Create a Webpage from a Screenshot
**Objective:** Reverse-engineer a website design

1. Find a screenshot of a simple website (or create one yourself)
2. Analyze its structure:
   - How many sections?
   - What headings?
   - What content types?
   - What images?
3. Create the HTML that matches the structure
4. Don't worry about styling yet—just structure!

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
- [ ] Attempted at least one Bonus Challenge
- [ ] All code is properly indented
- [ ] All code validates without errors

---

## 💡 Tips for Success

1. **Don't copy-paste:** Type out the code to learn better
2. **Experiment:** Try changing things and see what happens
3. **Validate:** Use the HTML validator to check your work
4. **Organize:** Use proper indentation and structure
5. **Comment:** Add comments to explain your code
6. **Ask:** If you're stuck, ask for help from mentors or peers

---

## 🚀 Next Steps

After completing these exercises:

1. Review any concepts you struggled with
2. Move to [Module 2: Semantic HTML](../02-semantic-html)
3. Start the Beginner Project in the Projects folder
4. Continue building your HTML skills!

---

## ✅ Success Criteria

You've mastered HTML Introduction when you can:

✅ Create a valid HTML document from scratch  
✅ Use common HTML tags appropriately  
✅ Organize content with proper structure  
✅ Add links and images  
✅ Create multi-page websites  
✅ Validate your HTML code  

---

