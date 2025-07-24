🎨 Developer SOP: HTML Design Standards
This SOP outlines best practices for writing HTML that is clean, semantic, accessible, SEO-friendly, and easy to maintain.
________________________________________
📁 1. HTML File Structure
•	Always start with the HTML5 doctype:
html
CopyEdit
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
•	Use UTF-8 encoding: <meta charset="UTF-8">.
________________________________________
🧱 2. Semantic HTML
•	Use semantic tags:
html
CopyEdit
<header>, <footer>, <main>, <article>, <section>, <nav>, <aside>
•	Avoid unnecessary <div> or <span> nesting ("div soup").
•	Use headings <h1> to <h6> in a logical, hierarchical order.
•	Use:
o	<a> for navigation.
o	<button> for actions.
________________________________________
🧼 3. Clean & Maintainable Code
•	Use consistent indentation (2 or 4 spaces).
•	Use lowercase for tag and attribute names.
•	Quote all attribute values:
html
CopyEdit
<input type="text" name="username" />
•	Close all tags properly.
•	Use clear section comments:
html
CopyEdit
<!-- Header Section -->
<!-- Main Content -->
________________________________________
🌐 4. SEO Best Practices
•	Only one <h1> tag per page (main topic).
•	Use relevant <title> and <meta name="description"> tags in the <head>.
•	All <img> elements should include descriptive alt attributes.
•	Use meaningful link text:
html
CopyEdit
<a href="/services">View our services</a>
________________________________________
♿ 5. Accessibility (a11y)
•	Provide descriptive alt text for all images.
•	Use semantic tags to assist screen readers.
•	Add ARIA roles/labels as needed:
html
CopyEdit
<button aria-label="Close modal">✖</button>
•	Ensure full keyboard navigation.
•	Label form fields properly:
html
CopyEdit
<label for="email">Email:</label>
<input id="email" type="email" />
________________________________________
📱 6. Responsive Design Structure
•	Include this meta tag in the <head>:
html
CopyEdit
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
•	Use responsive containers with Flexbox or Grid.
•	Avoid fixed pixel widths; handle layout in CSS.
•	Build mobile-first using utility classes (e.g., BEM, Tailwind).
________________________________________
🧩 7. Forms & Inputs
•	Wrap fields in <form> tags.
•	Use appropriate type attributes: email, tel, number, etc.
•	Use placeholder, required, and ARIA attributes as needed.
•	Group related fields with <fieldset> and <legend>.
________________________________________
⚙️ 8. Performance & Optimization
•	Enable lazy loading for images:
html
CopyEdit
<img src="image.webp" loading="lazy" alt="..." />
•	Avoid inline CSS/JS when possible.
•	Use defer or async for non-critical scripts:
html
CopyEdit
<script src="main.js" defer></script>
•	Prefer modern image formats: WebP, AVIF.
________________________________________
🎯 9. External Assets & Linking
•	Link stylesheets and scripts cleanly:
html
CopyEdit
<link rel="stylesheet" href="styles.css" />
<script src="main.js" defer></script>
•	For external links, always include security attributes:
html
CopyEdit
<a href="https://external.com" target="_blank" rel="noopener noreferrer">Visit Site</a>
________________________________________
🧾 10. Developer QA Checklist
Task	Status
HTML5 doctype and language attribute	✅ / ❌
All tags are semantically structured	✅ / ❌
Headings follow correct hierarchy	✅ / ❌
All images include descriptive alt text	✅ / ❌
Meta title and description are set and unique	✅ / ❌
Links are descriptive and accessible	✅ / ❌
Forms use proper labels and input types	✅ / ❌
HTML is W3C validated (validator.w3.org)
✅ / ❌
Page is responsive with viewport meta	✅ / ❌
Scripts and styles are properly linked and deferred	✅ / ❌
No inline styles or scripts unless necessary	✅ / ❌
External links use rel="noopener noreferrer"	✅ / ❌
HTML is cleanly indented and commented	✅ / ❌
Keyboard accessibility is verified	✅ / ❌
________________________________________
Last updated: 2025-07-24

