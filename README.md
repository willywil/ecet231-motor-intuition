# ECET 231 Motor Intuition Manual (public site)

Interactive reconstruction of the **Purdue University North Central ECET 231 Electrical Power and Machinery Lab Manual (Summer 2012)**, aimed at producing a complete motor datasheet from the manual’s tests.

Hosted for GitHub Pages from this repository (`ecet231-motor-intuition`).

## Editions

| Path | Edition | What it includes |
|------|---------|------------------|
| `lean/` | **A — Lean** | Theory, widgets, analysis methods, motor models (v2.5), control, magnetics, blank datasheet entry tables, redrawn SVG schematics, design system. **No** PNC page scans, **no** 2012 handwritten measurements, **no** Google Drive file IDs/links. Book citations are short attributions only. |
| `with-data/` | **B — With data** | Everything in A, plus Jonathan Wilhelm’s 2012 handwritten measurements as typed tables (exact transcription, flagged uncertainties kept) and analysis results computed from them. Verify/correct panel included **without** scan crops. Still no scans / Drive IDs. |
| `full/` | **C — Full** | Byte copy of the private v2.5 HTML (motor-models), including embedded page scans. |

Root `index.html` is the landing page. `.nojekyll` is present so Pages serves the site as static files.

## Credits & copyright

- Original lab manual: Purdue University North Central ECET 231 (Summer 2012).
- Handwritten measurements: Jonathan Wilhelm.
- PNC manual content remains the property of its authors. Edition C embeds reconstructed page scans; the site publisher accepted that copyright risk. Editions A and B omit the scans and keep only short citations.

## Local build note

These files were generated into `public_site_v25/` from the v2.5 build (motor-models) by `public_site_v25_tools/build_public_site_v25.py`, applying the v2.5 changes to the QC'd v2.4 public editions; earlier builds and `public_site/` were not modified.

## New in v2.5

Motor Models section (after Methods of Analysis): brushed DC ↔ BLDC in one model; LR → LRC → parasitics; thermal models as differential equations; BLDC six-step vs FOC; proposed LCR/VNA tests MM-T1…T12 and 49 optional datasheet fields (`datasheet_schema_v25.json`). A coding agent commits this bundle to GitHub separately.

Live site: https://willywil.github.io/ecet231-motor-intuition/
