# Content Outline

Generated from `docs/content_outline_raw.md` on 2026-02-17.

## 1. Current Goal
- Convert docs/context notes into publish-ready copy for Home/About and a prioritized project list.
- Replace placeholder examples with real content in Projects and Study sections.
- Keep About concise with only short growth context.

## 2. Source Context Inbox
- docs/context/abt myself (portfolio).md
- docs/context/rtcl-meeting-prep.md
- docs/context/prof-contact-email.md

## 2.1 Verified Fact Baseline
- Use verified items from `docs/context_intake.md` (e.g., `F-001` to `F-012`).
- Do not publish unverified statements without owner confirmation.

## 2.2 Provisional Execution Order
1. Finalize Home and About copy from `F-001`, `F-003`, `F-005`.
2. Build two full project pages first from `F-004`, `F-009` (Inference server and S3-FIFO).
3. Add one additional project (ROS2+YOLO or Uber pipeline) after metric availability check.
4. Backfill two recent study entries using `F-010`, `F-011`.

## 3. Mapping Plan (Source -> Target Page)

### Home (`content/_index.md`)
- One-line identity: Applied Statistics + Computer Science student focused on systems performance and architecture.
- Positioning sentence: from data analysis to systems optimization under constraints.
- Current focus candidates: operating systems, distributed systems, efficient AI serving.
- Use `Current Research` as the heading for the active-area summary.

### About (`content/about/_index.md`)
- Education: Yonsei University (2021-current), Applied Statistics major + Computer Science double major.
- Keep only concise profile, focus, and key experiences.
- Experience highlights: YBIGTA vice president and data engineering team leadership.
- Separate `Research Interests` (real-time systems, VLA/robotics, probabilistic timing) from `Systems Background` (OS, AI infrastructure, data engineering).

### Projects (`content/projects/`)
- Priority 1: Home inference server setup (DeepSeek operation, 25-1).
- Priority 2: Implementing S3-FIFO cache algorithm (25-1).
- Priority 3: ROS2 + YOLO hazard detection robot system (25-2).
- Backup: Uber data pipeline project (25-W).
- Keep project pages in a common structure: problem, approach, trade-offs, results, lessons.
- Add at least one metric per featured project (latency, throughput, scale, reliability).

### Study (`content/study/`)
- Flexible entry format: meeting summary, experiment notes, paper notes, or implementation memos.
- Topic stream: real-time scheduling under constrained resources.
- Topic stream: deadline vs accuracy trade-off in AI inference tasks.
- Topic stream: OS-level real-time concerns for ROS and embedded/edge systems.

## 4. Gaps and Questions
- Home featured set currently applied: Inference server, S3-FIFO, ROS2+YOLO.
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
- [x] Study entries added

## 7. Parked Projects and Study Review (2026-07-30)

Status: Candidate review only. No featured-project selection, Study scope, or public content change is confirmed.

### Project Candidates to Reassess

- ROS2 + YOLO: verify the implementation artifacts and the recorded `10 Hz` to `30+ Hz` improvement before using it publicly.
- Uber Data Pipeline: verify the architecture, individual contribution, and recorded `10,000+ events/s` result.
- Third featured slot: compare Home Inference Server and NotebookLocal based on available code, architecture, measurements, and public artifacts.
- S3-FIFO: keep as a supporting project candidate.
- GPU Batching Prototype: keep on hold until a real implementation and measurements are located.
- PRTG-VLA: keep under Current Research or Study until a stable experiment result supports promotion to Projects.

### Study Milestone Candidates

- `From Probabilistic Timing Guarantees to VLA Temporal Validity`
- `Profiling pi0.5 Inference on LIBERO`
- `When Does VLA Latency Become a Safety Problem?`

Use public-safe milestone summaries rather than automatically publishing every meeting record or lab-internal artifact.

### Resume Point

1. Recheck the live repository and current research state.
2. Verify the evidence and public safety of the project candidates.
3. Select only two or three featured projects with the owner.
4. Confirm whether the three Study milestones still represent the desired public research narrative.
