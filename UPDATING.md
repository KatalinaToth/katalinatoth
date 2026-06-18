# How to Update Your Website

All changes auto-deploy within ~2 minutes of pushing to the `main` branch. You can edit files directly on GitHub in the browser — no local tools needed.

---

## Add a New Paper

1. Open `data/papers.yaml`
2. Add a new entry at the top:

```yaml
- title: "Your Paper Title"
  authors: ["Katalina Toth", "Coauthor Name"]
  year: 2026
  status: "working paper"
  venue: ""
  pdf: "/files/your-paper.pdf"
  link: ""
  abstract: "One sentence description."
  job_market_paper: false
  tags: ["health policy"]
```

3. If you have a PDF, upload it to `static/files/`
4. Commit and push — the site rebuilds automatically

**Status options:** `published`, `accepted`, `revise and resubmit`, `under review`, `working paper`, `work in progress`

---

## Mark a Paper as Published

In `data/papers.yaml`, change:
- `status:` from `"working paper"` to `"published"`
- Add `venue: "Journal Name"`
- Add `link:` with the DOI or publisher URL

---

## Designate Your Job Market Paper

In `data/papers.yaml`, set `job_market_paper: true` on the relevant entry. It will appear in a highlighted card at the top of the Research section.

---

## Update Your Bio

Edit `content/_index.md`. The text between the `---` markers (front matter) and the end of the file is your bio, written in Markdown.

---

## Add a Teaching Entry

Open `data/teaching.yaml` and add:

```yaml
- course: "Course Name"
  role: "Teaching Fellow"
  institution: "Harvard University"
  term: "Fall 2026"
  instructor: "Prof. Name"
```

---

## Add a Blog Post

1. Create a new folder: `content/blog/your-post-slug/`
2. Inside it, create `index.md`:

```yaml
---
title: "Your Post Title"
date: 2026-06-01
description: "One-sentence summary."
tags: ["topic"]
---

Your post content in Markdown here.
```

---

## Update Your CV

Replace `static/files/cv.pdf` with the new version. Keep the same filename so existing links don't break.

---

## Change Your Photo

Replace `static/images/photo.jpg` with the new photo. Keep the same filename.

---

## Add an Award

Open `data/awards.yaml` and add:

```yaml
- name: "Award Name — brief description"
  year: "2026"
```

---

## Add a Presentation

Open `data/presentations.yaml` and add:

```yaml
- title: "Talk Title"
  authors: ["Katalina Toth", "Coauthor"]
  venue: "Conference Name, City"
  date: "2026"
```

---

## Change Site Metadata

Edit `hugo.yaml` to update your email, tagline, description, or navigation menu items.
