# Design: Technical Blog Rendering

## Rendering Engine
- **KaTeX**: Loaded via CDN in `baseof.html`. Used for server-side-ish math rendering with high performance.
- **Mermaid.js**: Initialized in the footer. Searches for `.mermaid` classes and renders diagrams.
- **Tables**: Standard GFM (GitHub Flavored Markdown) tables, styled in `main.css` to match the Bento/Shadcn aesthetic.

## Metadata Display Logic
Metadata will be rendered conditionally using Hugo's `with` or `if` blocks:
- `name` (Title)
- `desc` (Summary)
- `tags` (Pill badges)
- `date` (Formatted string)
- `project` (Link to the project page)

## Homepage Integration
The grid will be adjusted:
- Remove standalone Beta/Alpha project cards.
- Add a new `span-4` (or similar) card for "Recent Blogs".
- Provide a clear "View Archive" button.
