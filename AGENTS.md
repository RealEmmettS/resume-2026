# Repository Guidelines

## Project Structure & Module Organization

- `index.html` holds the resume content with semantic sections (header, main, sidebar).
- `styles.css` contains the print-first layout, typography, and responsive rules.
- `fonts/` stores the local Personal Vogue font files used by the stylesheet.
- `PERSONAL_RESUME.pdf` is the exported, print-ready snapshot of the resume.
- `README.md` and `CLAUDE.md` document usage and design decisions.

## Build, Test, and Development Commands

This is a static HTML/CSS project, so there is no build step.

- Preview locally (Windows): `start index.html`
- Preview via local server (optional): `python -m http.server` then open `http://localhost:8000/index.html`
- Export PDF: open `index.html`, print to PDF (Ctrl+P / Cmd+P) and save over `PERSONAL_RESUME.pdf`

## Coding Style & Naming Conventions

- Indentation: 2 spaces for HTML and CSS.
- Class names: lowercase kebab-case (e.g., `contact-item`, `section-title`).
- Prefer semantic HTML with minimal wrappers; keep the two-column structure intact.
- Use CSS custom properties in `:root` for palette and sizing to preserve consistency.
- Maintain print-first behavior; update `@media print` rules when layout changes.

## Testing Guidelines

There are no automated tests. Manually verify:
- Screen rendering in a modern browser.
- Print preview matches US Letter (8.5" x 11") and margins.
- PDF output is updated when content or styles change.

## Commit & Pull Request Guidelines

- Commit messages in history are short, imperative statements (e.g., "Add files via upload"). Keep them concise and present-tense.
- PRs should describe layout or content changes and include a screenshot or PDF preview if visuals are affected.
- If `index.html` or `styles.css` changes, regenerate and commit `PERSONAL_RESUME.pdf`.

## Assets & External Dependencies

- Local fonts live under `fonts/` and are referenced via `@font-face` in `styles.css`.
- Body text uses Source Sans 3 from Google Fonts; keep network dependencies minimal.
