# Updating Your Website

This site is built with Hugo and deploys automatically when you push to the `main` branch on GitHub. Changes usually go live within about two minutes.

## Add a new paper

1. Open `data/papers.yaml` on GitHub (or locally).
2. Add a new entry at the top of the file:

```yaml
- title: "Your Paper Title"
  authors: ["Your Name", "Coauthor Name"]
  year: 2026
  status: "working paper"
  venue: ""
  pdf: "files/your-paper.pdf"
  link: ""
  abstract: "One-sentence or one-paragraph summary."
  job_market_paper: false
  tags: ["health economics"]
```

3. If you have a PDF, upload it to `static/files/your-paper.pdf`.
4. Commit and push to `main`.

**Status options:** `published`, `accepted`, `revise and resubmit`, `under review`, `working paper`, `work in progress`

## Mark your job market paper

Set `job_market_paper: true` on the relevant entry in `data/papers.yaml`. Set it to `false` on all other papers.

## Mark a paper as published

Change `status` from `"working paper"` to `"published"` and add the journal name in the `venue` field.

## Update your bio

Edit `content/_index.md`. The text under the front matter (`---`) is your bio on the homepage.

## Update your tagline or contact info

Edit `hugo.yaml` under the `params:` section.

## Add a teaching entry

Edit `data/teaching.yaml` and add:

```yaml
- course: "Course Name"
  role: "Instructor"
  institution: "Texas Tech University"
  term: "Fall 2026"
```

## Add a presentation

Edit `data/presentations.yaml` and add a new entry at the top.

## Update your CV

1. Export your CV as a PDF from Overleaf.
2. Replace `static/files/cv.pdf` with the new file (keep the same filename).
3. Update the CV menu link in `hugo.yaml` to point to `/files/cv.pdf` instead of the Overleaf URL.
4. Push to `main`.

## Change your photo

Replace `static/images/photo.jpg` with a new headshot (square or portrait works best). Keep the same filename.

## Add a blog post

Create a new folder and file: `content/blog/your-post-slug/index.md`

```yaml
---
title: "Post Title"
date: 2026-03-15
description: "One-sentence summary."
---

Your post content here.
```

Then add a Blog menu item in `hugo.yaml` if you want it in the navigation.

## Add an award or fellowship

Edit `data/awards.yaml` and add a new entry.

---

All changes auto-deploy when you push to `main`. No need to install anything locally unless you want to preview before pushing (`hugo server`).
