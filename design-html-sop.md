# 🎨 Developer SOP: HTML Design Standards

This SOP outlines best practices for writing HTML markup that is clean, semantic, accessible, SEO-friendly, and easy to maintain.

---

## 📁 1. HTML File Structure

- Always start with the HTML5 doctype:

  ```html
  <!DOCTYPE html>
Standard document structure:

html
Copy
Edit
<html lang="en">
  <head>
    <!-- Metadata and linking -->
  </head>
  <body>
    <!-- Page content -->
  </body>
</html>
Set appropriate language in <html lang="...">.

Use proper character encoding:

html
Copy
Edit
<meta charset="UTF-8">
🧱 2. Semantic HTML
Use semantic tags to describe content:
<header>, <footer>, <main>, <article>, <section>, <nav>, <aside>

Avoid excessive <div> or <span> nesting ("div soup").

Use headings <h1> to <h6> in a logical hierarchy (no skipping levels).

Use <button> for actions, <a> for navigation.

🧼 3. Clean & Maintainable Code
Proper indentation (2 or 4 spaces, consistent).

Use lowercase tag and attribute names.

Quote all attribute values:

html
Copy
Edit
<input type="text" name="username" />
Close all tags properly (especially in JSX or XHTML).

Organize sections with clear comments:

html
Copy
Edit
<!-- Header Section -->
<!-- Features Section -->
🌐 4. SEO Best Practices
Only one <h1> tag per page, describing the main topic.

Use relevant <title> and <meta description> in <head>.

Use alt attributes for all <img> tags.

Use descriptive text in anchor links:

html
Copy
Edit
<a href="/services">View our services</a>
♿ 5. Accessibility (a11y)
Always provide alt text for images.

Use semantic tags to help screen readers.

Use ARIA roles and labels when necessary:

html
Copy
Edit
<button aria-label="Close modal">✖</button>
Ensure keyboard navigability for all interactive elements.

Use label tags linked to form inputs:

html
Copy
Edit
<label for="email">Email:</label>
<input id="email" type="email" />
📱 6. Responsive Design Structure
Use the viewport meta tag:

html
Copy
Edit
<meta name="viewport" content="width=device-width, initial-scale=1.0">
Structure your layout using responsive containers and Flex/Grid.

Avoid fixed widths in HTML – let CSS handle layout.

Include mobile-first class structure (e.g., BEM, Tailwind, etc.).

🧩 7. Forms & Inputs
Wrap inputs in <form> tags.

Use appropriate type attributes:

type="email", type="tel", type="number", etc.

Include placeholder, required, and aria-* attributes when needed.

Group form fields with <fieldset> and <legend> when relevant.

⚙️ 8. Performance & Optimization
Use lazy loading on images:

html
Copy
Edit
<img src="image.webp" loading="lazy" alt="..." />
Avoid inline CSS/JS in HTML files.

Defer or async load non-critical scripts:

html
Copy
Edit
<script src="script.js" defer></script>
Use modern image formats (WebP, AVIF).

🎯 9. External Assets & Linking
Link to CSS and JS with proper paths and attributes:

html
Copy
Edit
<link rel="stylesheet" href="styles.css" />
<script src="main.js" defer></script>
Set rel="noopener noreferrer" on external links for security:

html
Copy
Edit
<a href="https://external.com" target="_blank" rel="noopener noreferrer">External</a>
🧾 10. Developer QA Checklist
Task	Status
Document uses HTML5 doctype and language attribute	✅/❌
All tags are semantically structured	✅/❌
Headings follow correct hierarchy	✅/❌
All images include descriptive alt text	✅/❌
Meta title and description are set and unique	✅/❌
All links are descriptive and accessible	✅/❌
Forms use proper labels and input types	✅/❌
HTML is W3C validated (validator.w3.org)	✅/❌
Page is mobile responsive and uses viewport meta	✅/❌
Scripts and styles are properly linked and deferred	✅/❌
No inline styles or scripts unless necessary	✅/❌
External links use rel="noopener noreferrer"	✅/❌
HTML is well-indented and commented	✅/❌
Keyboard navigation works across interactive elements	✅/❌

Last updated: 2025-07-24

yaml
Copy
Edit

---

📌 **To use**:  
1. Save the content above as a file: `design-html-sop.md`.  
2. Place it in your Git repo (e.g., in a `/docs/` folder).  
3. Link it from your main `README.md` like:

```md
- [HTML Design SOP](docs/design-html-sop.md)
