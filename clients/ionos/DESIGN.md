---
name: IONOS EXOS
description: |
  IONOS corporate design system, extracted from the official EXOS framework v3.0.
  Brand-orange primary action, OpenSans/Overpass type pairing, generous 16px radius,
  pill-shaped buttons. Built for trustworthy B2B/hosting product UIs.
version: 1.0
colors:
  primary: "#ff8800"
  primary-hover: "#cc6e00"
  primary-soft: "#ffdbb2"
  secondary: "#2944cc"
  surface: "#ffffff"
  surface-elevated: "#ffffff"
  surface-muted: "#f7f7f9"
  surface-inverted: "#2e3842"
  on-surface: "#2e3842"
  on-surface-strong: "#1b1b1b"
  on-surface-muted: "#8493b3"
  on-surface-subtle: "#ccd5e3"
  on-surface-inverted: "#f7f7f9"
  border: "#dee2e6"
  border-strong: "#8493b3"
  success: "#256f25"
  success-shape: "#2af7bb"
  warning: "#86510d"
  warning-shape: "#ffbf10"
  critical: "#e20000"
  critical-shape: "#ff2a2a"
  info: "#1a4079"
  info-shape: "#2f2f70"
typography:
  display:
    fontFamily: "Overpass"
    fontSize: "32px"
    fontWeight: 600
    lineHeight: "38px"
  h1:
    fontFamily: "Overpass"
    fontSize: "32px"
    fontWeight: 600
    lineHeight: "38px"
  h2:
    fontFamily: "Overpass"
    fontSize: "22px"
    fontWeight: 600
    lineHeight: "28px"
  h3:
    fontFamily: "Overpass"
    fontSize: "16px"
    fontWeight: 600
    lineHeight: "22px"
  h4:
    fontFamily: "Overpass"
    fontSize: "14px"
    fontWeight: 600
    lineHeight: "20px"
  body-lg:
    fontFamily: "Open Sans"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: "22px"
  body-md:
    fontFamily: "Open Sans"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: "20px"
  body-sm:
    fontFamily: "Open Sans"
    fontSize: "12px"
    fontWeight: 400
    lineHeight: "18px"
  label:
    fontFamily: "Open Sans"
    fontSize: "14px"
    fontWeight: 600
    lineHeight: "20px"
spacing:
  xxs: "4px"
  xs: "8px"
  sm: "12px"
  md: "16px"
  lg: "24px"
  xl: "32px"
  xxl: "48px"
  section: "64px"
rounded:
  xxs: "2px"
  xs: "4px"
  sm: "8px"
  md: "16px"
  button: "24px"
  full: "9999px"
breakpoints:
  mobile: "576px"
  tablet: "768px"
  desktop: "1024px"
  wide: "1280px"
shadows:
  sm: "0 1px 2px 0 #71809580"
  md: "0 2px 8px 0 #71809580"
  card: "0 1px 5px -3px #031a4a24"
  card-hover: "0 2px 10px -2px #031a4a24"
tech:
  framework: "EXOS 3.0"
  cdn-js: "https://ce1.uicdn.net/exos/framework/3.0/exos.min.js"
  cdn-css: "https://ce1.uicdn.net/exos/framework/3.0/exos.min.css"
  notes: |
    Use EXOS web components where possible (<exos-button>, <exos-card>, <exos-table> etc.).
    Custom Tailwind/CSS is acceptable for layout but should mirror the EXOS token values.
---

<!--
Extracted from: https://ce1.uicdn.net/exos/framework/3.0/exos.min.css (EXOS Framework 3.0)
Referenced styleguide: https://www.ionos-brand.com/8c09ffc8a/p/9961c6-ionos-styleguide
Date: 2026-05-19
Method: CSS custom property extraction from official IONOS framework
-->

# IONOS EXOS

## Overview

The IONOS corporate design language, codified in the **EXOS framework**. Designed to convey reliability, technical competence, and approachable expertise — the visual signature of a European hosting and cloud provider serving SMBs and IT professionals.

Two type voices: **Overpass** for headlines (the "corporate" voice — confident, structured) and **Open Sans** for body text (the "default" voice — readable, neutral). One signal color — IONOS Orange (`#ff8800`) — reserved exclusively for primary actions and brand moments. Everything else stays in muted neutrals so the orange always wins attention.

This system is responsive: text sizes step up at desktop breakpoints, and component shapes are deliberately rounded (16px default, 24px pill-buttons) to soften the otherwise corporate-blue surroundings.

## Colors

### Signal & Action

- **Primary** (`#ff8800` — corporate-4): The IONOS Orange. **Reserved for primary CTAs and active states only.** Never use as decoration or large surface fill.
- **Primary hover** (`#cc6e00`): Darker orange for hover/active states on primary actions.
- **Primary soft** (`#ffdbb2` — corporate-2): Subtle orange tint for selected list items, highlight backgrounds, or info badges that need a brand touch.
- **Secondary** (`#2944cc` — activating-2): Deep activating blue. For links and informational accents where orange would be too loud.

### Surfaces

- **Surface** (`#ffffff`): Default page background.
- **Surface elevated** (`#ffffff`): Cards, modals, dropdowns — relies on subtle shadow + border, not on background-color difference.
- **Surface muted** (`#f7f7f9` — neutral-1): Section breaks, secondary panels, table headers.
- **Surface inverted** (`#2e3842` — corporate-8): Dark mode surfaces (footer, dark hero sections, navigation bars).

### Text & Shapes

- **On-surface** (`#2e3842` — corporate-8): Default body text. The "house dark."
- **On-surface strong** (`#1b1b1b` — corporate-9): Headlines and emphasized text.
- **On-surface muted** (`#8493b3` — neutral-6): Secondary text, metadata, captions, placeholders.
- **On-surface subtle** (`#ccd5e3` — neutral-5): Disabled text, divider labels.
- **On-surface inverted** (`#f7f7f9` — neutral-1): Text on inverted surfaces.

### Borders

- **Border** (`#dee2e6` — neutral-4): Default input borders, subtle dividers, card outlines.
- **Border strong** (`#8493b3` — neutral-6): Focused inputs, active separators, table dividers.

### Feedback

- **Success** text `#256f25`, shape `#2af7bb`: Confirmations, "saved" states.
- **Warning** text `#86510d`, shape `#ffbf10`: Caution states, soft warnings.
- **Critical** text `#e20000`, shape `#ff2a2a`: Errors, destructive actions.
- **Info** text `#1a4079`, shape `#2f2f70`: Neutral informational notices.

Always pair `text-color` with the matching `shape-color`: text version on inputs/labels, shape version on icons/dots/badges.

## Typography

**Headline voice — Overpass:** A geometric grotesk, semibold (600). Conveys structure and confidence. Use for all headlines, button labels, and emphasized UI labels.

**Body voice — Open Sans:** A humanist sans-serif, regular (400) for body, semibold (600) for labels. Highly legible at small sizes, neutral in character.

### Type Scale (desktop)

| Token | Family | Size / Line-height | Weight | Use for |
|-------|--------|-------------------|--------|---------|
| `display` / `h1` | Overpass | 32 / 38 | 600 | Page titles, hero headlines |
| `h2` | Overpass | 22 / 28 | 600 | Section headers |
| `h3` | Overpass | 16 / 22 | 600 | Card titles, sub-sections |
| `h4` | Overpass | 14 / 20 | 600 | Group labels, field-set legends |
| `body-lg` | Open Sans | 16 / 22 | 400 | Lead paragraphs, intro text |
| `body-md` | Open Sans | 14 / 20 | 400 | Default body — the workhorse |
| `body-sm` | Open Sans | 12 / 18 | 400 | Captions, metadata, footnotes |
| `label` | Open Sans | 14 / 20 | 600 | Form labels, button text, table headers |

### Mobile Scale

Headlines drop one step on mobile (<768px):
- `h1`: 32 → 22px
- `h2`: 22 → 16px
- `h3`: 16 → 14px

Body sizes stay constant — readability beats hierarchy on small screens.

### Pairing Rules

- Mix the two voices intentionally: Overpass for "what this is", Open Sans for "what it says."
- Don't use Overpass for body text — it's too tight.
- Don't use Open Sans for headlines — it lacks the structural weight.

## Spacing & Layout

Based on a **4px grid** with t-shirt-sized tokens:

| Token | Px | Use for |
|-------|-----|---------|
| `xxs` | 4 | Icon-to-label gap, tight stacks |
| `xs` | 8 | Within form fields, button internals |
| `sm` | 12 | Between form fields in a group |
| `md` | 16 | Default spacing — card padding, list items |
| `lg` | 24 | Between groups, section internal padding |
| `xl` | 32 | Major card spacing, between content blocks |
| `xxl` | 48 | Sub-section break |
| `section` | 64 | Between full page sections |

### Container Widths

- **Reading content:** max 720px
- **App / dashboard layouts:** max 1280px
- **Marketing pages:** max 1440px

### Breakpoints

| Name | Px | Behavior |
|------|-----|----------|
| `mobile` | <576 | Single column, full-width cards |
| `tablet` | 576–768 | 2-column grids, side-padding 24px |
| `desktop` | 768–1024 | 3-column grids, hover states enabled |
| `wide` | >1024 | 4-column grids, fixed sidebar layouts |

## Components

For full component specs and states, see [components.md](./components.md).

### Buttons

EXOS buttons are **pill-shaped** (24px radius) — this is one of the most recognizable IONOS UI signatures.

- **Primary:** Filled orange (`primary`), white text, 2px border (transparent), padding `4px 20px`, font Overpass 600 14px.
- **Secondary:** Outlined, transparent fill, `border-strong` outline, `on-surface` text.
- **Ghost / Text:** No border, `secondary` (blue) text color, hover reveals soft background `surface-muted`.
- **Destructive:** Critical color fill, white text. Use sparingly — confirm before triggering.
- **Sizes:** Default 32px height. Small 24px (for table rows, inline). Large 40px (for hero CTAs).

Disabled state: 40% opacity, no hover transition, `not-allowed` cursor.

### Inputs

- 1px border (`border` color), `rounded-sm` (8px), `body-md` typography, padding `xs sm` (8px 12px).
- Height: 36px (default), 28px (compact for tables), 44px (large for forms).
- **Focus:** `secondary` (blue) border, 2px outline at 30% opacity (`#2944cc4d`).
- **Error:** `critical-shape` border + helper text below in `body-sm` `critical` color.
- **Disabled:** `surface-muted` background, `on-surface-subtle` text.

### Cards

- `surface-elevated` background, `rounded-md` (16px), padding `lg` (24px).
- Default: `border` 1px outline, `shadow-card` (very subtle).
- Hover (interactive cards): `shadow-card-hover` + 1px translate-Y up.
- Avoid stacking shadow + heavy borders on the same card — pick one tier.

### Tables

- `surface-elevated` rows with 1px bottom-border (`border` color).
- Hover row: `surface-muted` background.
- Selected row: `primary-soft` background, `primary` left-border (4px).
- Header: `surface-muted` background, `label` typography in `on-surface-muted` color, uppercase tracking +0.02em.

### Navigation

- **Top bar:** `surface-inverted` background (dark `#2e3842`), white text, 64px height.
- **Sidebar:** `surface` white background, 240px wide, 1px right-border. Active item: `primary-soft` fill + `primary` left-border.
- **Breadcrumb:** `on-surface-muted` separators (chevron-right icons), final crumb in `on-surface`.

## Patterns

**Forms:** Label above input (`label` typography, `xs` gap to input). Fields stack with `sm` gap. Submit button row has `lg` top margin, right-aligned on desktop, full-width on mobile.

**Empty states:** Centered. Icon at 64px (`xxl`) in `on-surface-muted`. Headline `h3`, supporting `body-md` in muted. Primary CTA below.

**Modals & sheets:** `surface-elevated`, `rounded-md`. Max-width 480px (small confirm), 720px (default), 960px (large). Backdrop: `on-surface` at 50% opacity. Always include explicit close action + escape-key handler.

**Toasts / page messages:** Use the `shape` variant of the matching feedback color for the icon, and the `text` variant for content. Position: top-right on desktop, top center on mobile. Auto-dismiss after 5s for success, sticky for errors.

## Motion

EXOS keeps motion subtle and functional. No decorative animation.

**Durations:**
- `fast` 150ms (hover states, focus transitions, icon-color changes)
- `base` 250ms (dropdown open/close, modal entry)
- `slow` 400ms (page-level transitions, drawer slide)

**Easing:**
- `ease-out` — `cubic-bezier(0.0, 0.0, 0.2, 1)` — for entering elements
- `ease-in` — `cubic-bezier(0.4, 0.0, 1, 1)` — for exiting elements
- `ease-in-out` — `cubic-bezier(0.4, 0.0, 0.2, 1)` — for state changes

**Patterns:**
- Hover on cards: 4px upward translateY + shadow upgrade (`card` → `card-hover`)
- Modal entry: fade-in 250ms + 8px translateY-from-bottom
- Toast entry: slide-in from edge, 250ms ease-out

Always respect `prefers-reduced-motion: reduce` — replace translateY/scale with opacity-only transitions.

## Accessibility

For details and verification scripts see [accessibility.md](./accessibility.md).

- **Contrast:** All token pairs in the YAML have been chosen so default text on default surface meets WCAG AA (4.5:1 body / 3:1 large). The IONOS Orange against white meets 3:1 — **use orange only for UI elements ≥18px or as background-with-white-text**.
- **Focus states:** Visible 2px ring on all interactive elements, using `secondary` (blue) at 30% opacity, offset 2px.
- **Touch targets:** Minimum 44x44px on touch surfaces — most EXOS buttons hit this in their default size.
- **Reduced motion:** All transitions opt-out via `@media (prefers-reduced-motion: reduce)`.
- **Color independence:** Feedback states (success/error/warning) always pair color with an icon or label — never communicate state through color alone.

## Tech Notes

This project uses **EXOS Framework v3.0** as the source of truth.

**Loading the framework:**
```html
<link rel="stylesheet" href="https://ce1.uicdn.net/exos/framework/3.0/exos.min.css" />
<script src="https://ce1.uicdn.net/exos/framework/3.0/exos.min.js" async defer></script>
```

**When to use EXOS web components:** Anywhere there's a stock pattern (buttons, inputs, tables, cards, panels, modals). Don't recreate them in Tailwind unless you need behavior EXOS doesn't ship.

**When to use Tailwind / custom CSS:** Layout (grid, flex), page-specific composition, marketing-page hero sections. Use the spacing/color tokens from this DESIGN.md so the custom code matches EXOS visually.

**CSS variables reference:** All tokens above map 1:1 to EXOS CSS custom properties (e.g., `colors.primary` → `var(--palette-corporate-4)`, `colors.on-surface` → `var(--default-text-color)`). When in doubt, use the CSS variable from EXOS directly.

## Do's & Don'ts

**Do:**
- Reserve orange for actions only — never for backgrounds, decorations, or large surface fills.
- Pair Overpass headlines with Open Sans body — both fonts are required for the IONOS voice.
- Use 16px (`rounded-md`) for cards and 24px (`rounded-button`) for buttons — these radii are unmistakably IONOS.
- Prefer EXOS web components over custom builds for stock UI patterns.
- Stick to the 4px spacing grid; layout consistency is what makes the system feel solid.

**Don't:**
- Don't use orange for body text or large hero backgrounds — contrast and brand-balance both suffer.
- Don't introduce custom border-radii outside the defined scale (2/4/8/16/24px).
- Don't mix in third-party UI kits (Material, Ant) — they fight EXOS's shape language.
- Don't use shadow AND a strong border on the same element — pick elevation tier (flat / outlined / floating).
- Don't add gradients or saturated decorative colors — IONOS visual identity is built on calm neutrals with a single warm accent.