# 🎨 Developer SOP: HTML Design Standards

This SOP outlines best practices for writing HTML markup that is clean, semantic, accessible, SEO-friendly, and easy to maintain.

---

## 📁 1. HTML File Structure

- Always start with the HTML5 doctype:

  ```html
  <!DOCTYPE html>
•	Standard document structure:
html
CopyEdit
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Page Title</title>
  </head>
  <body>
    <!-- Page content -->
  </body>
</html>
•	Set appropriate language in the <html lang="..."> tag.
•	Use UTF-8 encoding with <meta charset="UTF-8">.
________________________________________
  ---
## 🧱 2. Semantic HTML
•	Use semantic tags:
html
CopyEdit
<header>, <footer>, <main>, <article>, <section>, <nav>, <aside>
•	Avoid excessive <div> or <span> nesting ("div soup").
•	Use heading tags <h1> to <h6> in a logical, hierarchical order.
•	Use:
o	<a> for navigation.
o	<button> for actions.
________________________________________
  ---
## 🧼 3. Clean & Maintainable Code
•	Use consistent indentation (2 or 4 spaces).
•	Use lowercase tag and attribute names.
•	Quote all attribute values:
html
CopyEdit
<input type="text" name="username" />
•	Close all tags properly.
•	Use comments to separate sections:
html
CopyEdit
<!-- Header Section -->
<!-- Main Content -->
________________________________________
## 🌐 4. SEO Best Practices
•	Only one <h1> tag per page (describes the main topic).
•	Use a relevant <title> and <meta name="description"> in the <head>.
•	All <img> elements should include alt attributes.
•	Anchor links must use meaningful text:
html
CopyEdit
<a href="/services">View our services</a>
________________________________________
## ♿ 5. Accessibility (a11y)
•	Provide descriptive alt text for all images.
•	Use semantic HTML to help screen readers.
•	Add ARIA roles/labels when needed:
html
CopyEdit
<button aria-label="Close modal">✖</button>
•	Ensure full keyboard accessibility.
•	Label form fields correctly:
html
CopyEdit
<label for="email">Email:</label>
<input id="email" type="email" />
________________________________________
## 📱 6. Responsive Design Structure
•	Add this in the <head> for responsiveness:
html
CopyEdit
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
•	Use responsive containers and layout with Flexbox/Grid.
•	Avoid fixed pixel widths in HTML (use CSS).
•	Build mobile-first with utility classes (BEM, Tailwind, etc.).
________________________________________
## 🧩 7. Forms & Inputs
•	Wrap form fields inside <form> tags.
•	Use appropriate type attributes like email, tel, number.
•	Add placeholder, required, and ARIA attributes where necessary.
•	Use <fieldset> and <legend> to group form sections logically.
________________________________________
## ⚙️ 8. Performance & Optimization
•	Enable lazy loading on images:
html
CopyEdit
<img src="image.webp" loading="lazy" alt="..." />
•	Avoid inline CSS and JavaScript.
•	Use defer or async for non-critical scripts:
html
CopyEdit
<script src="main.js" defer></script>
•	Use modern image formats like WebP or AVIF.
________________________________________
## 🎯 9. External Assets & Linking
•	Link stylesheets and scripts cleanly:
html
CopyEdit
<link rel="stylesheet" href="styles.css" />
<script src="main.js" defer></script>
•	For external links, always use:
html
CopyEdit
<a href="https://external.com" target="_blank" rel="noopener noreferrer">Visit Site</a>
________________________________________
## 🧾 10. Developer QA Checklist
Task	Status
HTML5 doctype and language attribute	✅ / ❌
All tags are semantically structured	✅ / ❌
Headings follow correct hierarchy	✅ / ❌
All images include descriptive alt text	✅ / ❌
Meta title and description are set and unique	✅ / ❌
Links are descriptive and accessible	✅ / ❌
Forms use proper labels and input types	✅ / ❌
HTML is W3C validated (https://validator.w3.org)
✅ / ❌
Page is responsive with viewport meta	✅ / ❌
Scripts and styles are properly linked and deferred	✅ / ❌
No inline styles or scripts unless necessary	✅ / ❌
External links use rel="noopener noreferrer"	✅ / ❌
HTML is cleanly indented and commented	✅ / ❌
Keyboard accessibility is verified	✅ / ❌
________________________________________
Last updated: 2025-07-24
yaml
CopyEdit

---

