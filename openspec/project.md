# Project Context

## Purpose
A high-end personal portfolio website built with Hugo, featuring a "HUD" (Heads-Up Display) graphic design theme. The project aims to showcase work with a technical, hacker-inspired aesthetic.

## Tech Stack
- **Hugo**: Static Site Generator (SSG).
- **Vanilla CSS**: Custom design system (avoiding external frameworks like Tailwind unless requested).
- **HTML5 & Vanilla JavaScript**: Core web technologies for structure and interactivity.
- **OpenSpec**: Framework for spec-driven development and change tracking.

## Project Conventions

### Code Style
- **Semantic HTML**: Prioritize clear, accessible structure with appropriate HTML5 elements.
- **Modern CSS**: Utilize CSS Variables, Flexbox, and Grid. Avoid ad-hoc utility classes in favor of a cohesive design system.
- **Simplicity**: Follow the "Simplicity First" rule—prefer <100 lines of new code and single-file implementations until proven insufficient.

### Architecture Patterns
- **Hugo Template System**: Modular use of `layouts/`, `partials/`, and `assets/`.
- **Spec-Driven Development**: All non-trivial changes must follow the OpenSpec workflow: Proposal -> implementation (tasks) -> Archive.
- **HUD Theme Design**: Consistent use of technical typography (e.g., monospace fonts), corner accents, glassmorphism, and red/status highlights.

### Testing Strategy
- **Manual Visual Review**: Ensuring design fidelity across different screen sizes and browsers.
- **Responsive Validation**: All components must be fully responsive.

### Git Workflow
- **Atomic Commits**: Commits should be focused and correspond to tasks in `tasks.md`.
- **Descriptive Branching**: Use kebab-case branch names tied to the `change-id`.

## Domain Context
- The site is a personal portfolio; content is primarily projects, blog posts, and contact information.
- The "HUD" theme is a central aesthetic goal, requiring precise CSS execution.

## Important Constraints
- **No Heavy Frameworks**: Avoid adding large libraries or CSS frameworks unless strictly necessary.
- **OpenSpec Compliance**: All changes must be validated using `openspec validate --strict`.

## External Dependencies
- **Google Fonts**: For technical typography (e.g., Outfit, Roboto Mono).
- **Hugo**: Required for building and local development (`hugo server`).
