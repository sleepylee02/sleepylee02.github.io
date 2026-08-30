# Project Guide: sleepylee02.github.io

Operational guide for maintaining this Hugo-based portfolio site.

## 1. Project Overview
- Type: Static Site Generator (Hugo)
- Theme: `terminal`
- Deployment target: GitHub Pages
- Site positioning: researcher portfolio + curated current research overview

## 2. Current Navigation and Content Model

Main menu (from `hugo.toml`):
- `/`
- `/about/`
- `/research/`
- `/projects/`
- `/contact/`

Content sections (under `content/`):
- `content/_index.md`: Home
- `content/about/_index.md`: About
- `content/projects/`: Project pages
- `content/research/_index.md`: Curated current research direction
- `content/contact/_index.md`: Contact links

## 3. Directory Structure and Ownership

| Directory/File | Purpose |
| :--- | :--- |
| `README.md` | Stable human entry to the repository and its owners. |
| `WORKSPACE.md` | Purpose, ownership boundary, and final domain/WOS bindings. |
| `00-workspace/` | Target-local WOS coordination, Guides, records, logs, maps, and ignored Transit. |
| `hugo.toml` | Main site configuration (title, params, menu). |
| `content/` | Public page content in Markdown. |
| `docs/` | Domain docs for content design, fact verification, and detailed planning. |
| `00-workspace/workstream/guides/content-update.md` | Public-content update procedure, privacy rules, and done criteria. |
| `docs/Explanation.md` | Content strategy and section philosophy. |
| `docs/context_intake.md` | Verified facts extracted from `docs/context/*` before publishing. |
| `docs/content_outline.md` | Detailed content mapping and candidate inventory; not active Workstream state. |
| `00-workspace/workstream/README.md` | Current Attention and Workstream lifecycle view. |
| `00-workspace/workstream/log/` | Material coordination chronology. |
| `archetypes/default.md` | Default front matter template for new content. |
| `static/` | Static assets served as-is (files, images, favicon). |
| `themes/terminal/` | Theme source. Avoid direct edits unless necessary. |
| `layouts/` | Override templates if theme customization is needed. |

## 4. Content Writing Workflow

When adding content, follow
`00-workspace/workstream/guides/content-update.md`. The domain-level sequence is:

1. Extract/verify facts in `docs/context_intake.md`.
2. Decide the target section (`research`, `about`, `projects`, `contact`).
3. Create a Markdown file with front matter:
```markdown
---
title: "Page Title"
date: 2026-02-16
lastmod: 2026-08-24
draft: false
---
```
4. Keep section intent aligned with `docs/Explanation.md`.

Freshness metadata:
- `date` records when the page was first created or published.
- `lastmod` records the most recent meaningful content review.
- Hugo resolves `lastmod` only from the explicit front matter field; it does not fall back to `date`.
- Update `lastmod` after factual or editorial review, not for styling, build, or typo-only changes.
- Project completion state uses separate `project_status` and `project_year` fields.

Recommended patterns:
- Projects: problem, approach, trade-offs, result, lesson.
- Research: current question, evidence boundary, public-safe trajectory, and stable selected artifacts only.

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

### GitHub Pages Deployment (GitHub Actions)
- Workflow file: `.github/workflows/hugo-pages.yml`
- Trigger: push to `main` (and manual run via `workflow_dispatch`)
- Build: Hugo Extended with theme submodules checked out
- Deploy: artifact upload + `actions/deploy-pages`

Required one-time repository setting:
1. Go to `Settings` -> `Pages`.
2. Set `Source` to **GitHub Actions**.

After this, pushes to `main` deploy the latest Hugo build automatically.

## 6. Notes and Maintenance Rules
- `public/` is build output and is ignored by Git.
- `.hugo_build.lock` is a temporary lock file and is ignored by Git.
- Keep domain content design, fact verification, and detailed planning in `docs/`.
- Keep current checkpoints, Guides, and material coordination logs under `00-workspace/`.
- Never recreate a parallel current-state or progress-log authority under `docs/`.
- `docs/context/` is ignored private source material; never stage or copy it without
  exact fact extraction and public-safety review.
- If site structure changes, update `docs/Explanation.md` first, then reflect in `content/` and `hugo.toml`.

---
Update this file whenever structure, workflow, or maintenance policy changes.
