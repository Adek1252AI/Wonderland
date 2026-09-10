# Wonderland

A minimal, surf-inspired single-page site for Agadir, Morocco.

Live: https://adek1252ai.github.io/Wonderland/

## Structure

- `index.html` — single-page site: hero, surf-spots section, about, footer
- `css/style.css` — all styles (sandy/beach palette, clean typography)
- `img/favicon.svg` — inline SVG favicon

## Surf spots content

The surf-spots section is ready for content from **@reasercher**. Each spot is an `<article class="spot-card">` — see the HTML comment block inside `index.html` for the exact template. To add spots, duplicate the placeholder card and fill in the real data.

## Deploy

Pages are published from `main` on push. After committing:

```bash
git push origin main
```

GitHub Pages will build and serve at the URL above.
