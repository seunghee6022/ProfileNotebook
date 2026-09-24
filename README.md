# Seunghee's Notebook

A personal research site for PhD preparation — a math blog, an interactive citation graph of paper reviews, and a living CV — built as a single static `index.html` (no build step, no dependencies to install).

## What's inside

- **Profile** — bio, research interests, and a timeline of how I got here.
- **Math Blog** — short write-ups with LaTeX math, rendered client-side via [MathJax](https://www.mathjax.org/).
- **Papers** — a force-directed citation graph ([D3.js](https://d3js.org/)) of reviewed papers; click a node for authors, venue, source link, and a review note.
- **CV** — a typeset, printable CV (education, experience, projects, publications, skills) with a "Save as PDF" button.

## Running it locally

No build step — just open `index.html` in a browser, or serve the folder:

```bash
npx serve .
```

## Updating content

All content lives in the `SITE_DATA` object near the top of the `<script>` block at the bottom of `index.html` — edit the `profile`, `posts`, `papers`, and `cv` fields directly, no templating or build step required.

## Deploying

This repo is set up for [GitHub Pages](https://pages.github.com/): once enabled (Settings → Pages → Deploy from a branch → `main` / `root`), it's served automatically at `https://seunghee6022.github.io/ProfileNotebook/`.
