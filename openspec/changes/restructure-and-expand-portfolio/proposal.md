# Proposal: Restructure and Expand Portfolio

## Summary
Restructure the homepage to have a prominent non-grid hero, transform bento components into a interactive timeline and skills grid, and expand the site with a dedicated recruiter-friendly "About" page and structured "Projects" section (including a featured page for "Heimdall").

## Motivation
The user wants a more traditional but high-end hero introduction and a deeper level of detail for recruiters. The "Experience" stat is too simple; a timeline provides better context for recent work like "Heimdall". Scaling these components for the "About" page ensures consistency while providing the "deep dive" recruiters need.

## Proposed Solution
- **Homepage Structure**:
  - Move the Greeting/Name and "About Me" CTA above the `.l-grid`.
  - Content within the grid will focus on the Timeline, Skills, and Recent Projects/Posts.
- **New Components**:
  - `partial "components/timeline.html"`: A vertical line with dots/labels.
  - `partial "components/skills.html"`: A grid of DevIcons.
- **Content Expansion**:
  - Create `content/about.md` and a corresponding `layouts/page/about.html` or similar.
  - Create `content/projects/heimdall.md`.
  - Ensure `layouts/projects/list.html` and `layouts/projects/single.html` exist for structured exploration.

## Scenarios
- **Hero Engagement**: Recruiter lands and immediately sees the name and value prop without grid clutter.
- **Technical Insight**: Recruiter scrolls to "Skills" and sees a recognized stack via icons.
- **Career Path**: Recruiter sees the vertical timeline highlighting the intensive focus on "Heimdall" in 2025.
- **Project Deep Dive**: Use clicks a project to see a full technical breakdown.
