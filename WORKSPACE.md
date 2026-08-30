# Workspace: Jaeyoung Lee Portfolio

← [Portfolio repository](README.md)

## Contract

- Purpose: maintain a public researcher portfolio and its public-safe content pipeline.
- Owns: Hugo source, public content, site-specific design and templates, verified
  publication facts, content planning, build and deploy configuration, and target-local
  WOS coordination.
- Does not own: RTCL research state, lab-internal evidence, other project repositories,
  shared WOS semantics, deployed-WOS registry state, or GitHub Pages runtime state.
- Decision owner: user.
- Parent / inheritance: repository `AGENTS.md` and any higher-priority adopted runtime
  instructions apply together; publication privacy and deploy gates remain binding.

## Entry points

- Human: `README.md`
- Agent guidance: `AGENTS.md`
- Workspace hub: `00-workspace/README.md`
- Current coordination: `00-workspace/workstream/README.md`
- Hugo operations: `docs/project_guide.md`

## Domain bindings

- Public-site content model: `docs/Explanation.md`
- Verified publication facts and approval state: `docs/context_intake.md`
- Detailed content plan and candidate inventory: `docs/content_outline.md`
- Historical raw outline input: `docs/content_outline_raw.md`
- Public content: `content/`
- Templates and shortcodes: `layouts/`
- Static public assets: `static/`
- Hugo configuration: `hugo.toml`
- Build and deploy workflow: `.github/workflows/hugo-pages.yml`
- Ignored private source context: `docs/context/`

The fact table, content plan, site design, code, templates, and generated site are domain
artifacts. They are not Workstream records merely because they contain open questions or
implementation detail.

## WOS artifact bindings

- Workstream records: `00-workspace/workstream/records/`
- Decision maps: `00-workspace/workstream/maps/`
- Guides: `00-workspace/workstream/guides/`
- Log: `00-workspace/workstream/log/daily/`

No target-local WOS Design, Durable Decision, Glossary, or Reference binding is active.
Create one only when confirmed content requires that role; do not alias domain documents
into it.

## Runtime bindings

- Managed Transit: `00-workspace/.transit/`
- Ignored Hugo output: `public/`
- Ignored Hugo lock and resources: `.hugo_build.lock`, `resources/`

Transit is temporary context-package state. Generated Hugo output and raw source context
are not WOS memory and must not be staged.

## External bindings

- WOS deployment observation:
  `/home/sleepylee/Desktop/0imoy/00-dashboard/wos/`
- Shared WOS design:
  `/home/sleepylee/Desktop/0imoy/01-moi/computer_and_me/my_overall_system/workstream_operating_system/`

External writes, commit, push, deployment, repository-setting changes, and history
rewrites each require their own applicable authority and verification.
