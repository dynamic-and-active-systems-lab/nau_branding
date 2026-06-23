# NAU Branding — Claude Design System

Official Northern Arizona University brand specifications for use with Claude-assisted design. This repository provides the source of truth for colors, typography, spacing, logo rules, and voice/tone so Claude can produce on-brand designs without manual guidance on every request.

## How to Use This Repo with Claude

1. Open a Claude Code session in this directory (or add it as a project context).
2. Claude reads `CLAUDE.md` automatically and applies brand rules without being asked.
3. Reference `css/variables.css` in any web project to get all tokens as CSS custom properties.
4. Point Claude to specific guideline files for detailed rules on a given topic.

## Repository Structure

```
CLAUDE.md                  ← Claude reads this automatically — brand quick reference + rules
README.md                  ← This file

tokens/
  colors.json              ← All colors: hex, RGB, CMYK, Pantone, usage notes
  typography.json          ← Font families, weights, print specifications
  spacing.json             ← Spacing scale, logo minimum sizes, layout values

css/
  variables.css            ← All tokens as CSS custom properties (--nau-true-blue, etc.)

guidelines/
  color-usage.md           ← When/how to use each color, accessibility rules
  typography.md            ← Font decisions by context, print specs
  logo-usage.md            ← Logo types, sizes, colors, dos and don'ts
  voice-tone.md            ← Brand pillars, personality, AP style, legal copy

logos/
  README.md                ← Where to download official logo files (Mediagraph)

examples/
  components.html          ← Reference UI: color palette, type, buttons, cards, alerts, hero, forms

RESOURCES/                 ← Source PDFs (not committed to public repo)
  NAU-Brand-Quick-Guide-update-6-1-23.pdf
  Visual-Identity-Guide.pdf
```

## Key Brand Values at a Glance

| Token | Value |
|-------|-------|
| Primary color | `#002454` NAU True Blue (Pantone 282 C) |
| Accent color | `#FAC01A` NAU Gold (Pantone 3514 C) |
| Web font | Acumin Pro (3 variants only) |
| Print font | Univers (licensed) |
| Voice | Personal, active, concrete, concise |

## Sources

All specifications are drawn from:
- [NAU Visual Identity Guide](https://in.nau.edu/visual-identity-guide/)
- [NAU Color Guide](https://in.nau.edu/visual-identity-guide/color/)
- [NAU Typography Guide](https://in.nau.edu/visual-identity-guide/typography/)
- [NAU University Marks](https://in.nau.edu/visual-identity-guide/university-marks/)
- [NAU Writing Style Guide](https://in.nau.edu/writing-style-guide/)
- [NAU Brand](https://in.nau.edu/brand-strategic-communications/nau-brand/)
- Visual Identity Guide PDF v3 (2018) and Brand Quick Guide (2023)

## Important Notes

- **Logo files are not stored here.** Download from [mediagraph.io/nau/login](https://mediagraph.io/nau/login) (NAU institutional login required). All trademark use requires authorization from the Office of Trademarks & Licensing.
- **Source PDFs are not committed** to public repositories due to trademark sensitivity. Store locally in `RESOURCES/`.
- Color values in this repo reflect the authoritative web guide (in.nau.edu). Where the PDFs differ, the website values take precedence.

## Contact

| Office | Email | Phone |
|--------|-------|-------|
| University Marketing | marketing@nau.edu | 928-523-1741 |
| Trademark Licensing | licensing@nau.edu | 928-523-5404 |
| Brand Management | BrandMgmt@nau.edu | — |
