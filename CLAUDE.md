# Personal Academic Site

GitHub Pages portfolio site for Benjamin J. Pasquale. Political science / South Asia focus,
plus real estate and software. **Minimal static HTML** — a single `index.html` with inline CSS,
no build step.

## Stack

- Plain static HTML + inline CSS (black-and-white, askell.io-inspired). Icons via Font Awesome +
  Academicons (CDN links in `index.html`).
- No Jekyll, no Ruby, no build. `.nojekyll` disables GitHub Pages' Jekyll processing so the repo
  is served as-is.
- Deployed via GitHub Actions (`.github/workflows/deploy.yml`) — uploads the repo root (`path: '.'`)
  straight to GitHub Pages on push to `main`/`master`.
- Remote: `git@github.com:bjpasquale/bjpasquale.github.io.git` (SSH)

> **History:** the site was built on the [al-folio](https://github.com/alshedivat/al-folio) Jekyll
> theme until it was replaced with the current static `index.html` on 2026-04-08
> (commit `5ed073e`).

## Local Dev

No build. Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000   # → http://localhost:8000
```

## Content

- `index.html` — the entire live site: bio, timeline (academic + professional), publications
  with abstracts. Edit here.

## Vestigial al-folio scaffolding (NOT served)

The redesign left the old theme files in the repo but they are dormant — `.nojekyll` means none
of them are processed or published. Do not treat these as live content:

- `_pages/`, `_posts/`, `_projects/`, `_news/`, `_books/`, `_bibliography/`, `_data/`,
  `_layouts/*.liquid`, `_config.yml` — leftover al-folio source.
- `README.md`, `INSTALL.md`, `CUSTOMIZE.md`, `FAQ.md`, `CONTRIBUTING.md` — upstream al-folio theme
  docs. They describe the old Jekyll theme, **not** this site. Candidates for removal (ask Ben).
- `.github/workflows/update-citations.yml` still runs and commits `_data/citations.yml`, but the
  static `index.html` does not read that file — the "Update Google Scholar citations" commits are
  now no-ops for the live site. Candidate for disabling (ask Ben).

## Notes

- Mostly dormant — update `index.html` as needed for the academic/professional profile.
- Domain: currently `bjpasquale.github.io`; planned migration to `benpasquale.com`.
