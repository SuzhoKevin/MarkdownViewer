# Chat2PDF

A modern, single-page Markdown editor that renders equations with KaTeX in real time. Paste ChatGPT conversations or other AI chat transcripts on the left, tweak the Markdown if needed, and see the formatted preview—including math blocks, tables, and code—on the right before exporting to PDF.

## Demo
- https://chat2pdf.net

## Features
- **ChatGPT conversation paste-in workflow** with automatic Markdown/LaTeX normalization
- **Live Markdown preview** with GitHub-flavored Markdown support
- **Automatic detection and wrapping** of inline/block LaTeX expressions
- **KaTeX-powered math rendering** for beautiful mathematical equations
- **Editor toolbar** with copy, paste, and clear shortcuts
- **Adjustable preview font size** (persisted in `localStorage`)
- **Dark mode support** with automatic theme persistence
- **Modern UI design** with clean, professional styling
- **Privacy policy** modal with transparent data handling information
- **One-click print view** for generating PDFs or paper copies
- **Fully client-side** - no server required, all processing happens in your browser

## Getting Started
1. Clone the repository
   ```bash
   git clone https://github.com/SuzhoKevin/MarkdownViewer.git
   cd MarkdownViewer
   ```
2. Open `index.html` in your browser (double-click the file or use a local HTTP server).
3. Start editing the left-hand textarea—rendered output updates instantly on the right.

## User Interface

### Header Controls
- **Theme Toggle** - Switch between light and dark modes
- **Font Size Controls** - Adjust preview text size (A- / A+)
- **Print Button** - Generate PDF or print the preview

### Editor Toolbar
- **Copy** - Copy editor content to clipboard
- **Paste** - Paste content from clipboard
- **Clear** - Clear the editor

### Footer
- **Privacy Policy** - View privacy and data handling information
- **GitHub** - Link to the open-source repository

## Development Notes
- The app is framework-free and depends on CDN builds of [Marked](https://marked.js.org/) and [KaTeX](https://katex.org/).
- `normalizeMathInput` pre-processes pasted text to wrap likely LaTeX content with `$...$` or `$$...$$` before running Marked.
- When printing (`Cmd/Ctrl + P`), the interface hides the editor and reformats the preview for paper or PDF output.
- Theme preference and font size settings are saved in `localStorage` for persistence.

## Privacy & Data
- **100% client-side processing** - Your content never leaves your browser
- **No tracking or analytics** - We don't collect any user data
- **Local storage only** - Only theme and font size preferences are stored locally
- **No cookies** - The application doesn't use cookies

## Roadmap Ideas
- ~~Configurable theme (light/dark/system)~~ ✅ Implemented
- Import/export Markdown files
- Custom KaTeX macros and macro presets
- Syntax highlighting for code blocks
- Export to other formats (HTML, DOCX)

## License
Released under the [MIT License](LICENSE).
