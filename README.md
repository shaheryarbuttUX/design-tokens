# Design Tokens

A real, usable design-token set: the single source of truth for color, typography, spacing, radius, shadows, and breakpoints across my projects.

## Files

| File | Format | Use |
|------|--------|-----|
| `tokens.json` | W3C-style JSON | Feed into Style Dictionary or any build pipeline |
| `tokens.css` | CSS custom properties | Drop straight into a stylesheet: `var(--color-brand-500)` |

## What's inside

- **Color** — brand blues, neutrals (9-step), success/warning/danger
- **Typography** — Inter-based scale (xs → 4xl), weights, line heights
- **Spacing** — 4px base scale
- **Radius & shadows** — sm/md/lg + full
- **Breakpoints** — sm / md / lg / xl

## Usage

```css
@import "tokens.css";

.button-primary {
  background: var(--color-brand-500);
  color: var(--color-neutral-0);
  border-radius: var(--radius-md);
  padding: var(--spacing-3) var(--spacing-6);
  font-size: var(--font-size-base);
  font-weight: var(--font-weight-medium);
}
```

## Why this exists

Design systems live or die on tokens. This is the same token structure I use when setting up design systems in Figma (variables) and in code (Webflow/Framer/hand-coded sites) — one naming convention, both worlds.
