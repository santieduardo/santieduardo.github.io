# eduardosanti.dev — portfolio source

Static site, no build step. Dark mode, Swift-orange accent, system SF font stack.

## Files
- `index.html` — all content (hero, case studies, writing, about, footer)
- `style.css` — all styling
- `script.js` — mobile nav toggle only
- `assets/` — put your profile photo / any images here if you add them

## Deploy to GitHub Pages (your existing santieduardo.github.io repo)

1. Copy `index.html`, `style.css`, and `script.js` into the root of your
   `santieduardo.github.io` repo, replacing the old files.
2. Commit and push:
   ```
   git add .
   git commit -m "Redesign portfolio"
   git push
   ```
3. GitHub Pages will rebuild automatically (usually within a minute).
   Check it live at https://santieduardo.github.io/

No Jekyll config, no dependencies, no build tools required — it's plain HTML/CSS/JS.

## Editing content later
- All text lives directly in `index.html` — case studies are in `<article class="case">` blocks.
- Colors and fonts are CSS variables at the top of `style.css` under `:root` — change once, applies everywhere.
- To add a photo: drop it in `assets/`, then reference it in the `.hero` section of `index.html` if you want a headshot.

## Browser support
Uses CSS flexbox `gap`, `backdrop-filter`, and `<details>` — all standard in
Safari, Chrome, Firefox, and Edge since 2021. No polyfills needed.
