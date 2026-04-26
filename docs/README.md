# AI Quick Translate — Public Site

This folder is published as a static site via GitHub Pages.

## Files

| File | Purpose |
|---|---|
| `index.html` | Landing page (hero, features, use cases, screenshots, languages, FAQ) |
| `privacy.html` | Privacy Policy |
| `terms.html` | Terms & Conditions |
| `404.html` | Soft-error page |
| `sitemap.xml` | XML sitemap for search engines |
| `robots.txt` | Crawler directives + sitemap pointer |
| `manifest.webmanifest` | PWA manifest (app metadata) |
| `humans.txt` | Friendly site credits |
| `assets/style.css` | Shared styles |
| `assets/app-logo.svg` | Brand logo |
| `assets/favicon.png` | Browser favicon |
| `assets/og-image.png` | 1200×630 social preview image |
| `assets/screenshots/*.jpg` | App screenshots (optimized) |
| `.nojekyll` | Disables Jekyll so files starting with `_` serve as-is |

## Enable GitHub Pages

1. Push this folder to `main`.
2. On GitHub: **Settings → Pages**.
3. **Source**: `Deploy from a branch`.
4. **Branch**: `main`, **Folder**: `/docs`.
5. Save. The site will be available at:
   `https://umarnisar1.github.io/-Image-PDF-Translator-Pro/`

The Privacy Policy URL to paste into the Google Play Console:
`https://umarnisar1.github.io/-Image-PDF-Translator-Pro/privacy.html`

## SEO checklist (already in place)

- ✅ Unique `<title>` and meta description per page
- ✅ Canonical URLs on every page
- ✅ Open Graph + Twitter Card with 1200×630 image
- ✅ JSON-LD structured data: `Organization`, `WebSite`, `MobileApplication`, `FAQPage`, `PrivacyPolicy`, `WebPage`, `BreadcrumbList`
- ✅ Semantic HTML: `<header>`, `<main>`, `<nav>`, `<article>`, `<section>`, `<figure>`
- ✅ Heading hierarchy (one `<h1>` per page)
- ✅ Skip-to-content link for accessibility
- ✅ Explicit `width`/`height` on all images (no CLS)
- ✅ `loading="lazy"` + `decoding="async"` on below-fold images
- ✅ JPEG-compressed screenshots (~50KB each, down from ~1.3MB)
- ✅ `preconnect` and `preload` for critical resources
- ✅ Mobile-friendly viewport
- ✅ `robots.txt` + `sitemap.xml`
- ✅ PWA manifest
- ✅ FAQ section with `FAQPage` schema (eligible for SERP rich results)
- ✅ 404 page with `noindex`
- ✅ `aria-label` on icon buttons and navs
- ✅ `alt` text on every meaningful image
- ✅ `theme-color` for mobile browser chrome

## Post-launch SEO actions (do these once Pages is live)

1. **Google Search Console**
   - Add property: `https://umarnisar1.github.io/-Image-PDF-Translator-Pro/`
   - Verify via HTML tag (paste into `<head>` of `index.html`) or DNS
   - Submit `sitemap.xml`
   - Request indexing for `/`, `/privacy.html`, `/terms.html`

2. **Bing Webmaster Tools**
   - Add the same property and submit the sitemap

3. **Test rich results**
   - Run https://search.google.com/test/rich-results on each page
   - Run https://www.linkedin.com/post-inspector/ and https://cards-dev.twitter.com/validator for OG/Twitter previews
   - Run https://search.google.com/search-console/mobile-friendly

4. **Performance audit**
   - Run https://pagespeed.web.dev/ — should score 95+ on mobile

5. **Backlinks (long-tail organic)**
   - Add the GitHub repo description with a link to the Pages site
   - Cross-link from Google Play listing (developer website field)
   - Submit to free Android app directories (e.g., AlternativeTo, ProductHunt, AppAgg)
   - Post on r/androidapps, r/translator with a "made this" angle

## Updating

Edit the HTML files directly — no build step required. Update the `Last updated`
date inside each legal page when changing its content, and update `<lastmod>`
in `sitemap.xml` for the corresponding URL.
