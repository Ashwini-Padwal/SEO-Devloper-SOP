# 🎨 Developer SOP: HTML Design Standards

This SOP outlines best practices for writing HTML markup that is clean, semantic, accessible, SEO-friendly, and easy to maintain.

---

## 📁 1. HTML File Structure

- Always start with the HTML5 doctype:

  ```html
  <!DOCTYPE html>
```
- Standard document structure

```bash
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
```
- Set appropriate language in the <html lang="..."> tag.
- Use proper character encoding with <meta charset="UTF-8">.

  ## 🧱 2. Semantic HTML
- Use semantic tags to describe content:
```bash
<header>, <footer>, <main>, <article>, <section>, <nav>, <aside>
```
- Avoid excessive <div> or <span> nesting ("div soup").

- Use headings <h1> to <h6> in a logical hierarchy (do not skip levels).

- Use:

-- <a> for navigation links.

-- <button> for actions.
