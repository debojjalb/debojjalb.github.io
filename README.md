# debojjalb.github.io

Personal academic website, built with [Hugo](https://gohugo.io/) (no theme).

```
content/            page text (edit these)
  _index.md           Home: bio, education, recent updates, profile links
  research.md         Research: areas, publications, talks
  travel.md           Diary: one entry per trip
  informs.md          INFORMS 2026 talk page (/INFORMS/)
layouts/            page templates (HTML)
  index.html          Home
  404.html            "Page not found"
  _default/           baseof.html (shared header, navigation, footer),
                      research.html, travel.html, informs.html
static/             copied to the site as-is
  images/             profile photo and travel/<trip folder>/ photos
  uploads/            CV and thesis PDFs
  style.css           all styling
  favicon.png
hugo.yaml           site title, navigation menu, analytics ID
```

Preview locally with `hugo server`. Pushing to `main` publishes the site
(see `.github/workflows/publish.yaml`).

To add a Diary entry, add a folder of photos under `static/images/travel/`
and an entry pointing to it in `content/travel.md`.
