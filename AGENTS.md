# Repository Guidelines

## Project Structure & Module Organization

This repository is a Hugo portfolio and study archive. Site content lives in `content/`: section landing pages use `_index.md`, project entries belong in `content/projects/`, and dated research notes belong in `content/study/`. Put images, PDFs, favicons, and downloadable files in `static/`; Hugo serves them from the site root. Repository-specific templates and shortcodes live in `layouts/`, while `themes/terminal/` contains the upstream theme and should be edited only when an override cannot solve the problem. `hugo.toml` controls navigation and site settings. Planning, fact verification, and maintenance records are kept in `docs/`.

## Build, Test, and Development Commands

- `hugo server` starts the local preview at `http://localhost:1313/` and rebuilds on changes.
- `hugo` creates the production output in `public/` and catches template or content build errors.
- `hugo --destination /tmp/hugo-check` performs an isolated validation build without changing repository output.
- `hugo --gc --minify` approximates the GitHub Pages production build.

Use Hugo Extended 0.123.7 when matching CI. Pushes to `main` deploy through `.github/workflows/hugo-pages.yml`.

## Coding Style & Naming Conventions

Write concise Markdown with YAML front matter (`title`, `date`, and `draft`). Use two-space indentation in TOML/YAML where nesting is needed. Name project files with lowercase kebab case, such as `gpu-batching-prototype.md`; prefix study notes with an ISO date, such as `2026-03-17-topic.md`. Prefer repository-level overrides in `layouts/` and keep Go-template logic small. Follow existing CSS formatting in `static/*.css`; no repository-wide formatter is configured.

## Testing Guidelines

There is no automated unit-test or coverage framework. Before committing, run an isolated Hugo build and inspect affected pages locally, including navigation, links, images, PDF previews, responsive layout, and draft visibility. Treat warnings and broken internal links as defects.

## Content Workflow & Safety

For content changes, follow `docs/rules.md`: verify facts in `docs/context_intake.md`, map them in `docs/content_outline.md`, update `content/`, validate the build, then add a one-line result to `docs/progress.md`. Do not publish student IDs, personal contact details, schedule logistics, or non-public lab information.

## Commit & Pull Request Guidelines

History uses short, lowercase, imperative summaries (for example, `featured project cleaned`). Prefer a more specific equivalent, such as `add PDF preview shortcode`, and keep each commit focused. Pull requests should explain the visible change, list validation commands, link relevant issues, and include screenshots for layout or styling changes. Call out configuration, navigation, or deployment changes explicitly.
