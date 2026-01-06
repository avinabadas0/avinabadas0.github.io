# Proposal: Polish Homepage Design

## Summary
Elevate the visual fidelity of the homepage to match the "high-end" aesthetic of `design.md` and the user's inspiration images. This involves moving from flat colors to rich gradients, enhancing glassmorphism, and adding subtle animations.

## Motivation
The initial implementation provided the structure (Bento grid) but lacks the "wow" factor (gradients, depth, glow) which makes the design feel "boring" and "flat". The user wants it "spiced up".

## Proposed Solution
- **Global Background**: Add a subtle mesh gradient or vignettes to the body background so it's not just flat black.
- **Card Styling**:
  - Replace flat background with `linear-gradient` surfaces.
  - strengthen borders with `rgba(white, 0.08)`.
  - Add specific "glow" states for hover.
- **Hero Section**: Give the hero card a signature gradient backing (Purple/Pink/Blue blends).
- **Typography**: Increase contrast between headers (white) and body (grey). Use tighter letter-spacing for headers.
- **Buttons**: Switch to "glass" buttons with hover glows.

## Scenarios
- **First Impression**: User sees a cinematic, glowing interface rather than a wireframe.
- **Interaction**: Hovering over cards reveals a subtle "spotlight" or border glow effect.
