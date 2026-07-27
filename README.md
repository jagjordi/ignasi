# Ignasi Solé Piñas — academic website

Personal academic website for **Dr Ignasi Solé Piñas**, musicologist (empirical performance studies).
Built with the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme and deployed automatically
to GitHub Pages.

🔗 **Live site:** https://jagjordi.github.io/ignasi/

## What's here

| Path | Content |
|------|---------|
| `_pages/about.md` | Homepage / biography |
| `_pages/publications.md` + `_bibliography/papers.bib` | Publications (preprints, thesis, dataset) |
| `_pages/research.md` | Research statement |
| `_pages/teaching.md` | Teaching statement |
| `_pages/cv.md` + `_data/cv.yml` | CV (rendered from YAML) |
| `_projects/` | Project cards (research threads & work in preparation) |
| `_news/` | Homepage announcements |
| `assets/pdf/ignasi_sole_pinas_portfolio.pdf` | Downloadable full portfolio PDF |

## Deployment

Deployment is fully automated by GitHub Actions (`.github/workflows/deploy.yml`):

1. On every push to `main`, the workflow builds the Jekyll site.
2. The built site is published to the `gh-pages` branch.
3. GitHub Pages serves `gh-pages` at the URL above.

No manual steps are required after the initial Pages setup (Settings → Pages → Deploy from a branch → `gh-pages`).

## Local development (optional)

Requires Ruby + Bundler and Node:

```bash
bundle install
npm install
bundle exec jekyll serve
```

Then open <http://localhost:4000/ignasi/>.

## Things to personalise

- **Profile photo** — replace `assets/img/prof_pic.jpg` with a real photo (the current file is a generated placeholder).
- **Google Scholar / ORCID** — add `scholar_userid` / `orcid_id` in `_data/socials.yml` to show those icons.
- **arXiv IDs** — three 2026 preprints currently show their submission IDs; add public arXiv IDs in `_bibliography/papers.bib` once assigned.

---

Based on the [al-folio](https://github.com/alshedivat/al-folio) theme (MIT License).
