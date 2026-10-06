# AGENTS.md

Jekyll personal resume site, deployed to GitHub Pages. No tests, lint, or typecheck.

## Structure

- `resume.md` is the source of truth. `readme.md` is a symlink to it; `index.md` renders it via `{% include_relative resume.md %}`.
- `_config.yml` (Jekyll 4.3, `minima` theme), `_layouts/default.html`, `assets/css/main.css`.
- Private context lives in the separate private repo `djseng/me-private`, checked out at `../me-private`. Never copy its files into this public repo.
  - `djseng-me-agent-brief.md`: resume background. Prefer it over guessing.
  - `djseng-me-resume-notes.md`: full confirmed detail behind `resume.md`, including confidential engagement context and content trimmed for the 2-page limit. Read it before rewriting.

## Build / deploy

- CI (`.github/workflows/jekyll.yml`) runs only on push to `master` (`bundle exec jekyll build`, then `md-to-pdf resume.md` → `_site/resume.pdf`, deploy to Pages).
- Preview locally: `bundle install` then `bundle exec jekyll serve`. Requires Ruby 3.2 per CI.
- Do not add a `Gemfile.lock`, `node_modules/`, or `vendor/`; all are excluded in `_config.yml`.

## Resume editing rules

- Do not invent employers, dates, durations, metrics, or tools. Engagements carry explicit durations (e.g. `· 7 yrs 2 mos`); keep them.
- Match the existing resume voice; consult the brief in `../me-private` for background.
- The generated PDF must stay at 2 pages. Check with `md-to-pdf` and `pdfinfo` before finishing.
- The PDF download button in `_layouts/default.html` expects `resume.pdf` at the site root (CI generates it); keep the `resume.md` filename stable.
