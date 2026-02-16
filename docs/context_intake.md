# Context Intake

Use this document to extract accurate, publish-ready facts from `docs/context/*` before writing or editing `content/*`.

## 1. Purpose
- Prevent guesswork when converting raw notes into public content.
- Separate verified facts from assumptions and personal drafts.
- Keep a clear audit trail from source notes to published pages.

## 2. Intake Workflow
1. Read relevant files in `docs/context/*`.
2. Extract facts into the table below with source references.
3. Mark publish safety and confidence level for each fact.
4. Resolve open questions with the owner.
5. Move validated facts into `docs/content_outline.md`.

## 3. Fact Table (Source of Truth)
| ID | Source File | Source Snippet/Section | Extracted Fact | Confidence | Publish Safe | Target Page | Owner Confirmed | Notes |
|---|---|---|---|---|---|---|---|---|
| F-001 | `docs/context/abt myself (portfolio).md` | Who am I > Education | Yonsei University (2021-current), Applied Statistics major, CS double major | High | Yes | About, Home | No | Confirm preferred wording |
| F-002 | `docs/context/abt myself (portfolio).md` | Experience | YBIGTA vice president (2025.06-2025.12), DE team lead (2025.12-2026.06) | Medium | Yes | About, Timeline | No | Confirm exact end date |
| F-003 | `docs/context/rtcl-meeting-prep.md` | Interest motivation | Interest shifted from data analysis to systems/real-time constraints | High | Yes | Home, Timeline | No | Keep concise |
| F-004 | `docs/context/prof-contact-email.md` | Project list | Home inference server, S3-FIFO, ROS2+YOLO, data pipeline projects | Medium | Yes | Projects | No | Add metrics before publish |
| F-005 | `docs/context/abt myself (portfolio).md` | Interest / Research Interests | Core interests include OS, distributed/parallel systems, real-time systems, AI serving, system architecture | High | Yes | Home, About, Research | No | Can be published as focus areas |
| F-006 | `docs/context/abt myself (portfolio).md` | Past narrative | Post-military return led to data/ML projects, then focus shifted to throughput, parallel execution, and systems-level efficiency | Medium | Yes | Timeline | No | Keep timeline concise and date-anchored |
| F-007 | `docs/context/rtcl-meeting-prep.md` | Career direction | Prefers research-oriented path; plans to pursue MS and decide on PhD after research experience | Medium | Yes | Timeline | No | Publish as direction, not commitment |
| F-008 | `docs/context/abt myself (portfolio).md` | Lectures (CS) | Completed core systems-related courses: OS, System Programming, Real-Time System, Computer Network, Distributed Training and Inference | High | Yes | About, Timeline | No | Avoid listing too many courses on public pages |
| F-009 | `docs/context/abt myself (portfolio).md` | Projects | Project history spans data analysis, agent applications, inference setup, ROS, and data pipeline work | High | Yes | Projects, Timeline | No | Use 2-3 representative projects first |
| F-010 | `docs/context/rtcl-meeting-prep.md` | Real-time interest details | Strong interest in constrained scheduling and deadline/accuracy trade-offs in AI inference tasks | High | Yes | Research, Timeline | No | Good anchor for weekly research logs |
| F-011 | `docs/context/rtcl-meeting-prep.md` | ROS/RT interest | Interest in OS-level real-time guarantees for ROS and embedded/edge scenarios | Medium | Yes | Research, Projects | No | Keep claims directional unless validated by project artifacts |
| F-012 | `docs/context/rtcl-meeting-prep.md` | Data engineering reflection | Data engineering is useful but currently viewed as less aligned with intended research depth | Medium | Yes | Timeline | No | Phrase as personal preference, not absolute claim |

Confidence rule:
- `High`: explicitly stated in source, no ambiguity
- `Medium`: stated but needs date/scope clarification
- `Low`: inferred from context, needs confirmation

## 4. Decision Locks (Must Confirm Before Publish)
| Decision | Current Value | Status | Owner Confirmation |
|---|---|---|---|
| Public language policy | English core docs/pages, Korean allowed in `docs/context/*` notes | Resolved (Working Rule) | Confirmed |
| Home featured projects (2-3) | Inference server, S3-FIFO, ROS2+YOLO | Applied | Pending Review |
| YBIGTA leadership end date | 2026.06 (from context note) | Provisional | Pending |
| Timeline milestone dates | Year-level milestones added (2021, 2024-2025, 2025-2, 2026) | Applied | Pending Review |
| Public page language style | Full English pages (current) | Applied | Pending Review |

## 5. Open Questions
- Which 2-3 projects should be featured on Home right now?
- Should all project pages be English only, or bilingual detail sections?
- What is the exact end date of the YBIGTA DE team leader period (confirm 2026.06)?
- Which project has stable metrics ready for public posting?

## 6. Provisional Draft Pack (Editable)
Use these as temporary copy until owner review.

### Home Draft (Provisional)
- Identity line: "Applied Statistics + Computer Science student focused on systems performance and architecture."
- Transition line: "My focus moved from data analysis to constrained system optimization."
- Focus tags: OS, distributed systems, real-time systems, efficient AI serving.

### About Draft (Provisional)
- Keep concise: education, current focus, key leadership experience.
- Include YBIGTA leadership summary and current systems-oriented direction.

### Timeline Draft (Provisional)
- 2021: Entered Yonsei, broad exploration stage.
- Post-military return: expanded through data/ML and implementation-heavy projects.
- 2024-2025: shifted from analytics outputs to throughput/parallelism concerns.
- Turning point: OS and real-time systems coursework.
- 2025-2 onward: CS double major and systems research orientation.
- 2026: target MS path, PhD decision after hands-on lab research exposure.

### Project Priority Draft (Provisional)
- Priority 1: Home inference server setup (operational systems perspective).
- Priority 2: S3-FIFO implementation (systems algorithm perspective).
- Priority 3: ROS2 + YOLO hazard detection (real-time/edge perspective).
- Backup: Uber data pipeline (scalability and reliability perspective).
## 7. Publish Safety Checklist
- No student ID, private contact details, or meeting logistics.
- No lab-internal or non-public implementation details.
- No private email content copied verbatim into public pages.
- Every public claim can be traced to a source fact ID above.
