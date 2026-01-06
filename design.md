# Portfolio Design System

## Overview
This design system establishes the visual language for a high-end personal portfolio. The philosophy balances **professional data density** with **cinematic aesthetics**. It relies on a "dark mode first" approach, using deep backgrounds, modular "bento-box" grids, and vibrant gradients to guide user focus.

## Brand Identity

### Color Palette

#### Base/Neutrals
The foundation of the interface. We avoid pure black to maintain depth.
- **Void Black**: `#050505` (Main App Background / Body)
- **Deep Surface**: `#0F0F0F` (Secondary Background)
- **Card Surface**: `#161616` (Main Component Background)
- **Elevated Surface**: `#1F1F1F` (Modals / Hover States)
- **Stroke/Border**: `rgba(255, 255, 255, 0.08)` (Subtle separation)

#### Text/Content
- **Primary Text**: `#FFFFFF` (Headings, Values)
- **Secondary Text**: `#A1A1AA` (Labels, Descriptions - Zinc-400 equivalent)
- **Disabled/Muted**: `#52525B` (Zinc-600 equivalent)

#### Semantic Accents (Neons)
Used sparingly for data visualization and interactive states.
- **Signal Green**: `#34D399` (Growth, Success, "Online")
- **Electric Purple**: `#A78BFA` (Creative, Analytics, Insights)
- **Solar Orange**: `#FBBF24` (Energy, Warnings)
- **Plasma Pink**: `#F472B6` (Highlights, Marketing)

### Typography

**Font Family**: `Inter`, `Outfit`, or `DM Sans` (Clean, modern sans-serif).
*Optional: Use a Monospace font (e.g., `JetBrains Mono`) specifically for data tables or code blocks*

**Type Scale**
- **Display XL** (Hero Stats): `64px` / Light (300) / -2% tracking
- **H1** (Page Titles): `32px` / SemiBold (600) / -1% tracking
- **H2** (Section/Card Headers): `24px` / Medium (500)
- **H3** (Subsection): `18px` / Medium (500)
- **Body**: `16px` / Regular (400) / 1.5 line-height
- **Label/Caption**: `12px` / Medium (500) / +2% tracking (Uppercase optional)

## Foundation

### Spacing Scale
Based on a 4px grid.
- **xs**: `4px`
- **sm**: `8px`
- **md**: `16px`
- **lg**: `24px` (Standard Card Padding)
- **xl**: `32px`
- **2xl**: `48px`

### Layout & Grid
- **Container**: Max-width `1440px`.
- **Dashboard Grid**: A "Bento UI" approach using CSS Grid.
- **Gap**: `20px` or `24px` between cards.
- **Card Padding**: Consistent `24px` internal padding.

### Shapes & Corners
- **Card Radius**: `24px` (Smooth, modern feel).
- **Inner Radius**: `12px` (Buttons, Inputs).
- **Icon Radius**: `50%` (Circular icon buttons).

## Visual Effects

### Depth & Glass
- **Subtle Glow**: `box-shadow: 0 0 40px -10px rgba(accent-color, 0.15);`
- **Card Border**: `border: 1px solid rgba(255, 255, 255, 0.05);`
- **Glass Panel**: 
  - `background: rgba(20, 20, 20, 0.7);`
  - `backdrop-filter: blur(12px);`
  - `border: 1px solid rgba(255, 255, 255, 0.1);`

### Gradients
Use subtle radial gradients on card backgrounds to simulate a light source.
- *Example*: `radial-gradient(circle at top left, rgba(255,255,255,0.03), transparent 70%)`

## Components

### 1. The "Bento" Card
The primary container for all content.
- **Visual**: Dark grey surface (`#161616`), `24px` radius, subtle 1px border.
- **Header**: Flex row with Title (H2/H3) on left, Action/Icon on right.
- **Content**: Fills remaining space.

### 2. Stat Blocks
- **Layout**: Label (top) + Huge Value (middle) + Trend indicator (bottom/right).
- **Typography**: Value is Display XL size.
- **Color**: Value is White; Trend is green/red.

### 3. Navigation Rail
- **Style**: Vertical pill or floating dock.
- **Item**: Icons with generous padding.
- **State**: 
  - *Active*: White icon, subtle glow background.
  - *Inactive*: Grey icon (`#52525B`).

### 4. Action Buttons
- **Primary**: Solid Accent Color (e.g., Green or White) -> Black Text. Pill shape (`999px` radius) or Rounded Rect (`12px`).
- **Secondary**: Transparent background -> White border (1px) -> White Text.
- **Utility**: Icon-only, circular, slightly lighter background (`#27272A`).

### 5. Charts (Visuals)
- **Style**: Area charts with gradient fills (fading to transparent at bottom).
- **Lines**: Smooth Bezier curves (stroke-width 2px or 3px).
- **Axes**: Minimal or hidden. No grid lines (or very faint dashed).

## Guidelines

1. **Hierarchy via Contrast**: Don't use lines to separate content; use spacing and text color (White vs Grey).
2. **Breathing Room**: Keep layouts airy. The heavy dark background needs negative space to feel "premium" rather than "cramped."
3. **Data First**: The most important number on a card should be the largest element.
4. **Consistency**: Always use the defined corner radiuses (`24px` outer, `12px` inner). Do not mix sharp and round corners.
