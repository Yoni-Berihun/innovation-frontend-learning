# 01-Introduction: HTML Basics

> Learn the fundamentals of HTML and create your first webpage!

- [Start Exercises](./Exercises.md)
- [Next Module: Semantic HTML](../02-semantic-html/README.md)
- [HTML Track Overview](../README.md)

Welcome! 👋 This module introduces you to HTML and shows you how it works. Don't worry if you've never seen code before—we'll start from the very beginning.

---

## 🌐 What is HTML?

### The Simple Answer
HTML stands for **HyperText Markup Language**. It's the code that tells your browser what to display on a webpage.

### A Real-World Analogy 🏠
Think of HTML like the **blueprint of a house**:
- `<header>` = The front entrance
- `<main>` = The living spaces inside
- `<footer>` = The foundation/utility area
- `<article>` = Individual rooms
- `<p>` = Furniture inside rooms

The blueprint (HTML) provides structure. CSS paints it. JavaScript makes it interactive.

---

## 🎯 Learning Objectives

By the end of this module, you'll understand:

✅ What HTML is and why it matters  
✅ HTML document structure  
✅ Common HTML tags  
✅ How to write your first HTML page  
✅ How browsers read HTML  

---

## 🏗️ HTML Document Structure

Every HTML document has this basic structure:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Page Title</title>
</head>
<body>
    <!-- Content goes here -->
</body>
</html>
```

Let's break it down:

### 1️⃣ `<!DOCTYPE html>`
- Tells the browser this is an HTML5 document
- Must be the first line
- Not technically an HTML tag, just an instruction

### 2️⃣ `<html lang="en">`
- The root element containing everything
- `lang="en"` tells the browser this is English

### 3️⃣ `<head>` - The Brain 🧠
Contains information ABOUT the page (not visible to users):

```html
<head>
    <meta charset="UTF-8">                  <!-- Character encoding -->
    <meta name="viewport" ...>              <!-- Mobile responsiveness -->
    <title>My Website</title>               <!-- Browser tab title -->
    <meta name="description" content="..."> <!-- Search engine description -->
</head>
```

### 4️⃣ `<body>` - The Visible Content 👀
Everything users see goes here:

```html
<body>
    <h1>My Heading</h1>
    <p>My paragraph text.</p>
    <button>Click me!</button>
</body>
```

---

## 🏷️ Essential HTML Tags

### Headings 📍
```html
<h1>This is the largest heading</h1>  <!-- Main title -->
<h2>This is a subheading</h2>
<h3>Smaller heading</h3>
<!-- ... up to h6 -->
```

**Remember:** Only use one `<h1>` per page!

### Paragraphs 📝
```html
<p>This is a paragraph of text.</p>
<p>This is another paragraph.</p>
```

### Links 🔗
```html
<!-- External link -->
<a href="https://google.com">Click here to visit Google</a>

<!-- Link to another page -->
<a href="about.html">About Us</a>

<!-- Link to file -->
<a href="document.pdf">Download PDF</a>
```

### Images 🖼️
```html
<img src="image.jpg" alt="Description of image">
```

**Why `alt` text?** It describes the image if it doesn't load, and helps screen readers for accessibility.

### Lists 📋
```html
<!-- Unordered list (bullets) -->
<ul>
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
</ul>

<!-- Ordered list (numbered) -->
<ol>
    <li>First step</li>
    <li>Second step</li>
    <li>Third step</li>
</ol>
```

### Text Formatting 💅
```html
<strong>This text is important (bold)</strong>
<em>This text is emphasized (italic)</em>
<u>This is underlined</u>
<small>This is smaller text</small>
```

---

## 💡 Key Concepts

### Tags & Elements
- **Tag**: `<p>` or `</p>`
- **Element**: `<p>This is content</p>` (opening tag + content + closing tag)

### Attributes
Attributes provide additional information:

```html
<img src="photo.jpg" alt="My photo" width="200" height="150">
        ^^^                ^^^       ^^^^^  ^^^
       attribute name  attribute   attribute name
                        value
```

Common attributes:
- `src` - Source of image or link
- `href` - URL for links
- `alt` - Alternative text
- `id` - Unique identifier
- `class` - Category for styling
- `style` - Inline CSS styling

### Nesting & Indentation
```html
<!-- Correct nesting -->
<div>
    <p>Paragraph inside a div</p>
</div>

<!-- Wrong nesting (don't do this!) -->
<div>
    <p>This is wrong
</div>
</p>
```

**Always indent to show structure!**

---

## 📝 Your First HTML Page

Let's create a simple webpage step by step:

### Step 1: Create a File
1. Open VS Code
2. Create a new file
3. Save it as `index.html`

### Step 2: Type the Code
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>My First Website</title>
</head>
<body>
    <h1>Welcome to My Website!</h1>
    <p>Hello! This is my first HTML page.</p>
    
    <h2>About Me</h2>
    <p>I am learning to code. It's exciting!</p>
    
    <h2>My Favorite Things</h2>
    <ul>
        <li>Coding</li>
        <li>Building websites</li>
        <li>Learning new things</li>
    </ul>
    
    <a href="https://google.com">Visit Google</a>
</body>
</html>
```

### Step 3: Open in Browser
1. Right-click the file
2. Select "Open with" → Browser
3. You should see your webpage!

### Step 4: Experiment
- Change the heading text
- Add more paragraphs
- Add more list items
- Save and refresh the browser

---

## 🎨 How Browsers Render HTML

```
Your HTML File
      ↓
   Browser reads it
      ↓
  Creates the DOM
  (Document Object Model)
      ↓
   Applies CSS styling
      ↓
   Runs JavaScript
      ↓
   Displays webpage
```

---

## 🐛 Common Mistakes to Avoid

### ❌ Missing Closing Tags
```html
<!-- Wrong -->
<p>This paragraph isn't closed

<!-- Correct -->
<p>This paragraph is properly closed</p>
```

### ❌ Incorrect Nesting
```html
<!-- Wrong -->
<p><strong>Text</p></strong>

<!-- Correct -->
<p><strong>Text</strong></p>
```

### ❌ Missing DOCTYPE
```html
<!-- Wrong - missing DOCTYPE -->
<html>
    <body>...</body>
</html>

<!-- Correct -->
<!DOCTYPE html>
<html>
    <body>...</body>
</html>
```

### ❌ Not Using Semantic Tags
```html
<!-- Wrong - just divs everywhere -->
<div>Title</div>
<div>Article content</div>

<!-- Correct - use semantic tags -->
<h1>Title</h1>
<article>Article content</article>
```

---

## 🎬 Learning Resources

### 📹 Videos
- [HTML Crash Course (Traversy Media)](https://youtu.be/UB1O30fR-EE)
- [HTML Tutorial (Codecademy)](https://www.codecademy.com/learn/learn-html)
- [HTML Basics (Freecodecamp)](https://youtu.be/qz0aGYrrlhU)

### 📚 Articles & Docs
- [MDN HTML Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics)
- [W3Schools HTML Tutorial](https://www.w3schools.com/html/)
- [HTML5 Specification](https://html.spec.whatwg.org/)

### 🛠️ Tools
- [HTML Validator](https://validator.w3.org/)
- [VS Code HTML Extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode.html-language-server)

---

## ✅ Knowledge Check

### Quick Review Questions

1. **What does HTML stand for?**
2. **What is the purpose of `<!DOCTYPE html>`?**
3. **Why should we use semantic tags?**
4. **What's the difference between `<em>` and `<strong>`?**
5. **How many `<h1>` tags should be on a page?**
6. **Why is `alt` text important for images?**
7. **What goes in the `<head>` vs `<body>`?**

<details>
<summary>View Answers</summary>

1. HyperText Markup Language
2. To tell the browser this is an HTML5 document
3. For accessibility, SEO, and semantic meaning
4. `<em>` is for emphasis (italic), `<strong>` is for importance (bold)
5. One - it's the main heading
6. For accessibility and SEO when images don't load
7. `<head>` has metadata, `<body>` has visible content

</details>

---

## 🚀 Next Steps

Now that you understand HTML basics:

1. Complete the **Exercises** below
2. Build your first real webpage
3. Experiment with different tags
4. Move to [Module 2: Semantic HTML](../02-semantic-html)

---

