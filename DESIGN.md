---
name: Neutral Wireframe
colors:
  surface: '#faf8ff'
  surface-dim: '#dad9e3'
  surface-bright: '#faf8ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f4f3fc'
  surface-container: '#eeedf7'
  surface-container-high: '#e8e7f1'
  surface-container-highest: '#e2e1eb'
  on-surface: '#1a1b22'
  on-surface-variant: '#47464a'
  inverse-surface: '#2f3037'
  inverse-on-surface: '#f1f0f9'
  outline: '#78767b'
  outline-variant: '#c8c5ca'
  surface-tint: '#5f5e60'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#1c1b1d'
  on-primary-container: '#858386'
  inverse-primary: '#c8c6c8'
  secondary: '#5d5e66'
  on-secondary: '#ffffff'
  secondary-container: '#e3e1ec'
  on-secondary-container: '#63646c'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#1f1a1a'
  on-tertiary-container: '#8a8282'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#e5e1e4'
  primary-fixed-dim: '#c8c6c8'
  on-primary-fixed: '#1c1b1d'
  on-primary-fixed-variant: '#474649'
  secondary-fixed: '#e3e1ec'
  secondary-fixed-dim: '#c6c5cf'
  on-secondary-fixed: '#1a1b22'
  on-secondary-fixed-variant: '#46464e'
  tertiary-fixed: '#ebe0df'
  tertiary-fixed-dim: '#cec4c4'
  on-tertiary-fixed: '#1f1a1a'
  on-tertiary-fixed-variant: '#4c4545'
  background: '#faf8ff'
  on-background: '#1a1b22'
  surface-variant: '#e2e1eb'
typography:
  headline-xl:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-lg:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  headline-sm:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '600'
    lineHeight: 24px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  label-lg:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
  label-md:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
  label-sm:
    fontFamily: Inter
    fontSize: 10px
    fontWeight: '500'
    lineHeight: 14px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  gutter: 1rem
  gutter-mobile: 0.75rem
  margin: 1rem
  margin-mobile: 1rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 2rem
---

## Brand & Style

This design system is engineered specifically for low-fidelity wireframing and structural prototyping. Its purpose is to eliminate aesthetic distraction and focus purely on layout hierarchy, spatial cadence, user flows, and interaction patterns. 

The aesthetic is functional, strictly grayscale, and intentionally devoid of brand personality or chromatic sentiment:
- **Design Style:** Minimalist, structural, and schematic. The system borrows from blueprint architectural drawings and modern wireframing conventions.
- **Visual Tenor:** Objective, clean, deliberate, and unopinionated. Elements express their behavioral role through tonal differentiation rather than expressive styling.
- **Guiding Principle:** Content and structure first. Every container, button, form element, and placeholder acts as an abstract scaffolding for rapid mobile product conceptualization.

## Colors

The palette is strictly achromatic, built on precise neutral zinc tiers. No saturated colors or hue shifts are allowed anywhere within the system.

### Functional Color Roles
- **Base Canvas (`#FFFFFF`):** Default background for artboards, mobile screens, and full-width views.
- **Subtle Surface (`#F4F4F5`):** Secondary backgrounds, card containers, and empty image block fills.
- **Structural Border (`#E4E4E7`):** Card bounds, subtle dividers, and inactive input field outlines.
- **Emphasis Border (`#D4D4D8`):** Container borders, interactive component borders, and placeholder cross-lines.
- **Placeholder / Inactive Text (`#A1A1AA`):** Form placeholder hints, skeleton bar placeholders, and disabled states.
- **Secondary / Supporting Text (`#71717A`):** Captions, secondary labels, metadata, and helper text.
- **Body Text (`#3F3F46` / `#27272A`):** High-readability standard copy, list content, and descriptions.
- **Primary / Dominant (`#09090B`):** Solid call-to-action buttons, high-contrast badges, active states, and screen titles.

## Typography

Typography prioritizes clarity, structural weight distribution, and standard system legibility. Font fallback chain resolves to `Inter, -apple-system, BlinkMacSystemFont, "SF Pro", "Segoe UI", Roboto, sans-serif`.

### Usage Guidelines
- **Headlines:** Use `headline-xl` sparingly for screen headers on mobile; use `headline-lg` and `headline-md` for view anchors and modal titles.
- **Body Copy:** Standardize on `body-md` for application flows; use `body-sm` for secondary disclosures and metadata.
- **Labels:** Use `label-lg` for interactive targets (buttons, menu items) and `label-sm` for badge indicators, wireframe annotations, and form field fieldsets.
- **Wireframe Text Placeholders:** When actual copy is undecided, use either standard Latin sentences or grayed skeleton blocks (`h-2` to `h-3` rounded rectangles filled with `#E4E4E7`).

## Layout & Spacing

The layout model is tailored for mobile viewport architectures (375px to 430px base viewports) with consistent horizontal gutters and rhythm.

### Grid & Canvas Structure
- **Mobile Canvas:** Standard 4-column layout on mobile devices with `gutter-mobile` (12px / 0.75rem) and `margin-mobile` (16px / 1rem) outer padding.
- **Rhythm Multiples:** Strictly built on an 8pt baseline grid, with 4pt (`space-xs`) reserved for tight internal component padding (e.g., input field padding, badge padding).
- **Component Separation:** Standard component gap within stacks is `space-md` (16px). Major section blocks (lists to card groups, header to content) use `space-lg` (24px) or `space-xl` (32px).

## Elevation & Depth

This system is completely flat. No dynamic blurs, ambient multi-layered shadows, or colored glow effects are allowed.

### Depth Hierarchy
- **Level 0 (Base Canvas):** Pure white (`#FFFFFF`).
- **Level 1 (In-Page Grouping / Containers):** Surface tint `#F4F4F5` or `#FFFFFF` enclosed by a 1px solid `#E4E4E7` border.
- **Level 2 (Overlays, Bottom Sheets, Dialogs):** `#FFFFFF` fill with a crisp 1px solid `#D4D4D8` border. If depth separation is required over dense content, a flat semi-opaque scrim (`rgba(9, 9, 11, 0.4)`) is used behind the layer.
- **No Drop Shadows:** Elevation is communicated through contrasting outlines and surface fills, maintaining a blueprint drafting aesthetic.

## Shapes

The shape philosophy uses slight, restrained rounding (`roundedness: 1`, 4px base border radius) to prevent harsh terminal corners while maintaining the structured, technical appearance of a blueprint.

- **Base Radius (`rounded`, 4px / 0.25rem):** Standard for inputs, buttons, checkboxes, chips, and small cards.
- **Medium Radius (`rounded-lg`, 8px / 0.5rem):** Sheet dialogs, nested content containers, and large mobile cards.
- **Full Radius (`rounded-full`):** Reserved solely for circular avatar placeholders, status dots, and radio buttons.

## Components

### Buttons
- **Primary:** Background `#09090B`, text `#FFFFFF`, 1px border `#09090B`. Height: 44px (touch target), radius: 4px.
- **Secondary:** Background `#FFFFFF`, text `#09090B`, 1px border `#D4D4D8`.
- **Ghost / Tertiary:** Background transparent, text `#71717A`, no border.
- **Disabled:** Background `#F4F4F5`, text `#A1A1AA`, 1px border `#E4E4E7`.

### Input Fields
- **Container:** Height 44px, background `#FFFFFF`, border 1px solid `#D4D4D8`, corner radius 4px, padding 0 12px.
- **Placeholder Text:** `#A1A1AA`, typography `body-md`.
- **Value Text:** `#09090B`, typography `body-md`.
- **Label:** Positioned above input, typography `label-sm`, color `#3F3F46`, gap 4px.

### Cards & Grouping Containers
- **Border Card:** Background `#FFFFFF`, 1px solid `#E4E4E7`, padding 16px, radius 8px.
- **Tonal Card:** Background `#F4F4F5`, 1px solid transparent or `#E4E4E7`, padding 16px, radius 8px.

### Wireframe Image & Media Placeholders
- **Box Placeholder:** Background `#F4F4F5`, border 1px solid `#D4D4D8`.
- **Crosshair / Diagonals:** 1px solid `#D4D4D8` drawn corner-to-corner (X motif) across the box, or centered standard image icon (`24x24px` outlined in `#A1A1AA`).
- **Aspect Ratios:** Default to `16:9`, `4:3`, or `1:1`.

### Chips & Badges
- **Status Badge:** Height 24px, background `#F4F4F5`, border 1px solid `#D4D4D8`, typography `label-sm`, text `#3F3F46`, horizontal padding 8px.
- **Selected Filter Chip:** Background `#09090B`, text `#FFFFFF`, border 1px solid `#09090B`.

### Lists & Cell Rows
- **List Item:** Height min 48px, horizontal layout with space-between alignment.
- **Divider:** 1px solid `#E4E4E7` horizontal rule, inset by 16px or full width.

### Checkboxes & Radios
- **Checkbox:** 18x18px square, 2px radius, 1px solid `#71717A`. When checked: fill `#09090B`, stroke `#FFFFFF` checkmark icon.
- **Radio Button:** 18x18px circle, 1px solid `#71717A`. When selected: fill `#FFFFFF`, with centered 8px solid `#09090B` dot.

### Iconography
- **Style:** 1.5px stroke, monoline, 20x20px or 24x24px bounding box, stroke color `#27272A` or `#71717A`. No solid filled iconography unless indicating active bottom-tab selection.