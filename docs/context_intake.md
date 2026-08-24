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
| F-002 | `docs/context/abt myself (portfolio).md` | Experience | YBIGTA vice president (2025.06-2025.12), DE team lead (2025.12-2026.06) | Medium | Yes | About | No | Confirm exact end date |
| F-003 | `docs/context/rtcl-meeting-prep.md` | Interest motivation | Interest shifted from data analysis to systems/real-time constraints | High | Yes | Home, About | No | Keep concise |
| F-004 | `docs/context/prof-contact-email.md` | Project list | Home inference server, S3-FIFO, ROS2+YOLO, data pipeline projects | Medium | Yes | Projects | No | Add metrics before publish |
| F-005 | `docs/context/abt myself (portfolio).md` | Interest / Research Interests | Core interests include OS, distributed/parallel systems, real-time systems, AI serving, system architecture | High | Yes | Home, Research, About | No | Can be published as focus areas |
| F-006 | `docs/context/abt myself (portfolio).md` | Past narrative | Post-military return led to data/ML projects, then focus shifted to throughput, parallel execution, and systems-level efficiency | Medium | Yes | About | No | Keep concise and date-anchored |
| F-007 | `docs/context/rtcl-meeting-prep.md` | Career direction | Prefers research-oriented path; plans to pursue MS and decide on PhD after research experience | Medium | Yes | About | No | Publish as direction, not commitment |
| F-008 | `docs/context/abt myself (portfolio).md` | Lectures (CS) | Completed core systems-related courses: OS, System Programming, Real-Time System, Computer Network, Distributed Training and Inference | High | Yes | About | No | Avoid listing too many courses on public pages |
| F-009 | `docs/context/abt myself (portfolio).md` | Projects | Project history spans data analysis, agent applications, inference setup, ROS, and data pipeline work | High | Yes | Projects | No | Use 2-3 representative projects first |
| F-010 | `docs/context/rtcl-meeting-prep.md` | Real-time interest details | Strong interest in constrained scheduling and deadline/accuracy trade-offs in AI inference tasks | High | Yes | Research | No | Use as background, not as a finished claim |
| F-011 | `docs/context/rtcl-meeting-prep.md` | ROS/RT interest | Interest in OS-level real-time guarantees for ROS and embedded/edge scenarios | Medium | Yes | Research, Projects | No | Keep claims directional unless validated by project artifacts |
| F-012 | `docs/context/rtcl-meeting-prep.md` | Data engineering reflection | Data engineering is useful but currently viewed as less aligned with intended research depth | Medium | Yes | About | No | Phrase as personal preference, not absolute claim |
| F-013 | Owner-directed Meeting 21 review | Current research checkpoint | The working direction moved from standalone temporal validity toward runtime acceptability and monitoring under timing and resource constraints | High | Yes | Home, Research, About | Yes | Publish only the broad question and evidence boundary; omit weekly materials and internal experiment detail |
| F-014 | Owner-directed homepage copy review | Confirmed public research identity | The Home hero frames the work as predictable and reliable execution under timing and resource constraints, with machine-learning systems and robotics as the current focus; the public affiliation label is RTCL@Yonsei | High | Yes | Home | Yes | Plain-language wording approved 2026-08-24 |
| F-015 | Owner-directed project-list review | Confirmed public project titles and placement | Add Adaptive Multi-Interest Recommendation Pipeline [26-1], ROBO 404++ Autonomous Driving Pipeline [26-1], New-Town Traffic Safety Infrastructure Analysis [25-W], and Home Inference Server Setup [25-1] to their respective Additional Work groups | High | Yes | Projects | Yes | New-Town term corrected by the owner on 2026-08-24; keep the New-Town and Home Inference Server work as one-line entries rather than Selected Work |
| F-016 | Owner-directed About copy review | Confirmed public research-interest framing | About retains three research-interest lines: Real-Time Systems; VLA & Robotic Systems; Probabilistic Timing Analysis | High | Yes | About | Yes | Wording approved verbatim 2026-08-24 |
| F-034 | Owner-directed Research page review | Confirmed public research structure | Research leads with the current VLA runtime question, then presents Real-Time Systems, Probabilistic Timing Analysis, and VLA & Robotic Systems as stable areas; ML for RT and RT for ML remain a connecting perspective | High | Yes | Research | Yes | Keep the trajectory at overview level and omit discarded hypotheses and internal diagnostic details |
| F-017 | Local `degent` repository and project plan | README, model and replay architecture | AMIRec combines MovieLens recommendation, adaptive interest clustering, and a batch-to-stream replay path | High | Yes | Projects | Yes | Avoid presenting the replay path as production streaming infrastructure |
| F-018 | Local `27th-DE-WinterProject` repository | README pipeline and deployment sections | The Uber-style pipeline connects Kafka, Flink, and ClickHouse and supports distributed deployment and observability | High | Yes | Projects | Yes | Project-level description; omit unverified throughput metrics |
| F-019 | Home-server vault workspace | WireGuard and host-protection setting notes | Home-server access work covered VPN-based remote access and host/network hardening | High | Yes | Projects | Yes | Do not publish addresses, topology, credentials, or operational details |
| F-020 | Public-safe Home Inference Server project draft | Problem, approach, and result snapshot | The home inference environment focused on local LLM serving and runtime behavior under constrained hardware | High | Yes | Projects | Yes | Keep vendor/model detail out of the list descriptor |
| F-021 | Local `28th-conference-robo404_plus` and public `jiy0-0nv/robo404pp_hardware` repositories | Software pipeline and hardware README at commit `279a632` | ROBO 404++ integrates Jetson Nano ROS2/TensorRT perception and decision with a physical 4WD platform controlled through Pico 2, micro-ROS, and a TB6612FNG motor driver | High | Yes | Projects | Yes | Distinguish the physical deployment from the earlier simulation; software scope ends at `/cmd_vel`, while the hardware repository owns low-level control |
| F-022 | Local `27th-conference-robo404` repository | README overview and architecture | ROBO 404 is a Gazebo and TurtleBot3 simulation combining Nav2, YOLO hazard detection, camera tracking, and vision-based safety assessment | High | Yes | Projects | Yes | Label it as simulated and do not publish unverified performance claims |
| F-023 | Local and public `26th-summer-NotebookLocal` repository | README architecture overview | NotebookLocal connects an Obsidian plugin to a RAG backend for document-grounded knowledge assistance | High | Yes | Projects | Yes | Use the stable system boundary rather than broad intelligence claims |
| F-024 | Public `26th-conference-Legent` repository | README pipeline and implementation tree | The legal agent combines uploaded traffic-accident video analysis with legal-document retrieval | High | Yes | Projects | Yes | Keep the descriptor at the project-system level |
| F-025 | Public `bindingflare/agi_hackathon-team_ODE` repository | FORMula README and implementation tree | The hackathon system supports trade/customs Q&A, PDF validation, regulatory checks, FAISS document retrieval, and FastAPI/Streamlit services using Upstage and GPT-4o Search APIs | High | Yes | Projects | Yes | Publish architecture and domain only; never publish repository environment values |
| F-026 | Public `YBIGTA/26th-project-JeMeChu` repository | README introduction and pipeline | The project recommends restaurants from natural-language conditions using structured filtering and review embeddings | High | Yes | Projects | Yes | Rename the vague meal-recommendation title to match the implemented restaurant service |
| F-027 | Local COMPAS repository and final report | Analysis pipeline and final placement results | The New-Town project transferred geospatial traffic risk and selected safety-facility sites for Hanam Gyosan | High | Yes | Projects | Yes | Team-project description; do not imply sole ownership |
| F-028 | Archived baseball analysis notes | Question framing, audience data, and survey sources | The baseball project analyzed audience and survey evidence around baseball and social cohesion | High | Yes | Projects | Yes | Use a concise descriptive title rather than the original question sentence |
| F-029 | Local `Byte2.0-main` repository | Crawling, embedding, forecasting, and SHAP modules | The project combines Samsung Electronics news from Naver and Yonhap with financial and macro features, OpenAI embeddings, autoencoder/truncation reduction, Transformer forecasting, and SHAP attribution | High | Yes | Projects | Yes | Describe measured model attribution rather than claiming causal news effects |
| F-030 | Public `VisualizingLacityCrimeData` repository | README, R scripts, and Shiny artifacts | The crime project used geospatial LA data, prediction models, and an R Shiny application | High | Yes | Projects | Yes | Keep the descriptor method-oriented |
| F-031 | Public `WindfarmEnergyGeneration` repository | Forecasting notebook model definition | The wind project combines LDAPS/SCADA inputs, a physics-based power estimate, Box–Cox transformation, and Laplace/Beta distribution calibration | High | Yes | Projects | Yes | The source dataset is private; publish no raw data or operational paths |
| F-032 | Public `PublicFigureCrisisManagement` repository | Crawling, text-analysis, and visualization artifacts | The opinion project mined Naver News and YouTube text for public-figure crisis-response patterns | High | Yes | Projects | Yes | Avoid naming individuals or reproducing collected comments |
| F-033 | Public `BikeWheelSetRecommendation` repository | R pipeline and sentiment outputs | The wheelset project used community text and sentiment analysis to compare product attributes | High | Yes | Projects | Yes | Keep the descriptor general and public-safe |
| F-035 | Owner-directed Selected Work review | Confirmed representative robotics project | Feature ROBO 404++ as a vision-guided 4WD robotic vehicle and keep both the physical ++ system and earlier Gazebo/TurtleBot3 mobile-robot simulation in Additional Work | High | Yes | Projects | Yes | Use the hardware integration boundary verified in F-021; reserve vehicle language for the physical platform |
| F-036 | Owner-directed Selected Work review | Confirmed representative data-infrastructure project | Feature the Uber-style distributed data pipeline alongside ROBO 404++ in Selected Work while retaining its chronological Additional Work entry | High | Yes | Projects | Yes | Emphasize the verified Kafka/Flink/ClickHouse/ONNX pipeline, distributed deployment, and observability boundary from F-018 |
| F-037 | Owner-directed long-term research vision | Confirmed public aspiration | Long term, aim to make real-time systems a practical foundation for reliable robotic intelligence | High | Yes | Research | Yes | Publish as a forward-looking closing statement, not as a completed achievement |

Confidence rule:
- `High`: explicitly stated in source, no ambiguity
- `Medium`: stated but needs date/scope clarification
- `Low`: inferred from context, needs confirmation

## 4. Decision Locks (Must Confirm Before Publish)
| Decision | Current Value | Status | Owner Confirmation |
|---|---|---|---|
| Public language policy | English core docs/pages, Korean allowed in `docs/context/*` notes | Resolved (Working Rule) | Confirmed |
| Home featured projects (2) | ROBO 404++ and the Uber-style distributed data pipeline | Resolved | Confirmed 2026-08-24 |
| YBIGTA leadership end date | 2026.06 (from context note) | Provisional | Pending |
| Public page language style | Full English pages (current) | Applied | Pending Review |
| About interest hierarchy | Research Interests: real-time systems, VLA/robotics, probabilistic timing; Systems Background: OS, AI infrastructure, data engineering | Resolved | Confirmed 2026-07-30 |

## 5. Open Questions
- Which selected projects have enough public evidence for dedicated detail pages?
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

### Earlier Project Priority Draft (Superseded)

The current Selected Work set is ROBO 404++ and the Uber-style distributed data pipeline. The earlier provisional priorities are retained below only as historical planning context.
- Priority 1: Home inference server setup (operational systems perspective).
- Priority 2: S3-FIFO implementation (systems algorithm perspective).
- Priority 3: ROS2 + YOLO hazard detection (real-time/edge perspective).
- Backup: Uber data pipeline (scalability and reliability perspective).
## 7. Publish Safety Checklist
- No student ID, private contact details, or meeting logistics.
- No lab-internal or non-public implementation details.
- No private email content copied verbatim into public pages.
- Every public claim can be traced to a source fact ID above.
