# ✅ Developer SOP for SEO Ranking

---

## 📁 1. Project Setup

- Use a clean and lightweight codebase.
- Use semantic HTML5 elements (`<article>`, `<section>`, `<header>`, etc.).
- Implement a mobile-first responsive design.
- Enable HTTPS with a valid SSL certificate.
- Use a modern CSS framework or utility-first CSS (e.g., Tailwind) for maintainability.
- Avoid unused libraries and dependencies.

---

## 🧱 2. URL Structure & Routing

- Ensure clean, readable, SEO-friendly URLs (e.g., `/about-us`, not `/page?id=123`).
- Use hyphens (`-`) instead of underscores (`_`) in URLs.
- Avoid unnecessary URL parameters.
- Ensure consistent trailing slash or non-trailing slash policy.
- Set up proper **301 redirects** for any changed or removed URLs.
- Use **canonical URLs** to avoid duplicate content issues.
- Avoid dynamic URLs where possible, or ensure proper canonicalization.

---

## 🗺️ 3. Site Architecture & Navigation

- Follow a logical, shallow site structure (**3-click rule**).
- Create an **HTML sitemap** for users.
- Create an **XML sitemap** for search engines (auto-generated and auto-updated).
- Ensure breadcrumbs are implemented using **structured data**.
- Avoid orphan pages (ensure all content is linked internally).
- Use a consistent global navigation menu and footer.

---

## ⚙️ 4. Meta & Head Elements

- Title tag dynamically populated, unique per page, under 60 characters.
- Meta description unique, relevant, under 160 characters.
- Use `meta robots` tag correctly (`index, follow` or `noindex, nofollow` where needed).
- Include **Open Graph** and **Twitter Card** tags for social sharing.
- Use `<link rel="alternate" hreflang="x">` for multilingual support.
- Add favicon and theme-color meta tag.

---

## 🏎️ 5. Page Speed Optimization

- Minify CSS, JavaScript, and HTML.
- Enable **GZIP or Brotli compression**.
- Optimize and serve next-gen images (WebP, AVIF).
- Lazy load all non-critical images and iframes.
- Use a **Content Delivery Network (CDN)**.
- Eliminate render-blocking resources (async/defer scripts).
- Use HTTP/2 or HTTP/3.
- Apply browser caching for static assets.

---

## 🔍 6. Indexing & Crawlability

- Implement `robots.txt` with correct rules and disallowed paths.
- Use `<link rel="canonical">` on all pages.
- Fix broken links (404s).
- Handle soft 404s and server error pages correctly (custom 404 with helpful nav/search).
- Avoid duplicate content through canonical tags or 301 redirects.
- Use structured data (Schema.org) for:
  - Articles
  - Products
  - Breadcrumbs
  - FAQs
  - Events
  - Local business (if applicable)
- Submit XML sitemap to Google Search Console and Bing Webmaster Tools.

---

## 📱 7. Mobile Optimization

- Ensure all pages are fully responsive.
- Avoid intrusive interstitials/popups on mobile.
- Use proper viewport settings (`<meta name="viewport" content="width=device-width, initial-scale=1">`).
- Test with Google Mobile-Friendly Test.
- Optimize tap targets and font sizes.

---

## 🔗 8. Internal Linking

- Use contextual, descriptive anchor text (no “click here”).
- Avoid broken internal links.
- Avoid deep linking chains (keep important content near the root).
- Limit total number of links per page (100–150 max is ideal).
- Include breadcrumbs and navigation links where appropriate.

---

## 🧾 9. Analytics & Tracking

- Install **Google Analytics (GA4)**.
- Install **Google Tag Manager (GTM)**.
- Verify and connect **Google Search Console** and **Bing Webmaster Tools**.
- Set up conversion goals and events tracking.
- Submit the **XML sitemap** to GSC and resubmit after major changes.

---

## 🌐 10. Localization (if applicable)

- Use `hreflang` tags for multilingual/multiregional sites.
- Ensure localized URLs (e.g., `/en/`, `/fr/`) are correctly structured.
- Set proper language meta tags (`<html lang="en">`).
- Avoid content duplication between language versions.

---

## 📦 11. CMS/Platform-Specific Adjustments

- **WordPress**:
  - Use SEO-friendly themes and plugins (e.g., **Yoast SEO**, **Rank Math**).
  - Disable default archives and tag pages if not used.
  - Optimize permalinks.
- **React / SPAs**:
  - Implement **Server-Side Rendering (SSR)** or **Static Site Generation (SSG)**.
  - Use pre-rendering or hydration strategies for crawlable pages.
  - Implement dynamic meta tags (e.g., with React Helmet).
- **Shopify**:
  - Use lightweight, optimized themes.
  - Minimize apps/scripts and defer non-critical ones.
  - Customize meta titles/descriptions via the CMS or liquid templates.

---

## 📊 12. Core Web Vitals (UX Signals)

- **LCP (Largest Contentful Paint)** < 2.5s.
- **CLS (Cumulative Layout Shift)** < 0.1.
- **INP (Interaction to Next Paint)** < 200ms.
- Use Google Lighthouse, PageSpeed Insights, or Web Vitals library.
- Preload critical assets and fonts.
- Avoid layout shifts by reserving space for media.

---

## 🧠 13. JavaScript SEO

- Ensure Googlebot can crawl JavaScript-rendered content.
- Use `<noscript>` fallback for critical features (if possible).
- Avoid blocking resources in `robots.txt`.
- Use tools like Google's Mobile-Friendly & Render Tests.
- Dynamically insert metadata using SSR or hydration.

---

## 🛡️ 14. Accessibility & Security

- Follow [WCAG 2.1 AA](https://www.w3.org/WAI/standards-guidelines/wcag/) standards.
- Use semantic HTML and ARIA roles where necessary.
- Ensure all images have descriptive `alt` tags.
- Keyboard navigation and focus states enabled.
- Implement Content Security Policy (CSP).
- Avoid mixed content issues.

---

## 🧑‍💻 SOP Final Checklist (Developer QA)

| Task                                                  | Status |
|-------------------------------------------------------|--------|
| All pages use unique title and meta tags              | ✅  |
| Pages load in <3 seconds                              | ✅  |
| Mobile responsive tested on all major devices         | ✅  |
| No critical errors in Search Console                  | ✅  |
| Sitemap and robots.txt configured correctly           | ✅  |
| Structured data passes Google’s Rich Results test     | ✅  |
| Core Web Vitals pass (LCP, CLS, INP)                  | ✅  |
| No broken internal or external links                  | ✅  |
| Custom 404 page implemented                           | ✅  |
| JavaScript content is crawlable and rendered properly | ✅  |
| hreflang and lang attributes set correctly            | ✅  |
| Analytics and tracking verified                       | ✅  |
| SSL certificate valid and enforced (HTTPS)            | ✅  |
| Alt attributes and ARIA roles validated               | ✅  |

---

> **Last updated**: `2025-07-24`
