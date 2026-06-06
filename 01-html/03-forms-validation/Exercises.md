# Exercises: HTML Forms & Validation

> Practice building and validating HTML forms!

---

## 🟢 Easy Exercises

### Exercise 1.1: Create a Simple Login Form
**Objective:** Learn basic form elements

**Create a login form with:**
- Username input
- Password input
- Submit button
- Proper labels

```html
<form>
    <label for="username">Username:</label>
    <input type="text" id="username" name="username">
    
    <label for="password">Password:</label>
    <input type="password" id="password" name="password">
    
    <button type="submit">Login</button>
</form>
```

---

### Exercise 1.2: Build a Contact Form
**Objective:** Practice multiple input types

**Create a contact form including:**
- Name field
- Email field
- Subject dropdown (General, Support, Feedback)
- Message textarea
- Submit and Reset buttons

**Requirements:**
- Use proper labels
- All fields should have `name` attributes
- Use appropriate input types

---

### Exercise 1.3: Newsletter Signup Form
**Objective:** Practice checkboxes and validation

**Create a signup form with:**
- Email field (required)
- Frequency dropdown (Daily, Weekly, Monthly)
- Checkbox: "Agree to terms" (required)
- Interests checkboxes:
  - Technology
  - Business
  - Entertainment
- Subscribe button

---

## 🟡 Medium Exercises

### Exercise 2.1: Build a Survey Form
**Objective:** Practice various form elements

**Create a survey form for a school with:**

**Personal Information:**
- Full Name (text, required)
- Email (email, required)
- Age (number, min 13, max 100)

**School Information:**
- Grade Level (dropdown)
- Years at School (number)

**Preferences (radio buttons):**
- How often do you visit? (Daily, Weekly, Monthly, Never)

**Interests (checkboxes):**
- Sports
- Arts
- Technology
- Music
- Other

**Comments:**
- Textarea for additional comments

---

### Exercise 2.2: Create a Job Application Form
**Objective:** Practice form organization and validation

**Create a job application form with multiple sections:**

**Personal Information:**
- First Name (required)
- Last Name (required)
- Email (required)
- Phone (required)
- LinkedIn Profile (URL)

**Employment:**
- Years of Experience (number)
- Current Position (text)
- Company (text)

**Availability:**
- Start Date (date)
- Available to relocate? (yes/no radio buttons)

**Experience:**
- Skills (textarea)
- Previous Companies (textarea)

**Attachments:**
- Resume (file upload)
- Cover Letter (file upload)

---

### Exercise 2.3: Event Registration Form
**Objective:** Practice complex form structures

**Create an event registration form:**

**Event Selection:**
- Which event? (dropdown with multiple events)

**Attendee Information:**
- Full Name (required)
- Email (required)
- Phone (required)

**Tickets:**
- Number of Tickets (dropdown: 1-10)
- Ticket Type (radio: Early Bird, Standard, VIP)

**Dietary Preferences (checkboxes):**
- Vegetarian
- Vegan
- Gluten-free
- No restrictions

**Special Requests:**
- Textarea for special requests

**Agreement:**
- Checkbox to agree to terms (required)

---

## 🔴 Challenging Exercises

### Exercise 3.1: Build a Complete E-commerce Checkout Form
**Objective:** Create realistic form

**Create a checkout form with multiple fieldsets:**

**Shipping Address:**
```
<fieldset>
    <legend>Shipping Address</legend>
    - Street Address (required)
    - City (required)
    - State (dropdown)
    - ZIP Code (required)
    - Country (dropdown)
</fieldset>
```

**Billing Address:**
```
<fieldset>
    <legend>Billing Address</legend>
    - Checkbox: "Same as shipping"
    - Or show: Street, City, State, ZIP, Country
</fieldset>
```

**Payment Information:**
```
<fieldset>
    <legend>Payment</legend>
    - Cardholder Name
    - Card Number
    - Expiration Date
    - CVV
    - Billing ZIP
</fieldset>
```

**Shipping Method:**
```
<fieldset>
    <legend>Shipping Method</legend>
    - Radio buttons for shipping options
    - Standard (5-7 days)
    - Express (2-3 days)
    - Overnight
</fieldset>
```

**Order Summary & Submit:**
- Checkbox: "Agree to terms"
- Submit button
- Cancel button

---

### Exercise 3.2: Build a User Profile Edit Form
**Objective:** Practice comprehensive form with validation

**Create a user profile form with:**

**Profile Picture:**
- File upload for avatar

**Basic Information:**
- Username (text, required, minlength 3, maxlength 20)
- First Name (text, required)
- Last Name (text, required)
- Email (email, required)
- Phone (tel)
- Website (url)

**Date & Location:**
- Date of Birth (date)
- Country (dropdown)
- City (text)
- Bio (textarea, maxlength 500)

**Preferences:**
- Language (dropdown)
- Theme: Dark/Light (radio)
- Notifications (checkboxes):
  - Email notifications
  - SMS notifications
  - Marketing emails

**Social Media:**
- Twitter (url)
- LinkedIn (url)
- GitHub (url)

**Security:**
- Current Password (password, required)
- New Password (password)
- Confirm Password (password)

---

### Exercise 3.3: Build a Complex Multi-Step Form (As Single Page)
**Objective:** Practice advanced form structures

**Create a form for a fictional "Web App Signup":**

**Step 1: Account Type**
- Account type selection (radio: Personal, Business)
- Conditional fields based on selection

**Step 2: Personal Information**
- All personal info fields with validation
- Fieldsets for organization

**Step 3: Preferences**
- Multiple checkboxes and dropdowns
- Complex selection logic

**Step 4: Plan Selection**
- Radio buttons for pricing tiers
- Each with different features

**Step 5: Billing**
- Complete billing information
- Payment method options

**Step 6: Review & Confirm**
- Summary of all entered information
- Confirm checkbox (required)
- Submit button

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
- [ ] Tested all validation
- [ ] All forms are accessible
- [ ] All forms validate as HTML5

---

## ✅ Success Criteria

You've mastered HTML Forms when you can:

✅ Create functional HTML forms from scratch  
✅ Use all common form elements appropriately  
✅ Add proper labels for accessibility  
✅ Implement HTML5 validation  
✅ Organize forms with fieldsets  
✅ Create user-friendly forms  

---

## 🚀 Next Steps

1. Review the HTML projects
2. Start styling these forms with CSS
3. Eventually add JavaScript for advanced validation
4. Move to the CSS track!

---

