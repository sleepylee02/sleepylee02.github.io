# AGENTS.md - Jaeyoung Lee Portfolio

## Role

This agent works for the Hugo portfolio repository. It maintains public-safe site
content, site-specific design and implementation, build validation, and target-local WOS
coordination.

It does not own RTCL research state, lab-internal evidence, other repositories, shared
WOS semantics, deployed-WOS registry state, GitHub Pages settings, or live deployment
state. Keep those artifacts with their canonical owners and point to them instead of
copying their checkpoint or private content here.

Higher-priority runtime instructions, sandbox permissions, approvals, and explicitly
adopted owner rules remain binding.

## Read order

For repository work, read:

1. `README.md`
2. `WORKSPACE.md`
3. `00-workspace/workstream/README.md`
4. the Current Attention record, when one exists
5. `docs/project_guide.md`
6. only the content model, fact registry, content plan, Guide, source, template, or
   implementation file needed for the request

Use `00-workspace/workstream/guides/content-update.md` for public content changes. Raw
`docs/context/` files are ignored private inputs and are not part of ordinary discovery.

## Ownership and routing

- Public pages and project entries → `content/`
- Site content model → `docs/Explanation.md`
- Verified publication facts and approval state → `docs/context_intake.md`
- Detailed page mapping and candidates → `docs/content_outline.md`
- Hugo structure, commands, and deploy description → `docs/project_guide.md`
- Current checkpoint and next action → one bound Workstream record
- Material chronological coordination change → `00-workspace/workstream/log/daily/`
- Temporary context package → `00-workspace/.transit/`; never canonical state

Do not treat an open fact question, content candidate, draft page, or generated site as
an active Workstream. Do not recreate a parallel current-state list or progress ledger.

## Project structure

Section landing pages use `_index.md`. Project entries belong in `content/projects/`, and
the curated research overview is `content/research/_index.md`. There is no current public
weekly-note archive or separate Study writing path.

Put public images, PDFs, favicons, and downloadable files in `static/`. Repository
templates and shortcodes live in `layouts/`. `themes/terminal/` is an upstream submodule;
prefer repository-level overrides and do not modify or update the submodule without an
explicit request. `hugo.toml` controls navigation and site settings.

## Style and conventions

Write concise Markdown with YAML front matter such as `title`, `date`, `lastmod`, and
`draft`. Use two-space indentation where TOML or YAML nesting needs it. Name project
files with lowercase kebab case, such as `gpu-batching-prototype.md`.

Prefer repository-level overrides in `layouts/` and keep Go-template logic small. Follow
the existing formatting in `static/*.css`; no repository-wide formatter is configured.
Update `lastmod` only after meaningful factual or editorial review, not for build,
styling, or typo-only changes.

## Content and privacy

Verify public claims in `docs/context_intake.md` and map material editorial changes in
`docs/content_outline.md` before editing public copy. Never publish or copy into tracked
WOS artifacts:

- student IDs or private contact exchanges;
- schedule logistics, credentials, addresses, or operational access details;
- non-public lab information or raw experiment material;
- ignored `docs/context/` text that has not passed exact fact extraction and redaction.

Repository Markdown is public source even when Hugo does not render it. A privacy review
is therefore required before staging tracked documentation, not only before editing
`content/`.

## Build and verification

Use Hugo Extended 0.123.7 when matching CI. Prefer a fresh temporary destination so stale
ignored `public/` output cannot satisfy validation.

```bash
verify_root=$(mktemp -d /tmp/portfolio-verify.XXXXXX)
hugo --cacheDir "$verify_root/cache" \
  --destination "$verify_root/site" \
  --cleanDestinationDir --minify --panicOnWarning --printPathWarnings
```

Inspect affected pages locally, including navigation, internal links, images, responsive
layout, freshness metadata, draft visibility, and any intentional public downloads.
Treat warnings and broken internal links as defects. There is no automated unit-test or
coverage framework.

## Authority and deploy boundary

Read-only inspection or diagnosis does not authorize writes. An explicit bounded request
authorizes only the described repository paths and change. Move, delete, broad content
rewrite, privacy-sensitive source use, repository settings, history remediation, and
external-owner changes require exact scope and applicable confirmation.

Pushes to `main` can deploy through `.github/workflows/hugo-pages.yml`. Local build,
commit, push, workflow success, and live-site verification are separate gates. Do not
push, dispatch a workflow, modify Pages settings, or claim deployment success without
the corresponding authority and evidence.

Preserve ignored raw context, generated output, the theme submodule, and unrelated or
other-session changes.

## Completion and Git

Before completing a material change:

1. verify `README -> WORKSPACE -> Workstream index -> Current Attention record`;
2. run the target-specific Hugo and visual checks;
3. confirm no private source, ignored output, unrelated change, or stale live authority
   is included;
4. update the current record and material daily log when applicable;
5. run `git diff --check` and inspect the full task-owned diff.

Stage only task-owned explicit paths with `git add -- <paths>`; never use broad staging
commands by default. Do not stage unrelated changes. Before every commit, show the staged
scope and proposed short imperative message for approval. Commit approval does not
authorize push, deployment, amend, rebase, or history rewrite.

History uses short, lowercase, imperative summaries. A pull request should explain the
visible change, list validation commands, link relevant issues, include screenshots for
layout or styling changes, and call out configuration, navigation, or deployment changes.
