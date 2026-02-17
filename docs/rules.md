# Working Rules

This document defines how to work in this repository when multiple internal docs are interconnected.
Core planning and structure documents should be in English, while source notes in `docs/context/*` may remain in Korean.

## 1. Read Order (Start Here)
Before starting any new task, read files in this order:
1. `docs/rules.md`
2. `docs/project_guide.md`
3. `docs/Explanation.md`
4. `docs/context_intake.md`
5. `docs/content_outline.md`
6. `docs/progress.md`

## 2. Document Roles (Single Source of Truth)
Each document has a fixed role:

- `docs/rules.md`: working rules, read order, done criteria
- `docs/project_guide.md`: technical operations (Hugo, structure, commands)
- `docs/Explanation.md`: site philosophy and section intent
- `docs/context_intake.md`: verified fact extraction from raw context
- `docs/content_outline.md`: current-cycle content plan
- `docs/progress.md`: in-progress and completed logs
- `docs/context/*`: source notes, drafts, interview preparation material

## 3. Workflow Rules
Follow this sequence for content work:

1. Collect raw material from `docs/context/*`
2. Extract and verify facts in `docs/context_intake.md`
3. Map validated facts to target pages in `docs/content_outline.md`
4. Apply updates in `content/` (`home/about/projects/study/contact`)
5. Validate locally (`hugo` or `hugo --destination /tmp/hugo-check`)
6. Add a one-line result entry to `docs/progress.md`

## 4. Content Rules
Keep section intent stable:

- Home: 30-second introduction, core focus, entry links
- About: concise profile summary
- Projects: problem, approach, trade-offs, result, lessons, and at least one metric when possible
- Study: weekly log format (PPT plus short notes)

## 5. Privacy and Publishing Rules
Before publishing, always check:

- Remove sensitive personal details (student ID, personal contacts, schedule logistics)
- Remove lab-internal or non-public implementation details
- Link or attach only publishable materials

## 6. Definition of Done (Per Update Cycle)
A cycle is complete only when:

1. Target items in `docs/content_outline.md` are reflected in content
2. `content/` renders without build errors
3. Completion is logged in `docs/progress.md`
