# Design: Bento Grid Implementation

## Principles
Reference the root `design.md` for all visual tokens. This document focuses on the *grid implementation*.

## Grid Architecture
We will use CSS Grid for the main layout.
- **Container**: `display: grid; gap: var(--spacing-md);`
- **Columns**: `grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));` (approximate, usually better to exact count for Bento control).
- **Spans**: Cards can have classes like `.span-2` (wide) or `.span-row-2` (tall) to create the "Bento" look.

## Component Hierarchy
- `l-grid`: Main layout wrapper.
- `c-card`: The base glass-panel component.
    - `c-card--hero`: Special styling for the intro.
    - `c-card--project`: Contains image + title + tag.
    - `c-card--stat`: Big number + label.

## Asset Management
- **CSS**: Pure modular CSS (no Tailwind dependency required unless complex, but `design.md` tokens map easily to CSS variables). *Note: User mentioned Tailwind preferred, but also "modular CSS". Given the "Vanilla CSS" instruction in system prompt, I will stick to highly structured CSS Variables unless Tailwind is strictly enforced. Actually, for a Bento Grid, raw CSS Grid is often cleaner than fighting Tailwind classes for bespoke spans.*
- **Icons**: SVG injection or a lightweight icon font.
