# NAU Branding — Claude Design System Context

This repository contains Northern Arizona University's official brand specifications for use in Claude-assisted design work. Read this file before generating any NAU-branded designs, components, or copy.

---

## Quick Reference

### Colors

| Token | Hex | Use |
|-------|-----|-----|
| `--nau-true-blue` | `#002454` | Primary brand color — dominant in all designs |
| `--nau-gold` | `#FAC01A` | Accent, logo mountain, CTAs on dark backgrounds |
| `--nau-monsoon` | `#C3B8B2` | Neutral warm gray — subtle backgrounds, borders |
| `--nau-twilight` | `#0066B2` | Interactive blue for links and buttons |
| `--nau-sunset` | `#F68300` | Warm orange accent — sparingly |
| `--nau-summer-shade` | `#007A33` | Green accent — sparingly |
| `--nau-supai` | `#00ADB5` | Teal accent — sparingly |
| `--nau-sky` | `#41B6E6` | Light blue — very sparingly |
| `--nau-red-rock` | `#CF4527` | Red-orange accent — sparingly |

All CSS custom properties are defined in `css/variables.css`.
All raw token values with Pantone/CMYK/RGB are in `tokens/colors.json`.

### Typography

**Web:** `Acumin Pro` (3 variants only: Pro, Condensed, Extra Condensed). Fallback: Arial.
**Print/docs:** `Univers` (licensed). Fallback: Arial.
**Email:** `Calibri`. Fallback: Arial.
**Formal:** `Adobe Caslon Pro`. Fallback: Times New Roman.

Never use Univers on the web. Never use Acumin in print materials.

### Spacing

Base unit: 4px. Scale: 4, 8, 12, 16, 20, 24, 32, 40, 48, 64, 80, 96px.
Full scale in `tokens/spacing.json` and `css/variables.css`.

---

## Design Rules Claude Must Follow

### Colors
1. True Blue (`#002454`) must be the dominant color in every design. If a design doesn't feel blue-forward, revisit it.
2. Secondary colors (Sunset, Summer Shade, etc.) follow an **80/20 rule** — 80% primary colors, 20% secondary maximum.
3. **Never** use the gold-type logo variation in any digital or web context. Always use True Blue type on web.
4. All text over colored backgrounds must meet WCAG AA contrast (4.5:1 for normal text, 3:1 for large text).
5. Do not introduce colors outside the approved palette. Do not use tints or transparency of brand colors.

### Logo
6. Every NAU communication must include the NAU logo.
7. Default to the **Primary (stacked) Two-Color logo**: True Blue type, Gold mountain.
8. Maintain clear space equal to the ligature "A" height on all sides.
9. Minimum logo width on web: **185px**. Never render smaller.
10. Do not distort, rotate, tint, crop, recolor, or alter the logo in any way.
11. See `guidelines/logo-usage.md` for full rules. Actual logo files: nau.edu/digitalassets/widen-collective

### Typography
12. On web, use Acumin Pro only (3 variants). On print, use Univers. Never swap these.
13. Use font weight variation (not size alone) to establish hierarchy.

### Writing
14. Voice: personal, active, concrete, concise. Speak directly to the reader — not institutionally.
15. Brand personality: welcoming, supportive, collaborative, determined, respectful.
16. All URLs must begin with `nau.edu`.
17. Phone format: `xxx-xxx-xxxx`. Times: `6 p.m.` (space, periods). Dates: `October 3` (no ordinal suffixes).
18. All departmental publications require an Equal Opportunity statement (short form minimum).

---

## File Map

```
tokens/
  colors.json       — all color values (hex, RGB, CMYK, Pantone) + usage notes
  typography.json   — font families, weights, print specs
  spacing.json      — spacing scale + logo minimum sizes

css/
  variables.css     — all tokens as CSS custom properties

guidelines/
  color-usage.md    — when and how to use each color
  typography.md     — font decisions by context, print specs
  logo-usage.md     — logo types, sizes, colors, dos and don'ts
  voice-tone.md     — brand pillars, personality, AP style rules

logos/
  README.md         — where to download official logo files (Widen Collective)

examples/
  components.html   — reference UI implementation
```

---

## Brand Contacts

| Office | Email | Phone |
|--------|-------|-------|
| University Marketing | marketing@nau.edu | 928-523-1741 |
| Trademark Licensing | licensing@nau.edu | 928-523-5404 |
| Brand Management | BrandMgmt@nau.edu | — |
| Printing Services | printing.services@nau.edu | 928-523-1941 |

Templates: nau.edu/templates
Logo downloads: nau.edu/digitalassets/widen-collective
Order stationery: nau.edu/order
