<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Form</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="contact-form-container">
        <form action="mailto:hims9596@gmail.com" method="POST" enctype="text/plain" class="contact-form">
            <h2 class="form-title">Enquire Now</h2>
            <p class="form-subtitle">Get 100% Free Counseling</p>

            <!-- Name -->
            <label for="name" class="icon-label">👤 Name *</label>
            <input type="text" id="name" name="name" placeholder="Enter Your Name" required>

            <!-- Contact Number -->
            <label for="contact" class="icon-label">📱 Phone *</label>
            <div class="contact-input-wrapper">
                <span class="flag-icon">🇮🇳</span>
                <input type="tel" id="contact" name="contact" placeholder="Enter Your Number" required>
            </div>

            <!-- Email -->
            <label for="email" class="icon-label">✉ Email *</label>
            <input type="email" id="email" name="email" placeholder="Enter Your Mail ID" required>

            <!-- Course -->
            <label for="course" class="icon-label">📚 Course *</label>
            <select id="course" name="course" required>
                <option value="" disabled selected>Select Your Course</option>
                <option value="Engineering">Engineering</option>
                <option value="Management">Management</option>
                <option value="Arts">Arts</option>
                <option value="Science">Science</option>
            </select>

            <!-- State -->
            <label for="state" class="icon-label">📍 State *</label>
            <select id="state" name="state" required>
                <option value="" disabled selected>Select Your State</option>
                <option value="Andhra Pradesh">Andhra Pradesh</option>
                <option value="Maharashtra">Maharashtra</option>
                <option value="Karnataka">Karnataka</option>
                <option value="Delhi">Delhi</option>
                <option value="Tamil Nadu">Tamil Nadu</option>
            </select>

            <!-- Consent Checkbox -->
            <label class="checkbox-container">
                <input type="checkbox" id="consent" name="consent" required>
                Get Universities Discount Offers in Your Inbox.
            </label>

            <!-- Submit Button -->
            <button type="submit" class="submit-button">Submit</button>
        </form>
    </div>
</body>
</html>
---
title: Form styling
lang: en-US
---

# Form styling

With Formspark you get to bring your own HTML and CSS.

On this page you'll find tips, tricks and links to help you style your forms.

## Simple vertical layout

![Simple vertical layout](../.vuepress/public/simple-vertical-layout.png)

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <style>
      .vertical-form {
        display: flex;
        flex-direction: column;
        gap: 0.5rem;
        max-width: 500px;
      }
    </style>
  </head>
  <body>
    <form class="vertical-form" action="https://submit-form.com/your-form-id">
      <label for="first-name">First name</label>
      <input id="first-name" name="first-name" type="text" />
      <label for="last-name">Last name</label>
      <input id="last-name" name="last-name" type="text" />
      <label for="message">Message</label>
      <textarea id="message" name="message" cols="15" rows="5"></textarea>
      <button type="submit">Submit</button>
    </form>
  </body>
</html>
```

## Add an asterisk to required field labels

![Required field label asterisk](../.vuepress/public/required-field-label-asterisk.png)

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <style>
      label.required:after {
        content: "*";
        color: red;
      }
    </style>
  </head>
  <body>
    <form action="https://submit-form.com/your-form-id">
      <label for="first-name" class="required">First name</label>
      <input id="first-name" name="first-name" type="text" required />
      <label for="last-name">Last name</label>
      <input id="last-name" name="last-name" type="text" />
      <button type="submit">Submit</button>
    </form>
  </body>
</html>
```

## CSS frameworks

- [Bootstrap](https://getbootstrap.com/)
- [Milligram](https://milligram.io/)
- [Tailwind CSS](https://tailwindcss.com/)
