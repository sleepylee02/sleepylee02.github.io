# Progress Log

This file tracks current work status and short completion summaries.

## How To Use
- Update `In Progress` when a task starts or status changes.
- Add one line to `Completed Log` when a task is done.
- Keep each entry short (1-3 lines max).

## In Progress
| Date | Task | Status | Next Action |
|---|---|---|---|
| 2026-02-16 | Align site structure with `docs/Explanation.md` | Done | Start filling real content |
| 2026-02-16 | Convert `docs/context` notes into publishable content plan | In Progress | Apply outline to Home/About/Projects/Study pages |
| 2026-02-16 | Establish accurate context-intake process | Done | Confirm open decisions and start project page drafting |
| 2026-02-16 | Prepare provisional dataset from context notes | Done | Owner review and finalize decision locks |
| 2026-02-16 | Apply full context-based content update | Done | Add project metrics and confirm final factual locks |
| 2026-02-16 | Apply second-pass context enrichment | Done | Finalize factual confirmations and trim/edit copy tone |
| 2026-02-16 | Switch deployment mode to GitHub Actions | Done | Set GitHub Pages source to GitHub Actions in repository settings |
| 2026-02-16 | Rename Research section to Study section | Done | Review wording consistency and confirm final labels |
| 2026-02-16 | Automate recent Study list on Home | Done | Confirm top-3 auto rendering after each new study post |

## Completed Log
| Date | What Was Done | Short Summary |
|---|---|---|
| 2026-02-17 | Removed legacy section | Deleted the legacy section directory, removed its menu entry and links, and aligned docs to the new structure |
| 2026-02-16 | Reworked site structure and content templates | Menu changed to `about/projects/study`; seeded `content/` with starter pages and templates |
| 2026-02-16 | Removed old pages | Deleted `content/interests.md` and `content/reading.md` |
| 2026-02-16 | Organized context notes into structured outline | Parsed 3 context files and regenerated `docs/content_outline.md` via pipeline |
| 2026-02-16 | Added context verification layer | Created `docs/context_intake.md` and connected it to rules/guide/outline workflow |
| 2026-02-16 | Expanded context intake and prioritized execution | Added fact IDs `F-001` to `F-012`, provisional draft pack, and execution order in `docs/content_outline.md` |
| 2026-02-16 | Added dedicated Contact tab | Created `content/contact/_index.md`, added `/contact/` menu entry, and moved contact links into one page |
| 2026-02-16 | Applied context-based updates across public pages | Updated Home/About, added 3 context-grounded project pages, and added one real-time study log |
| 2026-02-16 | Enriched pages directly from context details | Added systems coursework in About, expanded project-history list, and deepened growth narrative notes |
| 2026-02-16 | Fixed menu order regression | Added explicit menu `weight` values in `hugo.toml` so Contact stays last |
| 2026-02-16 | Added GitHub Actions Pages workflow | Added `.github/workflows/hugo-pages.yml` and documented one-time Pages setting update |
| 2026-02-16 | Completed Study naming migration | Renamed menu/section/path from `research` to `study`, moved `content/research` to `content/study`, and updated docs/content links |
| 2026-02-16 | Added dynamic "Recent Study Notes" list on Home | Added `layouts/shortcodes/recent-study.html` and switched Home to auto-list latest 3 study posts |

## Next Candidates
- Replace sample text in `content/projects/gpu-batching-prototype.md` with real metrics.
- Add weekly study logs from recent advisor presentations.
