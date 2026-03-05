```table-of-contents
```

# GitHub.io Site Structure & Content Guide

This document defines the **content structure and philosophy** of my GitHub Pages website.
The goal is to focus on a **portfolio-focused personal site** and a **Study archive** to track my progress.

---

## Core Concept

- **No traditional blog**. The Study section serves as the continuous record.

> This site represents a *growing systems engineer / researcher*, not a finished product.

---

## Directory Structure (Hugo `content/`)

```text
content/
├── _index.md          # Home
│
├── projects/          # What I have built
│   ├── _index.md
│   ├── project-a.md
│   ├── project-b.md
│   └── ...
│
├── study/             # Ongoing study archive (notes, experiments, meeting materials)
│   ├── _index.md
│   ├── paper-gedf.md
│   ├── gpu-batching.md
│   └── ...
│
├── about/             # Curated public profile
│   └── _index.md
│
├── contact/           # Public contact links
│   └── _index.md
│

````

---

## Page-by-Page Content Definition

### 1. Home (`content/_index.md`)

**Purpose**

> Answer: “Who is this person?” in under 30 seconds.

**Contains**

- Name & identity & interest
    
- Current focus areas (3–5 items)
    
- Selected projects (links only)
    
- Entry points to other pages
    

**Does NOT contain**

- Detailed CV
    
- Full project lists
    
- Personal reflections
    

---

### 2. Projects (`content/projects/`)

**Purpose**

> Show what I have actually built and experimented with.

**Contains**

- Completed or near-complete projects
    
- Architecture, trade-offs, and outcomes
    
- GitHub / demo links
    

**Organization**

- Grouped by domain, not by year:
    
    - AI Systems & Serving
        
    - Data Engineering & Streaming
        
    - OS / Systems
        

**Each project page should answer**

- What problem did I solve?
    
- How did I approach it?
    
- What did I learn?
    

---

### 3. Study (`content/study/`)

**Purpose**

> Keep an ongoing archive of what I read, build, test, and present.

**Operating Style**

- **Frequency**: Flexible (regular updates plus event-driven notes).
- **Source**: Meeting materials, experiments, reading notes, and implementation work.
- **Format**:
    - Context or goal
    - What was read/built/tested
    - Key observations and trade-offs
    - Next actions
    - Optional attachment (PPT/PDF/link)
- **Goal**: Keep evidence of consistent progress and experimentation with minimal overhead.

**Template**
```markdown
---
title: "Study Note: 2026-XX-XX Topic"
date: 2026-XX-XX
tags: ["study-note"]
---
## Context
- Why this note exists

## What I Read/Built/Tested
- Item A
- Item B

## Key Observations
- What worked
- What did not work
- What to improve

## Next Actions
- Next step 1
- Next step 2

## Optional Attachment
[PPT/PDF/Link](/files/2026-xx-xx-note.pdf)
```
---

### 4. About (`content/about/`)

**Purpose**

> A clean, curated public profile.

**Contains**

- Name
    
- University & major
    
- Research interests (refined)
    
- Current focus
    

**Does NOT contain**

- Full project lists
    
- All courses taken
    
- Detailed activity history
    

---

### 5. Contact (`content/contact/`)

**Purpose**

> Provide one clear place for professional contact links.

**Contains**

- Primary email
    
- GitHub profile link
    
- LinkedIn profile link
    

---



---

## Structural Philosophy Summary

|Section|Core Question Answered|
|---|---|
|Home|Who am I?|
|Projects|What have I built?|
|Study|What am I learning, testing, and documenting now?|
|About|What is my official profile?|
|Contact|How can someone reach me?|





## One-Sentence Summary

> This site is not a blog.  
> It is a **living record of growth as a systems engineer and researcher**.
