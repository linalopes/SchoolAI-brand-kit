# School of Tomorrow's AI — Living Brand Kit

A lightweight, interactive **living brand guideline** built with HTML, CSS, and vanilla JavaScript. No build tools required.

## What is this?

This repository contains the official brand kit for **School of Tomorrow's AI** — a single-page reference for colors, typography, logos, and generative patterns. Everything is copy-friendly and designed for both designers and developers.

## What's included

| File | Description |
|------|-------------|
| `index.html` | The brand landing page with interactive components |
| `styles.css` | Design tokens + base components (buttons, cards, layout) |
| `tokens.json` | Design tokens in JSON format for tooling integration |
| `logo-big.svg` | Primary logo (circular) |
| `logo-horizontal.svg` | Horizontal lockup |
| `favicon.svg` | Browser favicon |
| `pattern-*.svg` | Exported SVG patterns (add as you generate) |

## Live Demo

**GitHub Pages:** [https://linalopes.github.io/SOTA-brand-kit/](https://linalopes.github.io/SOTA-brand-kit/)

The site also includes a lazy-loaded iframe preview of the [SOTA Vignette Generator](https://linalopes.github.io/SOTA-vignette-generator/) for creating custom patterns.

## Run Locally

No build step required.

1. Clone the repository:
   ```bash
   git clone https://github.com/linalopes/SOTA-brand-kit.git
   cd SOTA-brand-kit
   ```

2. Open `index.html` directly in your browser, or serve locally to avoid file:// restrictions:
   ```bash
   # Python 3
   python -m http.server 8000
   
   # Node.js (if you have npx)
   npx serve .
   
   # PHP
   php -S localhost:8000
   ```

3. Visit [http://localhost:8000](http://localhost:8000)

## Deploy on GitHub Pages

1. Go to your repository **Settings** → **Pages**
2. Under "Build and deployment", select:
   - **Source:** Deploy from a branch
   - **Branch:** `main` (or `master`) / `/ (root)`
3. Click **Save**
4. Your site will be live at `https://<username>.github.io/<repo-name>/`

## Exporting & Adding Pattern SVGs

1. Use the [SOTA Vignette Generator](https://linalopes.github.io/SOTA-vignette-generator/) to create patterns
2. Export as SVG for crisp, scalable graphics
3. Save files in the project root with naming convention:
   ```
   pattern-1.svg
   pattern-2.svg
   pattern-3.svg
   ```
4. The Patterns section in `index.html` includes download links for `pattern-1.svg` through `pattern-3.svg`

## Notes for Designers

### Colors

| Name | HEX | RGB | CSS Variable |
|------|-----|-----|--------------|
| Deep Purple | `#22113E` | `rgb(34, 17, 62)` | `--color-text` |
| Gray Green | `#CAD8D8` | `rgb(202, 216, 216)` | `--color-surface` |
| Pink | `#EA7DFF` | `rgb(234, 125, 255)` | `--color-primary` |
| Turquoise | `#08F2DB` | `rgb(8, 242, 219)` | `--color-accent` |
| White | `#FFFFFF` | `rgb(255, 255, 255)` | `--color-bg` |

### Typography

| Role | Font | Weights | Google Fonts |
|------|------|---------|--------------|
| Titles | Space Grotesk | 300 (Light), 500 (Medium) | [Link](https://fonts.google.com/specimen/Space+Grotesk) |
| Body | Inter | 300 (Light), 600 (SemiBold) | [Link](https://fonts.google.com/specimen/Inter) |
| Highlights | Courier Prime | 400 (Regular), 700 (Bold) | [Link](https://fonts.google.com/specimen/Courier+Prime) |

**Tip:** Use "Download family" on Google Fonts to get font files for Figma, Illustrator, or Affinity Designer.

### Assets

- Logos and patterns are delivered as **SVG** for maximum compatibility
- All assets have download buttons on the brand kit page
- Shape radius is always `4px` (`--radius`)

## Notes for Developers

### Semantic Tokens

Use semantic color tokens instead of raw values:

```css
/* Recommended */
color: var(--color-text);
background: var(--color-surface);

/* Avoid */
color: #22113E;
background: #CAD8D8;
```

### Available CSS Variables

```css
/* Colors */
--color-bg          /* Background (white) */
--color-text        /* Text/ink (deep purple) */
--color-surface     /* Surface (gray green) */
--color-primary     /* Primary action (pink) */
--color-on-primary  /* Text on primary (white) */
--color-accent      /* Accent (turquoise) */

/* Typography */
--font-title        /* Space Grotesk */
--font-text         /* Inter */
--font-mono         /* Courier Prime */

/* Spacing scale */
--space-1 through --space-6

/* Shape */
--radius            /* 4px */
```

### Component Classes

```html
<button class="button">Default</button>
<button class="button button--primary">Primary</button>
<button class="button button--accent">Accent</button>
<span class="badge">Badge text</span>
```

## License

This project is licensed under the [MIT License](LICENSE).

**Note:** While the code is open source, the **School of Tomorrow's AI** brand name, logos, and visual identity may be protected trademarks. If you fork or adapt this project, please replace the brand assets with your own.

## Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## Code of Conduct

This project follows the [Contributor Covenant Code of Conduct](CODE_OF_CONDUCT.md).
