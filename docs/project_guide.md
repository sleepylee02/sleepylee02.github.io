# Project Guide: sleepylee02.github.io

Operational guide for maintaining this Hugo-based portfolio site.

## 1. Project Overview
- Type: Static Site Generator (Hugo)
- Theme: `terminal`
- Deployment target: GitHub Pages
- Site positioning: portfolio + weekly research log (not a traditional blog)

## 2. Current Navigation and Content Model

Main menu (from `hugo.toml`):
- `/about/`
- `/projects/`
- `/research/`
- `/timeline/`
- `/contact/`

Content sections (under `content/`):
- `content/_index.md`: Home
- `content/about/_index.md`: About
- `content/projects/`: Project pages
- `content/research/`: Weekly research logs
- `content/timeline/`: Growth narrative
- `content/contact/_index.md`: Contact links

## 3. Directory Structure and Ownership

| Directory/File | Purpose |
| :--- | :--- |
| `hugo.toml` | Main site configuration (title, params, menu). |
| `content/` | Public page content in Markdown. |
| `docs/` | Internal docs for planning/operation. |
| `docs/rules.md` | Working contract: read order, behavior rules, done criteria. |
| `docs/Explanation.md` | Content strategy and section philosophy. |
| `docs/context_intake.md` | Verified facts extracted from `docs/context/*` before publishing. |
| `docs/progress.md` | Progress tracking and completion log. |
| `archetypes/default.md` | Default front matter template for new content. |
| `static/` | Static assets served as-is (files, images, favicon). |
| `themes/terminal/` | Theme source. Avoid direct edits unless necessary. |
| `layouts/` | Override templates if theme customization is needed. |

## 4. Content Writing Workflow

When adding content:
1. Extract/verify facts in `docs/context_intake.md`.
2. Decide the target section (`about`, `projects`, `research`, `timeline`, `contact`).
3. Create a Markdown file with front matter:
```markdown
---
title: "Page Title"
date: 2026-02-16
draft: false
---
```
4. Keep section intent aligned with `docs/Explanation.md`.

Recommended patterns:
- Projects: problem, approach, trade-offs, result, lesson.
- Research log: papers read, current interests, short diary notes, PPT/PDF link.

## 5. Development Workflow

Run locally:
```bash
hugo server
```
Local URL: `http://localhost:1313/`

Build check:
```bash
hugo
```

Optional isolated build output:
```bash
hugo --destination /tmp/hugo-check
```

## 6. Notes and Maintenance Rules
- `public/` is build output and is ignored by Git.
- `.hugo_build.lock` is a temporary lock file and is ignored by Git.
- Keep internal planning documents in `docs/`.
- If site structure changes, update `docs/Explanation.md` first, then reflect in `content/` and `hugo.toml`.

---
Update this file whenever structure, workflow, or maintenance policy changes.
