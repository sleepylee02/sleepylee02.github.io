---
title: "Research"
description: "Research on predictable and reliable execution under timing and resource constraints, with a current focus on VLA and robotic systems."
date: 2026-08-24
lastmod: 2026-08-24
draft: false
---

# Research

{{< freshness label="Last updated" format="January 2006" >}}

I study predictable and reliable execution under timing and resource constraints. My work connects real-time systems and probabilistic timing analysis to machine-learning and robotic systems.

---

### Current Research Question

How can VLA inference, action execution, monitoring, and recovery be coordinated so that unsafe behavior is detected and handled before intervention becomes ineffective?

- **Timely monitoring:** when and how often runtime checks must execute to detect problems in time.
- **Timing-aware intervention:** how quickly rejection, replanning, recovery, or fallback must complete to remain useful.
- **Shared-resource scheduling:** how inference, robot execution, and monitoring compete for limited compute resources.

---

### Research Areas

{{< content-entry title="Real-Time Systems" meta="Scheduling · Timing behavior · Resource constraints · Deadline constraints" >}}
Scheduling, timing behavior, and reliability under resource and deadline constraints.
{{< /content-entry >}}

{{< content-entry title="Probabilistic Timing Analysis" meta="Execution-time uncertainty · Deadline-failure risk · WCDFP / pWCET" >}}
Reasoning about execution-time uncertainty and deadline-failure risk.
{{< /content-entry >}}

{{< content-entry title="VLA & Robotic Systems" meta="VLA inference · Action execution · Runtime monitoring · Timely intervention" current="true" >}}
Exploring how inference and execution timing affect reliable robot behavior.
{{< /content-entry >}}

Across these areas, I am also interested in both directions of the relationship between machine learning and real-time systems: using ML to address real-time system problems, and designing predictable support for machine-learning workloads.

---

### Research Trajectory

Real-Time Systems → Probabilistic Timing Analysis → ML and Real-Time Systems → VLA Runtime Monitoring and Safety

My research has evolved from scheduling and probabilistic timing analysis toward VLA runtime safety.<br>
Long term, I aim to make real-time systems a practical foundation for reliable robotic intelligence.

---

{{< contextual-nav current="research" >}}
