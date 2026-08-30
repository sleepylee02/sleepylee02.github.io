# Guide: Portfolio Content Update

← [Portfolio Workstreams](../README.md)

Use this procedure for public content changes in this repository. Current effort status
belongs to the bound Workstream record, not to the content plan or fact registry.

## Read order

1. `WORKSPACE.md`
2. `00-workspace/workstream/README.md` and its Current Attention record, if any
3. `docs/project_guide.md`
4. `docs/Explanation.md`
5. `docs/context_intake.md`
6. `docs/content_outline.md`
7. only the raw `docs/context/*` source needed for the authorized update

## Workflow

1. Select the exact public page and bounded change.
2. Extract or verify facts in `docs/context_intake.md`; do not infer missing claims.
3. Map validated facts and editorial intent in `docs/content_outline.md` when the plan
   materially changes.
4. Update the relevant file under `content/`, `layouts/`, `static/`, or `hugo.toml`.
5. Build into a fresh temporary destination and inspect affected pages, navigation,
   links, images, responsive layout, freshness metadata, and draft visibility.
6. Update the active Workstream record when its checkpoint or next action changes. Add a
   daily log entry only for a material chronological change.

A small content correction does not require inventing a Workstream. A multi-session
refresh requires one record with one canonical checkpoint.

Keep tracked structure, planning documents, and public pages in English. Korean may
remain in ignored raw `docs/context/` notes until facts are extracted and rewritten for
the public surface.

## Section intent

- Home: 30-second introduction, current focus, and entry links
- Research: curated current question, trajectory, and public-safe framing
- About: concise public profile
- Projects: problem, approach, trade-offs, result, lessons, and evidence-backed metrics
- Contact: public professional contact links only

## Privacy and publishing

Before any tracked change or push:

- remove student IDs, private contact exchanges, schedule logistics, credentials, and
  non-public lab information;
- never copy ignored `docs/context/` content into a WOS record, log, Transit packet, or
  public page without explicit fact extraction and redaction;
- link or attach only publishable material;
- remember that repository Markdown is public source even when Hugo does not render it.

## Definition of done

A bounded update is complete only when:

1. the intended public content and any required domain plan/fact updates agree;
2. an isolated Hugo build succeeds without relevant warnings;
3. affected pages receive visual and link review;
4. the active Workstream checkpoint and material log are updated when applicable;
5. the diff contains no ignored output, private source context, unrelated change, or
   unauthorized deployment action.

Commit, push, GitHub Pages settings, workflow dispatch, live deployment verification,
and history remediation are separate gates.
