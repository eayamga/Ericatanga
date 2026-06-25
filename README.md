# Eric Ayamga — Academic Website

Personal academic website built with [Hugo](https://gohugo.io/) and deployed to GitHub Pages.

**Live URL (after deployment):** https://eayamga.github.io/Ericatanga/

## Local preview

```bash
hugo server -D
```

Then open http://localhost:1313/Ericatanga/ in your browser.

## Structure

- `content/_index.md` — homepage bio
- `data/papers.yaml` — publications and working papers
- `data/teaching.yaml` — teaching history
- `data/awards.yaml` — fellowships and awards
- `data/presentations.yaml` — conference presentations
- `static/images/photo.jpg` — headshot
- `static/files/` — PDFs (CV, papers)

See `UPDATING.md` for how to edit content.

## Deploy

Push to `main` on GitHub. GitHub Actions builds and deploys automatically. Enable GitHub Pages under **Settings → Pages → Source: GitHub Actions** on first deploy.
