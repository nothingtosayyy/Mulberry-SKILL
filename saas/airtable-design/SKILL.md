---
name: airtable-design
slug: airtable-design
cat: saas
desc: Airtable brand design system — complete design tokens for colors, typography (Haas Grotesk / Inter Display), spacing, border-radius, elevation, components (buttons, cards, nav, inputs, pricing), and r
source: 
color: "#FCB400"
logo: "a"
date: 2026-07-30

  description: Airtable brand design system — complete design tokens for colors, typography (Haas Grotesk / Inter Display), spacing, border-radius, elevation, components (buttons, cards, nav, inputs, pricing), and responsive breakpoints. Use when building UI pages or prototypes in Airtable's visual style. Triggers on airtable design, airtable style, airtable brand, airtable UI.
  version: 1.0.0
  install_method: share
  share_id: 1497d6e08b1313ed7c64fa90242c9da1
---

# Airtable Design System

## Overview

Airtable's marketing surfaces are quietly editorial. The base atmosphere is white canvas, dark ink type, generous whitespace, and a near-black pill CTA — nothing is fighting for attention until a section needs to. The brand voltage doesn't come from gradient washes or accent walls; it comes from **full-bleed signature cards** in coral (#aa2d00), dark green (#0a2e0e), and dark navy (#181d26) that punctuate long-scroll explainer pages every two or three screens. Between those signature bands, the page reads like a print magazine: a headline, supporting copy, a small image cluster, then breathing room.

Type voice is Haas Grotesk at modest weights (400 for display, 500 for sub-titles and buttons). Display headlines never go bolder than 500 — emphasis comes from size and color contrast, not from weight. Body copy stays at 14px / 400 throughout. The pricing surface runs its own dialect: **Inter Display** at unusual mid-weights (475 / 575) and **pill-shaped buttons** (9999px radius) that don't appear on any other page — a deliberate sub-system signaling "this page is about commercial precision."

## Colors

### Brand & Accent
| Token | Hex | Role |
|---|---|---|
| primary | #181d26 | Dominant brand color. Primary CTA bg, h1/h2 display type, dark surface band |
| primary-active | #0d1218 | Press state on primary buttons |

### Surface
| Token | Hex | Role |
|---|---|---|
| canvas | #ffffff | Default page surface |
| surface-soft | #f8fafc | Tabbed feature cards, featured pricing tier |
| surface-strong | #e0e2e6 | Light gray CTA banner near footer |
| surface-dark | #181d26 | Dark navy mid-page CTA cards |
| surface-dark-elevated | #1d1f25 | Articles-page hero base |
| hairline | #dddddd | 1px border for inputs, table dividers, secondary buttons |

### Text
| Token | Hex | Role |
|---|---|---|
| ink | #181d26 | Strongest text — h1/h2 display, primary button text-on-light |
| body | #333840 | Default running-text color |
| muted | #41454d | Footer links, breadcrumbs, captions |
| border-strong | #9297a0 | 1px outline on disabled secondary buttons |
| on-primary | #ffffff | Text on primary buttons and dark surfaces |
| on-dark | #ffffff | Text on dark surfaces |

### Signature Card Surfaces
| Token | Hex | Role |
|---|---|---|
| signature-coral | #aa2d00 | Largest signature card (homepage) |
| signature-forest | #0a2e0e | Deep-green signature card |
| signature-cream | #f5e9d4 | Cream callout band |
| signature-peach | #fcab79 | Demo-card surface |
| signature-mint | #a8d8c4 | Demo-card surface |
| signature-yellow | #f4d35e | Demo-card surface |
| signature-mustard | #d9a441 | Demo-card surface |

### Semantic
| Token | Hex | Role |
|---|---|---|
| link | #1b61c9 | Inline body links (NOT primary button color) |
| link-active | #1a3866 | Link press state |
| info | #254fad | Inline info badges |
| info-border | #458fff | Focused-input outline |
| success | #006400 | Confirmation states |
| success-border | #39bf45 | Success borders |
| pricing-ink | #1d1f25 | Pricing surface text |

## Typography

### Font Family
- **Main system:** Haas / Haas Groot Disp (fallback: -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, etc.)
- **Pricing sub-system:** Inter Display at mid-weights (475/575)
- **Substitute:** If Haas unavailable, use Inter Display (variable) — adjust line-height down ~5%

### Hierarchy
| Token | Size | Weight | Line-Height | Letter-Spacing | Use |
|---|---|---|---|---|---|
| display-xl | 48px | 500 | 1.1 | 0 | Articles page h2 |
| display-lg | 40px | 400 | 1.2 | 0 | Homepage h1 hero |
| display-md | 32px | 400 | 1.2 | 0 | Feature-section headlines |
| title-lg | 24px | 400 | 1.35 | 0.12px | Section titles |
| title-md | 20px | 400 | 1.5 | 0 | Sub-section titles |
| title-sm | 18px | 500 | 1.4 | 0 | Article-card titles |
| label-md | 16px | 500 | 1.4 | 0 | Demo-card titles, labels |
| button | 16px | 500 | 1.4 | 0 | CTA button labels |
| body-md | 14px | 400 | 1.25 | 0 | Body copy, footer links, nav |
| caption | 14px | 500 | 1.35 | 0.16px | Captions and meta text |
| legal | 13.12px | 600 | 1.2 | 0 | Cookie/legal CTA |
| pricing-display | 44.8px | 475 | 1.1 | 0 | Pricing h1 |
| pricing-section | 28px | 475 | 1.2 | 0 | Pricing section heads |
| pricing-card-title | 20px | 475 | 1.3 | 0 | Pricing tier plan name |

### Principles
- Display sizes prefer weight 400 — a 40px h1 is NOT bold
- Weight 500 for sub-titles, buttons, article titles; never 600/700 in editorial body
- Only true bold (600) in legal surfaces
- Pricing uses Inter Display at font-weight 475 (custom mid-weight variable font)

## Spacing

Base unit: **4px** (all spacing snaps to 4-multiples)

| Token | Value |
|---|---|
| xxs | 4px |
| xs | 8px |
| sm | 12px |
| md | 16px |
| lg | 24px |
| xl | 32px |
| xxl | 48px |
| section | 96px |

- **Section padding:** 96px vertical (universal constant)
- **Card padding:** 32px (feature/pricing cards), 48px (signature cards), 24px (cream callouts)
- **Gutters:** 24px between cards in 3-up grids; 16px in denser strips
- **Max content width:** ~1280px centered with 48px horizontal breathing room

## Border Radius

| Token | Value | Use |
|---|---|---|
| xs | 2px | Cookie/legal CTA buttons |
| sm | 6px | Text inputs, small buttons |
| md | 10px | Content cards, article cards, cream callouts |
| lg | 12px | Primary CTAs, signature cards, feature cards |
| pill | 9999px | Pricing-page CTAs ONLY (sub-system signal) |
| full | 9999px | Circular icon buttons, avatars |

## Elevation

| Level | Treatment | Use |
|---|---|---|
| Flat | No shadow, no border | Body sections, nav, footer |
| Soft hairline | 1px #dddddd border | Inputs, sub-nav, dividers, secondary buttons |
| Button rest | Soft drop with subtle blue-tinted glow | Primary CTA buttons |
| Button focus | Outer 2px blue ring | Keyboard focus on primary buttons |
| Card flat | No shadow; color contrast | Signature cards, cream callouts, demo cards |

**Philosophy:** Color-block first, shadow second. No atmospheric shadow or heavy elevation.

## Components

### Buttons
- **button-primary:** bg #181d26, text #fff, 16px/24px padding, 12px radius. One per viewport. Active: #0d1218
- **button-secondary:** bg #fff, text #181d26, 12px radius, 1px hairline outline
- **button-secondary-on-dark:** Same as secondary but on dark surfaces. White stays white.
- **button-pricing-pill:** bg #fff, text #1d1f25, 9999px radius, 12px/24px padding. PRICING ONLY.
- **button-legal:** bg #1b61c9, text #fff, 13.12px/600, 2px radius, 12px/10px padding
- **button-icon-circular:** 40×40px, bg #fff, hairline border, full radius
- **text-link:** #1b61c9, no underline by default, inherits body-md

### Cards & Containers
- **hero-band:** White canvas, no decoration, 96px vertical padding. Headline + buttons in whitespace.
- **signature-coral-card:** bg #aa2d00, text #fff, 12px radius, 48px padding. Full-bleed product callouts.
- **signature-forest-card:** bg #0a2e0e, text #fff, 12px radius, 48px padding.
- **hero-card-dark:** bg #181d26, text #fff, 12px radius, 48px padding. Mid-page CTA.
- **feature-card-tabbed:** bg #f8fafc, 12px radius, 32px padding. Left tab rail + right content pane.
- **cream-callout-card:** bg #f5e9d4, 10px radius, 24px padding. Product UI fragments.
- **demo-grid-card:** bg #fff or pastel surfaces, 10px radius, 16px padding. Uneven heights.
- **logo-strip:** bg #fff, muted logos, 32px vertical padding. 6 logos desktop, 3 mobile.
- **article-card:** bg #fff, 10px radius, 16px padding. 16:9 thumbnail + title + meta.

### Inputs
- **text-input:** bg #fff, 14px/400, 6px radius, 12px/16px padding, 44px height, 1px #dddddd border
- **text-input-focus:** Border recolors to #458fff

### Pricing Sub-System
- **pricing-tier-card:** bg #fff, 10px radius, 32px padding. Plan name in Inter Display 20px/475.
- **pricing-tier-card-featured:** bg #f8fafc (only signal is background shift)
- **pricing-comparison-row:** 12px vertical padding, hairline dividers, 4 plan columns

### Navigation
- **top-nav:** 64px tall, white, wordmark left, menu center-left, CTA cluster right. Always light.
- **footer:** bg #fff, 6-column links, body-md type, 96px+ vertical padding
- **cta-band-light:** bg #e0e2e6, 12px radius, 48px padding. Final CTA strip.

## Responsive Breakpoints

| Name | Width | Key Changes |
|---|---|---|
| Mobile | < 768px | 1-col, hamburger nav, 1-up grid, full-bleed signature cards |
| Tablet | 768–1024px | 2-up grid, horizontal scroll pricing table |
| Desktop | 1024–1440px | 3/4-up grid, full nav, 4-across pricing |
| Wide | > 1440px | Same as desktop, 1280px max, more outer margin |

## Do's and Don'ts

### Do
- Keep primary CTA near-black (#181d26), not link blue
- Reserve button-primary for one action per viewport
- Use button-secondary (white + hairline) as the natural pair
- Trust whitespace as hero atmosphere — no gradient/mesh
- Use signature cards (coral/forest/dark) for brand voltage moments
- Keep demo-grid-card heights uneven within a grid
- Treat pricing as its own dialect (Inter Display + pill buttons)
- Anchor every band with 96px vertical padding

### Don't
- Don't make #1b61c9 the primary button color (it's the link color)
- Don't add gradient backdrop to hero (white, full stop)
- Don't bold display-weight type (400/500 only, never 700)
- Don't use pill radius (9999px) outside pricing
- Don't repeat same surface in consecutive bands (maintain rhythm)
- Don't introduce additional accent colors beyond documented palette
