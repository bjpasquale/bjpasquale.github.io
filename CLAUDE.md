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

## Al-folio scaffolding — already removed

The al-folio leftovers are **gone**; do not go looking for them. Cleared in `2beeee4` (upstream
theme docs + the no-op citations workflow) and `0d0fd41` ("Remove al-folio theme scaffolding"):

- Removed: `_pages/`, `_posts/`, `_projects/`, `_news/`, `_books/`, `_data/`, `_layouts/`,
  `_config.yml`, `INSTALL.md`, `CUSTOMIZE.md`, `FAQ.md`, `CONTRIBUTING.md`, and
  `.github/workflows/update-citations.yml` (with `_data/citations.yml`).
- Still present, deliberately: `_bibliography/papers.bib` — the only surviving al-folio file.
  Not served (`.nojekyll`); kept as the publications source of record.
- `README.md` is no longer the upstream theme doc — it was rewritten in `2beeee4` to describe
  this static site accurately.

The whole tracked repo is now 14 files; `git ls-files` is the fastest inventory.

## Notes

- Mostly dormant — update `index.html` as needed for the academic/professional profile.
- Domain: `CNAME` is set to `benpasquale.com` (added in `dee7a49`). The repo and the default
  Pages host are still `bjpasquale.github.io`.
