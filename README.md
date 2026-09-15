# Redesign Studio v2

AI website audit, redesign & proposal tool.

Paste your website URL, select what you want to improve, and get:
- A scored audit across 6 dimensions (first impression, messaging, conversion, trust, mobile UX, SEO)
- An interactive HTML redesign concept (real code, not a mockup)
- A written proposal you can save as PDF

## Live site

Hosted on GitHub Pages: **https://slavomirhruska.github.io/redesign-studio-v2/**

## Tech

- Single-file HTML (self-contained, no build step)
- React 18 (CDN) for the interactive shell
- CSS custom properties for the design system
- Archivo font (WOFF2, subset)

## Development

No build step needed — open `index.html` directly in a browser, or serve with any static server:

```bash
python3 -m http.server 8000
```
