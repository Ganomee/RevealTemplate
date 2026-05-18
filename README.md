# easyRadiology Reveal.js Markdown Baseline

This repo now provides a **markdown-first baseline** for Reveal.js instead of a hardcoded HTML+JS deck.

## Run locally with reveal-md

```bash
npx reveal-md deck.md --css css/easyrad-theme.css
```

## What is included

- `deck.md` — starter slide content in markdown.
- `css/easyrad-theme.css` — reusable theme styles, including radial red rings and raised panels.
- `assets/brand/easyradiology-logo.svg` — placeholder filename/path for official logo asset.
- `assets/images/er-team.jpg` — placeholder filename/path for official image asset.

## Notes

- The deck is set to 16:9 (1600x900) via frontmatter in `deck.md`.
- To use different official assets, replace files in `assets/brand` and `assets/images` and update references in `deck.md`.

- In this environment, direct asset download from easyradiology.de returned HTTP 403, so placeholder files were kept for easy replacement.
