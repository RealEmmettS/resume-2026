# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static HTML/CSS resume website with a print-first, editorial design. The resume is designed to render as a standard US Letter (8.5" x 11") page and can be printed directly to PDF using the browser's print function.

## Architecture

- **index.html** - Single-page resume with semantic HTML structure (header, main content, sidebar)
- **styles.css** - Print-first stylesheet using CSS custom properties, grid layout, and media queries
- **fonts/** - Custom "Personal Vogue" display font (woff/woff2 formats)
- **PERSONAL_RESUME.pdf** - Pre-rendered PDF export

## Design System

The stylesheet uses CSS custom properties defined in `:root`:
- **Colors**: Navy/warm neutral palette (`--navy-deep`, `--charcoal`, `--warm-gray`, etc.)
- **Typography**: "Personal Vogue" for headings, "Source Sans 3" for body text
- **Layout**: Fixed 8.5" x 11" page container with two-column grid (1fr / 0.42fr)

## Generating PDF

To update the PDF, open `index.html` in a browser and use Print (Ctrl+P / Cmd+P) with "Save as PDF" destination. The `@media print` styles automatically adjust sizing for letter-sized output.

## Key CSS Sections

- **Lines 27-72**: CSS custom properties (colors, typography, spacing)
- **Lines 103-112**: Page container sizing
- **Lines 193-206**: Two-column grid layout
- **Lines 464-579**: Print-specific overrides
- **Lines 585-623**: Mobile responsive fallback
