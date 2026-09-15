# Uncertainty-Triggered Aerial Refinement — project page

Static project page for the paper, built from the
[Academic Project Page Template](https://github.com/eliahuhorwitz/Academic-project-page-template)
(a modernized fork of the [Nerfies](https://nerfies.github.io) page).

Live site: https://artificial-agent.github.io/uncertainty-triggered-aerial-refinement/

## Editing

Everything lives in `index.html`. Search for `TODO` to find what still needs filling in.

**Double-blind:** the paper is under review. Keep authors, affiliations, personal
links, and author metadata out of the page (and out of committed assets, e.g.
figures with lab logos or the paper PDF with a de-anonymized title block) until
the submission is de-anonymized. Places to fill in then are marked
`TODO after de-anonymization`.

- venue
- Paper / arXiv / Code / Video links
- abstract and method description
- BibTeX

Assets go under `static/`:

| Path | What |
|---|---|
| `static/videos/teaser.mp4` | short muted teaser clip (keep under ~10 MB) |
| `static/images/method.png` | system / pipeline figure |
| `static/images/result*.png` | result figures for the carousel |
| `static/images/social_preview.png` | 1200x630 link preview image |
| `static/images/favicon.ico` | replace the template favicon |
| `static/pdfs/paper.pdf` | paper PDF, if not linking to arXiv |

No build step. Open `index.html` in a browser to preview, or run
`python3 -m http.server` in this directory.

## Deploying

GitHub Pages serves the `main` branch from `/`. Pushing to `main` redeploys.
