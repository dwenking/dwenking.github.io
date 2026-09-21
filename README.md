# dwenking.github.io

Hand-written static site, no build step, no dependencies.

- `index.html` – the whole page: receipt, career card, pinned cards, popover details
- `style.css` – all styles; bump the `?v=` on the `<link>` in index.html after editing so browsers refetch
- `img/profile-4x3.png` – 1-bit dithered portrait (regenerate with Pillow: crop 4:3, resize 400×300, autocontrast, `.convert('1')`)
- `attaches/` – paper PDFs

Preview locally: `python3 -m http.server 8000` in the repo root, then open http://localhost:8000/ (hard-refresh with ⌘⇧R to bypass the CSS cache).

Edit, commit, push to `master`. GitHub Pages deploys it.
