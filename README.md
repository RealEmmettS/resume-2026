# resume-2026

A print-first HTML/CSS resume designed for US Letter (8.5" x 11") output.

## Preview

Open `index.html` in any browser to view the resume. The page is styled to match printed dimensions.

## Export to PDF

1. Open `index.html` in a browser
2. Press `Ctrl+P` (Windows) or `Cmd+P` (Mac)
3. Set destination to "Save as PDF"
4. Print

The `@media print` styles handle proper formatting automatically.

## Structure

```
├── index.html          # Resume content
├── styles.css          # Print-first stylesheet
├── fonts/              # Personal Vogue display font
└── PERSONAL_RESUME.pdf # Pre-rendered export
```

## Design

- **Typography**: Personal Vogue (headings) + Source Sans 3 (body)
- **Layout**: Two-column grid with experience on left, skills/education on right
- **Colors**: Navy and warm neutral palette