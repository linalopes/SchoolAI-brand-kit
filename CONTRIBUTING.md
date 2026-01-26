# Contributing to School of Tomorrow's AI — Living Brand Kit

Thank you for your interest in contributing! This document provides guidelines for contributing to this project.

## How to Contribute

### Reporting Issues

- Use [GitHub Issues](../../issues) to report bugs or suggest features
- Search existing issues before creating a new one
- Provide clear, descriptive titles
- Include steps to reproduce for bug reports

### Submitting Changes

1. **Fork** the repository
2. **Create a branch** for your changes:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Make your changes** following the style guidelines below
4. **Test** your changes locally by opening `index.html` in a browser
5. **Commit** with a clear, descriptive message:
   ```bash
   git commit -m "Add: description of your change"
   ```
6. **Push** to your fork and submit a **Pull Request**

### Pull Request Guidelines

- Reference any related issues in your PR description
- Keep PRs focused on a single change
- Ensure all links and assets work correctly
- Test on multiple browsers if possible

## Style Guidelines

### CSS

- Use CSS custom properties (variables) from `:root` for colors, fonts, and spacing
- Follow the existing naming conventions (e.g., `.button--primary`, `.card`)
- Keep selectors simple and avoid deep nesting
- Add comments for non-obvious styles

### HTML

- Use semantic HTML5 elements
- Maintain consistent indentation (2 spaces)
- Include appropriate ARIA labels for accessibility
- Use relative paths for all assets (e.g., `./styles.css`)

### File Naming

- Use lowercase with hyphens: `logo-horizontal.svg`
- Pattern files: `pattern-1.svg`, `pattern-2.svg`, etc.
- Keep names descriptive but concise

### Brand Consistency

- Stick to the defined color palette
- Use only the specified fonts (Space Grotesk, Inter, Courier Prime)
- Maintain the `4px` border radius (`--radius`)

## Questions?

Feel free to open an issue if you have questions or need clarification.
