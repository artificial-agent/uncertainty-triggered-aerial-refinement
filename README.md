# When to Ask for Help — project page

Static project page for *When to Ask for Help: Uncertainty-Triggered Aerial Refinement for
Off-Road Navigation*, built from the
[Academic Project Page Template](https://github.com/eliahuhorwitz/Academic-project-page-template)
(a modernized fork of the [Nerfies](https://nerfies.github.io) page).

## Double-blind

The paper is under review and reviewers reach this page through an anonymous mirror, which
serves these repo files as-is. So the page must not name the authors, their affiliations or
labs, **and must not contain absolute URLs back to the hosting GitHub account** — that link
alone de-anonymizes the submission. Every URL in `index.html` is relative for that reason,
and the code repository is deliberately not linked.

Search `index.html` for `TODO after de-anonymization` for what to restore on acceptance:

- authors, affiliations, and their links in the hero
- `citation_author` / `citation_pdf_url` meta tags and the JSON-LD author list
- absolute `og:url` and `og:image` (needed for real link previews)
- Paper / arXiv / Code / Video buttons
- BibTeX authors, cite key, venue, and DOI

## Content

Everything lives in `index.html` — abstract, method write-up, results carousel, simulation
table, and field summary are filled in from the submitted paper. Figures under
`static/images/` are downscaled exports of the paper figures:

| Path | Source figure |
|---|---|
| `teaser.jpg` | `fig_platforms_env_4` (hero) |
| `method.png` | `overall_figure` (autonomy pipeline) |
| `result_return_on_flight.png` | `fig_sim_return_on_flight` |
| `result_mission_time.png` | `fig_sim_mission_time` |
| `result_field_requests.jpg` | `route11_ground_only_assistance_signal_actual_policy` |
| `result_field_decision.jpg` | `route11_trial11_intervention3_decision_overview` |
| `result_platforms.jpg` | `fig_platforms_bold` |
| `social_preview.jpg` | 1200x630 crop of the hero, for link previews |

Still optional: a short muted teaser clip at `static/videos/teaser.mp4` (swap it in for the
teaser image), and the paper PDF at `static/pdfs/paper.pdf` once it can be released.

No build step. Open `index.html` in a browser to preview, or run `python3 -m http.server`
in this directory.

## Deploying

GitHub Pages serves the `main` branch from `/`. Pushing to `main` redeploys.
