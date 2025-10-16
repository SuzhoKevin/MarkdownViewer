# Markdown LaTeX Viewer

A single-page Markdown editor that renders equations with KaTeX in real time. Type Markdown mixed with LaTeX on the left and see the formatted preview—including math blocks, tables, and code—on the right.

## Features
- Live Markdown preview with GitHub-flavored Markdown support
- Automatic detection and wrapping of inline/block LaTeX expressions
- KaTeX-powered math rendering with copy, paste, and clear shortcuts
- Adjustable preview font size (persisted in `localStorage`) and print-friendly layout
- One-click print view for generating PDFs or paper copies

## Getting Started
1. Clone the repository
   ```bash
   git clone https://github.com/<your-username>/latex-viewer.git
   cd latex-viewer
   ```
2. Open `index.html` in your browser (double-click the file or use a local HTTP server).
3. Start editing the left-hand textarea—rendered output updates instantly on the right.

## Development Notes
- The app is framework-free and depends on CDN builds of [Marked](https://marked.js.org/) and [KaTeX](https://katex.org/).
- `normalizeMathInput` pre-processes pasted text to wrap likely LaTeX content with `$...$` or `$$...$$` before running Marked.
- When printing (`Cmd/Ctrl + P`), the interface hides the editor and reformats the preview for paper or PDF output.

## Roadmap Ideas
- Import/export Markdown files
- Configurable theme (light/dark/system)
- Custom KaTeX macros and macro presets

## License
Released under the [MIT License](LICENSE).
