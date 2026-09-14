# Content Outline

Status: current domain content plan and candidate inventory

This file owns detailed page mapping and publication candidates. It does not own Current
Attention, an active checkpoint, or a next action; those belong to
`00-workspace/workstream/README.md` and its bound record.

Initially generated from `docs/content_outline_raw.md` on 2026-02-17. That raw input is
now historical; later confirmed updates in this file supersede its Study-era vocabulary.

## 1. Current Goal
- Keep Home legible as a 30-second researcher introduction.
- Present one curated Research page and a prioritized project list.
- Keep About concise with only short growth context.
- Show explicit freshness metadata on Research, About, Projects, and reviewed individual project pages.
- Keep Research and Projects visually consistent with About through standard headings, lists, and horizontal dividers.
- Use a restrained title-summary-metadata pattern only for repeated Research Areas and Selected Work entries.

## 2. Source Context Inbox
- docs/context/abt myself (portfolio).md
- docs/context/rtcl-meeting-prep.md
- docs/context/prof-contact-email.md

## 2.1 Verified Fact Baseline
- Use verified items from `docs/context_intake.md` (e.g., `F-001` to `F-013`).
- Do not publish unverified statements without owner confirmation.

## 2.2 Historical Provisional Execution Order

The following 2026-02-16 order is retained as domain planning history. It is not a live
execution queue.

1. Finalize Home and About copy from `F-001`, `F-003`, `F-005`.
2. Build two full project pages first from `F-004`, `F-009` (Inference server and S3-FIFO).
3. Add one additional project (ROS2+YOLO or Uber pipeline) after metric availability check.
4. Keep weekly research records private; publish only selected milestones when they become stable.

## 3. Mapping Plan (Source -> Target Page)

### Home (`content/_index.md`)
- One-line role: Undergraduate Researcher · Real-Time Systems.
- Affiliation: Yonsei Real-Time Computing Lab (RTCL@Yonsei).
- Research identity: predictable and reliable execution under timing and resource constraints, with robotic systems as the current focus.
- Current Research summary: connect real-time systems, probabilistic timing analysis, and VLA runtime safety; frame the active problem around coordinating inference, robot execution, monitoring, and recovery before intervention becomes ineffective.
- Use `Current Research` as the heading for the active-area summary.
- Expand VLA to vision-language-action (VLA) at its first Home mention (F-045).
- Supply `Real-Time Systems · Robotics` as the Home search and Open Graph description through the theme's `params.subtitle` setting. Retain the original blue-pattern sharing image without added text (F-045).
- Add Personal AI Work & Knowledge System as the third Selected Work entry, using the same integrated overview as Projects (F-038 to F-041).
- Rely on the primary navigation and section-specific links instead of repeating the site menu beneath the Home profile.

### About (`content/about/_index.md`)
- Education: Yonsei University (2021-current), Applied Statistics major + Computer Science double major.
- Keep only concise profile, focus, and key experiences.
- Let Home carry the primary portrait; begin About directly with the profile narrative instead of repeating the same image.
- Experience highlights: YBIGTA vice president and data engineering team leadership.
- Preserve the introduction verbatim, followed by Experience & Leadership, Education, and How I Think in that order. Remove Research Interests and move Systems Background to Research to consolidate the technical overview (F-044).
- End About after `How I Think`; keep email and profile links on the dedicated Contact page.

### Projects (`content/projects/`)
- Show `Last updated` on the section page; show completion year and `Last updated` separately on reviewed individual projects.
- Feature ROBO 404++, the Uber-style distributed data pipeline, and Personal AI Work & Knowledge System on both Home and Projects, covering physical robotics, data infrastructure, and personal AI workflows.
- Explain the integrated Selected Work entry through its roles: resuming work across sessions, organizing and reusing knowledge, and navigating project context. Show the full component names as plain-text metadata beneath the summary: Workstream Operating System, AI-Assisted Knowledge Wiki, and Personal Dashboard. Do not turn these labels into links (F-043).
- Keep Workstream Operating System (WOS), AI-Assisted Knowledge Wiki (LLM-Wiki), and Personal Dashboard as three separate [26-S] entries at the start of AI Applications in Additional Work. The integrated Selected Work summary explains their relationship; this update adds no dedicated project page (F-038 to F-041).
- Order Additional Work as Robotics, Systems & Infrastructure, AI Applications, then Data Analysis & Forecasting. Split the former Robotics & AI Applications group: the two robot projects stay in Robotics; NotebookLocal, the legal agent, the form-filling agent, and the restaurant recommendation service join the three personal systems in AI Applications (F-042).
- Retain the robotics and data-pipeline entries in the domain-grouped Additional Work list as part of the complete chronology.
- Add AMIRec [26-1], Home Inference Server Setup [25-1], ROBO 404++ [26-1], and the New-Town traffic-safety analysis [25-W] as concise entries in their respective Additional Work groups; ROBO 404++ may also appear in Selected Work as the representative implementation.
- Use a variable-length muted metadata line for evidence-backed implementation details; do not pad to a fixed tag count, repeat the title, or add a line when no useful verified detail is available.
- Rename the former meal-recommendation entry to `RAG-Based Restaurant Recommendation Service` and simplify the baseball and form-filling titles to match the verified work.
- Priority 1: Home inference server setup (DeepSeek operation, 25-1).
- Priority 2: Implementing S3-FIFO cache algorithm (25-1).
- Priority 3: ROS2 + YOLO hazard detection robot system (25-2).
- Backup: Uber data pipeline project (25-W).
- Keep project pages in a common structure: problem, approach, trade-offs, results, lessons.
- Add at least one verified metric per featured project (latency, throughput, scale, reliability) when developed into a detail page. The current Personal AI Work & Knowledge System listing stays at overview level without a performance claim.

### Research (`content/research/_index.md`)
- Show `Last updated` beneath the page title using the shared month-and-year format.
- Preserve the introduction and remove the Current Research Question section, including its three investigation axes (F-044).
- Keep Research Areas in the existing order with unchanged descriptions: Real-Time Systems; Probabilistic Timing Analysis; VLA & Robotic Systems.
- Label VLA & Robotic Systems as `Current Focus`, and retain ML for RT and RT for ML as the existing connecting paragraph.
- Place Systems Background after Research Areas and the connecting paragraph, before Research Trajectory. Reuse the three existing About bullets verbatim, without an introductory sentence.
- End with a concise Research Trajectory that connects scheduling and probabilistic timing analysis to ML workloads, VLA runtime monitoring, and safety.
- Close Research Trajectory with the owner-confirmed long-term aim of making real-time systems a practical foundation for reliable robotic intelligence.
- Keep discarded hypotheses and candidate runtime diagnostics out of the overview until they are supported by a stable public milestone.

## 4. Candidate Gaps and Questions

These items are not active Workstreams until the user selects a bounded effort.

- Home and Projects feature ROBO 404++, the Uber-style distributed data pipeline, and Personal AI Work & Knowledge System.
- Public pages are currently written in English.
- Confirm exact end date for YBIGTA data engineering team leader role (provisional: 2026.06).
- Add concrete metrics to project pages (throughput, latency, reliability) for stronger evidence.

## 5. Private Review Checklist
- Do not publish student ID, private email exchange details, or scheduling logistics.
- Remove lab-internal or non-public implementation details before publishing.

## 6. Done in This Cycle
- [x] Home updated
- [x] About updated
- [x] Projects updated
- [x] Public Study archive replaced by a curated Research page

## 7. Parked Projects and Research Review (2026-07-30 Historical Checkpoint)

Status: Superseded on 2026-08-24. The Research page and featured-project selection are applied in the `researcher-redesign` branch; the remaining notes below are retained as historical review context.

### Project Candidates to Reassess

- ROS2 + YOLO: verify the implementation artifacts and the recorded `10 Hz` to `30+ Hz` improvement before using it publicly.
- Uber Data Pipeline: verify the architecture, individual contribution, and recorded `10,000+ events/s` result.
- Third featured slot: compare Home Inference Server and NotebookLocal based on available code, architecture, measurements, and public artifacts.
- S3-FIFO: keep as a supporting project candidate.
- GPU Batching Prototype: keep on hold until a real implementation and measurements are located.
- PRTG-VLA: keep under Research until a stable experiment result supports promotion to Projects.

### Research Milestone Candidates

- `From Probabilistic Timing Guarantees to VLA Temporal Validity`
- `Profiling pi0.5 Inference on LIBERO`
- `When Does VLA Latency Become a Safety Problem?`

Use public-safe milestone summaries only after a result is stable enough to explain. Do not automatically publish meeting records or lab-internal artifacts.

### Historical Resume Point

This resume point belonged to the superseded 2026-07-30 checkpoint. Do not use it as
current execution state.

1. Recheck the live repository and current research state.
2. Verify the evidence and public safety of the project candidates.
3. Select only two or three featured projects with the owner.
4. Confirm which, if any, milestones are stable enough to add beneath the Research overview.
