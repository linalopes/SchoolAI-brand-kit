# School of Tomorrow’s AI — Living Brand Kit (HTML/CSS)

This repository is a lightweight **living brand guideline** for **School of Tomorrow’s AI**:
colors, typography, logos, and generative patterns — all in a simple, copy-friendly HTML page.

It’s designed to be useful for both:
- **Designers** (HEX/RGB, font links, downloadable SVG assets)
- **Developers** (semantic CSS tokens, ready-to-copy snippets)

---

## What’s inside

- **`index.html`** — the brand landing page (manual)
- **`styles.css`** — design tokens + base components (buttons, cards, layout)
- **`logo-big.svg`** — primary logo (SVG)
- **`logo-horizontal.svg`** — horizontal lockup (SVG)
- **`pattern-*.svg`** — exported SVG patterns (optional / add as you generate)

Also includes a **live patterns preview** (lazy-loaded iframe) pointing to:
https://linalopes.github.io/SOTA-vignette-generator/

---

## Design tokens (quick overview)

Semantic tokens are the recommended way to use colors in UI:

- `--color-primary` (Pink)
- `--color-on-primary` (White)
- `--color-text` (Deep Purple)
- `--color-surface` (Gray Green)
- `--color-accent` (Turquoise)
- `--radius` is always `4px`

Typography:

- Titles: **Space Grotesk** (Light / Medium)
- Body: **Inter** (Light / SemiBold)
- Highlights: **Courier Prime** (Regular / Bold)

---

## How to run locally

No build step required.

1. Clone the repo
2. Open `index.html` in your browser

Optional (recommended): serve locally to avoid any browser restrictions around file URLs.

Example:

```bash
python -m http.server 8000
Then open:

http://localhost:8000

Updating the brand kit
Colors / tokens
Edit :root in styles.css to update tokens.
The UI reads values from CSS variables, so you usually won’t need to change HTML.

Logos
Replace or update:

logo-big.svg

logo-horizontal.svg

The page includes download links to these files.

Patterns (SVG)
Export your generated patterns as SVG and save in the project root, e.g.:

pattern-1.svg

pattern-2.svg

pattern-3.svg

The “Patterns” card includes download links for these files.

Notes for designers
Colors are shown with HEX + RGB and have copy buttons.

Fonts include Google Fonts links and guidance to use “Download family”.

Logos and patterns are delivered as SVG for maximum compatibility (Figma, Illustrator, Affinity, etc.).

License
Add your preferred license here (e.g. MIT / CC BY / proprietary).
If you want this to be private brand IP, write something like:

© School of Tomorrow’s AI. All rights reserved.
