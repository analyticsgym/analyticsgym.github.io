# STYLING.md

This file is the single source of truth for all visual decisions on this site. Reference it before making any styling changes.

---

## Design Philosophy: Japanese Minimalism (間 — Ma)

The site follows "Ma" (間) — the Japanese concept that emptiness is not absence but presence. Every design decision passes one test: "Can I remove something and make this better?"

## Principles

- **Kanso (簡素)** — Simplicity. Eliminate clutter and decoration. No gradients, no shadows, no rounded corners, no color fills.
- **Ma (間)** — Negative space IS the design. Generous margins and padding. Content breathes. Never crowd elements.
- **Fukinsei (不均整)** — Asymmetry. Left-aligned, not centered. Slight imbalance creates visual interest without decoration.
- **Shibui (渋い)** — Understated elegance. Beauty through restraint, not ornamentation.

## Typography

- Headings: "Cormorant Garamond" (Google Fonts). Light weight (300) for headings, regular (400) for emphasis. Large size, generous letter-spacing.
- Body: "IBM Plex Sans" at weight 300 (light). 18px base, 1.8 line-height. Comfortable long-form reading.
- Monospace (code): "IBM Plex Mono" at weight 300.
- NO bold text in body copy. Use spacing and size for hierarchy, not weight.

## Color Palette

- Background: #FAFAF8 (warm off-white, like washi paper)
- Text: #111111 (near-black, high contrast for readability)
- Accent: #6B3410 (deep sabi brown — like aged wood or rust)
- Muted: #5A5A55 (warm gray, readable secondary text)
- Borders: 1px solid #C8C6C1 (pencil-line, visible but quiet)
- Dark mode: do NOT implement. Single theme only.

## Layout Rules

- Max content width: 680px (narrow, focused reading column)
- Page margins: minimum 2rem on sides, 4rem top
- Section spacing: 3rem between sections minimum
- No sidebar. No multi-column layouts. Single column always.
- Horizontal rules: 1px, #E8E6E1, with 3rem vertical margin

## Navigation

- Top nav: site title left-aligned, minimal links right-aligned
- No logo, no icon. Title in Cormorant Garamond, light weight.
- Nav links: plain text, no underlines, sabi brown on hover
- No hamburger menu. If it doesn't fit on one line, cut links.

## Listing Page (Homepage)

- Posts listed vertically with generous spacing between items
- Each item shows: title (serif, larger) and status + categories (small, stone gray, below title)
- No thumbnails, no descriptions, no cards, no boxes
- Category filter buttons: plain text toggles, not pill buttons. Active state: sabi brown text. Inactive: stone gray.
- No grid. Vertical list only.

## Post Pages

- Title: Cormorant Garamond, large (2.5rem+), light weight
- Status badge: small text, stone gray, above or below title. Format: "Status: Developing" — plain text, not a colored badge
- Body: IBM Plex Sans Light, single column, generous line-height
- Block quotes: left border 2px sabi brown, italic, slightly indented. No background fill.
- Code blocks: IBM Plex Mono, #F5F4F0 background (barely tinted), 1px border #E8E6E1
- Lists: extra spacing between items, thin custom bullets
- Links: sabi brown, no underline. Underline on hover only.
- Images: full content-width, no border, 2rem margin above/below

## FORBIDDEN

- Box shadows of any kind
- Border radius (all corners sharp)
- Gradient backgrounds
- Colored backgrounds on any element (except code blocks)
- Bold body text (use size/spacing for hierarchy)
- Emoji anywhere on the site
- Animations or transitions (except subtle link hover: 0.2s)
- Cards, pills, badges with background colors
- More than 2 font families total (plus 1 monospace)
- Any color outside the defined palette
- Decorative elements (icons, dividers, flourishes)
- "Read more" links or truncated previews
- Dark mode
