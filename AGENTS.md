# AGENTS.md

Jekyll personal resume site, deployed to GitHub Pages. No tests, lint, or typecheck.

## Structure

- `resume.md` is the source of truth. `readme.md` is a symlink to it; `index.md` renders it via `{% include_relative resume.md %}`.
- `_config.yml` (Jekyll 4.3, `minima` theme), `_layouts/default.html`, `assets/css/main.css`.
- `djseng-me-agent-brief.md` (untracked, local-only) holds resume background when present. Prefer it over guessing; never commit it.

## Build / deploy

- CI (`.github/workflows/jekyll.yml`) runs only on push to `master` (`bundle exec jekyll build`, then `md-to-pdf resume.md` → `_site/resume.pdf`, deploy to Pages).
- Preview locally: `bundle install` then `bundle exec jekyll serve`. Requires Ruby 3.2 per CI.
- Do not add a `Gemfile.lock`, `node_modules/`, or `vendor/`; all are excluded in `_config.yml`.

## Resume editing rules

- Do not invent employers, dates, durations, metrics, or tools. Engagements carry explicit durations (e.g. `· 7 yrs 2 mos`); keep them.
- Match the existing resume voice; consult the local brief for background (it is untracked — never commit it).
- The PDF download button in `_layouts/default.html` expects `resume.pdf` at the site root (CI generates it); keep the `resume.md` filename stable.
