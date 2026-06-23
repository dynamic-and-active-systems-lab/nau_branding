# NAU Branding — Claude Design System

Official Northern Arizona University brand specifications for use with Claude-assisted design. This repository provides the source of truth for colors, typography, spacing, logo rules, and voice/tone so Claude can produce on-brand designs without manual guidance on every request.

## Using This Repo as a Design System in Claude

### Option 1 — Claude.ai Projects (recommended for most NAU users)

This is the easiest way to share the design system across your team without requiring any coding tools.

1. Go to [claude.ai](https://claude.ai) and create a new **Project**.
2. In the Project's **Knowledge** panel, upload the following files from this repo:
   - `CLAUDE.md`
   - `tokens/colors.json`
   - `tokens/typography.json`
   - `css/variables.css`
   - `guidelines/color-usage.md`
   - `guidelines/logo-usage.md`
   - `guidelines/typography.md`
   - `guidelines/voice-tone.md`
3. Add a **Project instruction** (in the project settings) such as:
   > You are an NAU design assistant. Always apply the NAU brand guidelines from the uploaded files. Follow every rule in CLAUDE.md without being asked.
4. Every conversation inside that Project will automatically have access to the full design system. Share the Project with colleagues via the share link.

> **Tip:** When the brand guidelines change, re-upload the affected files to the Project Knowledge panel to keep Claude current.

---

### Option 2 — Claude Code (for developers)

Claude Code reads `CLAUDE.md` automatically whenever you open a session in this directory, so no setup is needed beyond cloning the repo.

```bash
git clone git@github.com:dynamic-and-active-systems-lab/nau_branding.git
cd nau_branding
claude   # CLAUDE.md is loaded automatically
```

From there you can ask Claude to build components, write copy, or generate layouts and it will apply NAU brand rules without any additional prompting. Reference `css/variables.css` in any web project to inherit all brand tokens.

---

### Option 3 — Paste context into any Claude conversation

If you don't want to set up a Project, copy and paste the contents of `CLAUDE.md` at the start of any Claude conversation. This gives Claude the brand rules for that session only.

---

### Example prompts once the design system is loaded

- *"Create a hero banner for the College of Engineering using NAU brand guidelines."*
- *"Write an email announcement for a new graduate program. Use NAU voice and tone."*
- *"Build a registration form component using the NAU CSS variables."*
- *"What color should I use for a CTA button on a dark blue background?"*
- *"Review this paragraph for NAU writing style compliance."*

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
