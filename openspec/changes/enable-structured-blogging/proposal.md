# Proposal: Enable Structured Blogging

## Summary
Introduce a comprehensive blogging system supporting advanced technical content rendering (KaTeX, Mermaid, Tables) and a dedicated frontend listing. Replace the current placeholder projects on the homepage with a dynamic blog feed.

## Motivation
The user wants to share technical insights that require specialized rendering (math, diagrams). A dedicated "Blogs" section provides better categorization than the generic projects feed for purely informative content.

## Proposed Solution
- **Enhanced Rendering**: Integrate KaTeX for LaTeX math and Mermaid.js for diagrams via the base template.
- **Blog Section**: Create `blogs` content type with custom metadata (`name`, `desc`, `tags`, `date`, `project`).
- **Homepage Update**: Replace "Beta" and "Alpha" project tiles with a single large "Recent Content" or "Blogs" bento card that leads to `/blogs`.
- **Dedicated List page**: A clean, technical archive at `/blogs`.

## Scenarios
- **Technical Writing**: User writes a post with LaTeX formulas and a Mermaid flowchart; it renders beautifully on save.
- **Project Context**: A blog post about "Heimdall" shows the project link in the metadata because the `project` field is set.
- **Discovery**: A visitor on the homepage sees the latest blog snippet and clicks "Read More" to go to the archive.
