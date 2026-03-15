# Personal Academic Site

GitHub Pages portfolio site built on the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme. Political science / South Asia focus.

## Stack

- Jekyll (Ruby), al-folio theme
- Deployed via GitHub Pages (has `.github/workflows/` CI)
- Remote: `bjpasquale/bjpasquale.github.io` (SSH)

## Local Dev

```bash
bundle install
bundle exec jekyll serve
# → http://localhost:4000
```

## Content

- `_pages/` — static pages (about, CV, etc.)
- `_posts/` — blog posts (markdown with YAML frontmatter)
- `_projects/` — project showcase entries
- `_data/` — structured data (CV, coauthors, repositories)
- `assets/` — images, PDFs, CSS overrides

## Notes

- Mostly dormant — update as needed for academic profile
- `_config.yml` controls site metadata, theme options, social links
- Domain: currently `bjpasquale.github.io`, planned migration to `benpasquale.com` via Cloudflare
