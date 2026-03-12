# School of Tomorrow's AI - Living Brand Kit

A lightweight, interactive living brand guideline built with plain HTML, CSS, and vanilla JavaScript.
No build tools required.

## Overview

This repository is the official brand system reference for School of Tomorrow's AI.
It includes:

- a single-page guideline site (`index.html`)
- runtime design tokens in CSS (`styles.css`)
- design tokens in JSON (`tokens.json`)
- downloadable logo and pattern assets

The page is designed for both designers and developers, with copy-ready snippets and visual usage guidance.

## Repository Structure

| Path | Description |
|------|-------------|
| `index.html` | Brand kit page (sections 01-05) |
| `styles.css` | Tokens + layout + components + section-specific UI |
| `tokens.json` | Source token data for tooling/design pipelines |
| `favicon.svg` | Browser tab icon |
| `logos/` | Mark, vertical, and horizontal logo exports |
| `patterns/` | Pattern image exports (`pattern-1.png` ... `pattern-6.png`) |

## Live URLs

- Brand kit (GitHub Pages): [https://linalopes.github.io/SchoolAI-brand-kit/](https://linalopes.github.io/SchoolAI-brand-kit/)
- Pattern generator: [https://linalopes.github.io/SchoolAI-vignette-generator/](https://linalopes.github.io/SchoolAI-vignette-generator/)

## Local Development

No install step is needed.

1. Clone:
   ```bash
   git clone https://github.com/linalopes/SchoolAI-brand-kit.git
   cd SchoolAI-brand-kit
   ```
2. Serve locally (recommended):
   ```bash
   python -m http.server 8000
   ```
3. Open:
   [http://localhost:8000](http://localhost:8000)

## Design System Snapshot

### Core colors

| Name | Value | Semantic CSS var |
|------|-------|------------------|
| Deep Purple | `#22113E` | `--color-text` |
| Gray Green | `#CAD8D8` | `--color-surface` |
| Pink | `#EA7DFF` | `--color-primary` |
| Turquoise | `#08F2DB` | `--color-accent` |
| White | `#FFFFFF` | `--color-bg` |

### Fonts

| Role | Family | Weights |
|------|--------|---------|
| Title | Space Grotesk | 300, 500 |
| Body | Inter | 300, 600 |
| Mono/Highlight | Courier Prime | 400, 700 |

### Spacing and shape

- Spacing scale: `--space-1` to `--space-6` (`6px` to `52px`)
- Radius token: `--radius` (`4px`)
- Border width token: `--border-width` (`1px`)

## Page Sections

The brand page includes:

1. Logos (mark + lockups + usage examples)
2. Colors (editorial palette + approved contrast pairs)
3. Patterns (thumbnail grid + generator invite)
4. Typography (specimen + spacing scale)
5. Components (starter UI patterns)

## Token Sources

- Runtime CSS variables live in `styles.css` (`:root`).
- Portable token definitions live in `tokens.json`.

Use semantic tokens whenever possible instead of hardcoded values.

## License

This project is licensed under the [MIT License](LICENSE).

Note: while the code is open source, the School of Tomorrow's AI name and identity assets may be protected. If you fork this project, replace brand assets for public reuse.

## Contributing

Contributions are welcome.
Please read [CONTRIBUTING.md](CONTRIBUTING.md).
