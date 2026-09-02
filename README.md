# bjpasquale.github.io

Personal academic + professional site for **Benjamin J. Pasquale** — political science / South Asia, plus real estate and software. Served at [benpasquale.com](https://benpasquale.com). Ben is the founder of [Tiny Weekends](https://tinyweekends.co), a weekend guide for Delaware families.

## What this is

A **minimal static site**: a single `index.html` with inline CSS (no build step, no framework). `.nojekyll` tells GitHub Pages to serve the repo as-is. Icons via Font Awesome + Academicons (CDN).

Built on the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme until **2026-04-08** (commit `5ed073e`), when it was replaced with the current hand-written static page. The dormant al-folio scaffolding (`_pages/`, `_posts/`, `_layouts/`, `_config.yml`, etc.) is no longer served and is kept only as reference.

## Local preview

```bash
python3 -m http.server 8000   # then open http://localhost:8000
```

## Deploy

Automatic on push to `main`/`master` via `.github/workflows/deploy.yml` (uploads the repo root to GitHub Pages). No local build.

See `CLAUDE.md` for the full working notes.
