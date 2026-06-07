# 03-Forms & Validation: Collect User Data

> Build interactive forms to collect and validate user information.

- [Start Exercises](./Exercises.md)
- [Previous Module: Semantic HTML](../02-semantic-html/README.md)
- [Next Module: Advanced HTML](../04-advanced-html/README.md)
- [HTML Track Overview](../README.md)

Welcome to Forms! 📋 This module teaches you to create HTML forms that let users input information like names, emails, passwords, and more. We'll also explore how to validate that information.

---

## 🎯 Learning Objectives

By the end of this module, you'll:

✅ Create functional HTML forms  
✅ Use all common form elements  
✅ Add labels for accessibility  
✅ Validate user input  
✅ Handle form submissions  
✅ Build user-friendly forms  

---

## 📋 The `<form>` Element

Every form starts with the `<form>` tag:

```html
<form action="/submit" method="POST">
    <!-- Form elements go here -->
</form>
```

**Attributes:**
- `action` - Where the form data goes (URL)
- `method` - How to send it (GET or POST)

---

## 🔤 Text Input Elements

### `<input>` - The Workhorse
The most versatile form element:

```html
<!-- Text input -->
<input type="text" name="username" placeholder="Enter username">

<!-- Email -->
<input type="email" name="email" placeholder="Enter email">

<!-- Password (hides text) -->
<input type="password" name="password" placeholder="Enter password">

<!-- Number -->
<input type="number" name="age" min="0" max="120">

<!-- Date -->
<input type="date" name="birthdate">

<!-- URL -->
<input type="url" name="website">

<!-- Search -->
<input type="search" name="query" placeholder="Search...">

<!-- Telephone -->
<input type="tel" name="phone" placeholder="123-456-7890">

<!-- Color picker -->
<input type="color" name="favorite_color">

<!-- Range slider -->
<input type="range" name="volume" min="0" max="100">
```

---

## 📝 Text Areas & Selects

### `<textarea>` - Multi-line Text
```html
<textarea name="message" rows="4" cols="50" placeholder="Enter your message..."></textarea>
```

### `<select>` - Dropdown List
```html
<select name="country">
    <option value="">-- Select a country --</option>
    <option value="usa">United States</option>
    <option value="uk">United Kingdom</option>
    <option value="canada">Canada</option>
    <option value="australia">Australia</option>
</select>
```

### `<datalist>` - Suggestions While Typing
```html
<input type="text" list="browsers" name="browser">
<datalist id="browsers">
    <option value="Chrome">
    <option value="Firefox">
    <option value="Safari">
</datalist>
```

---

## ✅ Checkboxes & Radio Buttons

### Checkboxes (Multiple selections allowed)
```html
<label>
    <input type="checkbox" name="subscribe" value="yes"> Subscribe to newsletter
</label>

<label>
    <input type="checkbox" name="terms" value="yes" required> I agree to terms
</label>
```

### Radio Buttons (Only one selection)
```html
<label>
    <input type="radio" name="gender" value="male"> Male
</label>
<label>
    <input type="radio" name="gender" value="female"> Female
</label>
<label>
    <input type="radio" name="gender" value="other"> Other
</label>
```

---

## 📌 Labels - Make Forms Accessible

**Always** use `<label>` tags:

### Method 1: Wrapping
```html
<label>
    Email:
    <input type="email" name="email">
</label>
```

### Method 2: for/id Connection
```html
<label for="email-input">Email:</label>
<input type="email" id="email-input" name="email">
```

**Why?**
- Screen readers can read labels
- Clicking label focuses input
- Better accessibility
- Better user experience

---

## ✔️ Form Validation

### HTML5 Validation Attributes

#### `required`
Field must have a value:
```html
<input type="text" name="name" required>
```

#### `type="email"`
Checks for valid email format:
```html
<input type="email" name="email">
```

#### `type="number"`
Only accepts numbers:
```html
<input type="number" name="age">
```

#### `minlength` and `maxlength`
Restrict text length:
```html
<input type="text" name="username" minlength="3" maxlength="20">
```

#### `min` and `max`
Restrict number values:
```html
<input type="number" name="age" min="0" max="120">
```

#### `pattern`
Validate with regex:
```html
<!-- Phone number format -->
<input type="text" name="phone" pattern="[0-9]{3}-[0-9]{3}-[0-9]{4}">
```

#### `step`
Increment for numbers:
```html
<input type="number" name="price" step="0.01">
```

---

## 🔘 Buttons

### Submit Button
```html
<button type="submit">Submit Form</button>
```

### Reset Button (Clear form)
```html
<button type="reset">Clear</button>
```

### Regular Button
```html
<button type="button">Click Me</button>
```

### Input Button (Alternative)
```html
<input type="submit" value="Submit">
```

---

## 📋 Complete Form Example

```html
<!DOCTYPE html>
<html>
<head>
    <title>Contact Form</title>
</head>
<body>
    <h1>Contact Us</h1>
    
    <form action="/submit" method="POST">
        <!-- Name field -->
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" required>
        
        <!-- Email field -->
        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>
        
        <!-- Subject dropdown -->
        <label for="subject">Subject:</label>
        <select id="subject" name="subject" required>
            <option value="">-- Select --</option>
            <option value="general">General Inquiry</option>
            <option value="support">Support</option>
            <option value="feedback">Feedback</option>
        </select>
        
        <!-- Message textarea -->
        <label for="message">Message:</label>
        <textarea id="message" name="message" rows="5" required></textarea>
        
        <!-- Checkbox -->
        <label>
            <input type="checkbox" name="newsletter" value="yes">
            Subscribe to newsletter
        </label>
        
        <!-- Buttons -->
        <button type="submit">Send Message</button>
        <button type="reset">Clear</button>
    </form>
</body>
</html>
```

---

## 🎨 Grouping Related Fields

### `<fieldset>` and `<legend>`
```html
<fieldset>
    <legend>Contact Information</legend>
    
    <label for="name">Name:</label>
    <input type="text" id="name" name="name">
    
    <label for="email">Email:</label>
    <input type="email" id="email" name="email">
</fieldset>

<fieldset>
    <legend>Preferences</legend>
    
    <label>
        <input type="radio" name="format" value="email"> Email
    </label>
    <label>
        <input type="radio" name="format" value="phone"> Phone
    </label>
</fieldset>
```

---

## 📤 File Upload

```html
<label for="file-upload">Choose a file:</label>
<input type="file" id="file-upload" name="document" accept=".pdf,.doc,.docx">
```

**Attributes:**
- `accept` - File types allowed (`.pdf`, `.jpg`, etc.)
- `multiple` - Allow multiple files

---

## ✅ Knowledge Check

### Quick Review Questions

1. **What's the difference between `<input type="text">` and `<textarea>`?**
2. **Why use `<label>` tags?**
3. **Name 5 input types.**
4. **What does `required` attribute do?**
5. **How do radio buttons differ from checkboxes?**

<details>
<summary>View Answers</summary>

1. Input is single line, textarea allows multiple lines
2. For accessibility, improved user experience, better semantics
3. text, email, password, number, date, checkbox, radio, file, etc.
4. Makes the field mandatory before form submission
5. Radio buttons allow only one selection, checkboxes allow multiple

</details>

---

## 🎬 Learning Resources

### 📹 Videos
- [HTML Forms Tutorial (Traversy Media)](https://youtu.be/fNcJuPF4-Co)
- [Form Validation (Codecademy)](https://www.codecademy.com/learn/learn-html/modules/learn-forms)

### 📚 Docs
- [MDN: HTML Forms](https://developer.mozilla.org/en-US/docs/Learn/Forms)
- [W3Schools Forms](https://www.w3schools.com/html/html_forms.asp)

---

## 🚀 Next Steps

1. Complete the **Exercises** below
2. Build practical forms
3. Review projects in the HTML folder
4. Combine HTML + CSS for styled forms

---

