# eduardosanti.dev — portfolio source

Static site, no build step. Dark mode, Swift-orange accent, system SF font stack.

## Files
- `index.html` — all content (hero, case studies, writing, about, footer)
- `style.css` — all styling
- `script.js` — mobile nav toggle only


## Editing content later
- All text lives directly in `index.html` — case studies are in `<article class="case">` blocks.
- Colors and fonts are CSS variables at the top of `style.css` under `:root` — change once, applies everywhere.

## Browser support
Uses CSS flexbox `gap`, `backdrop-filter`, and `<details>` — all standard in
Safari, Chrome, Firefox, and Edge since 2021. No polyfills needed.
