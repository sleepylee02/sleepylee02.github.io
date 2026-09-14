```table-of-contents
```

# GitHub.io Site Structure & Content Guide

This document defines the **content structure and philosophy** of my GitHub Pages website.
The goal is to present a **researcher-focused personal site** with a concise public research narrative and selected project evidence.

---

## Core Concept

- **No traditional blog or weekly public log**. Research is curated around research areas, systems background, trajectory, and stable public evidence.
- **Sharing previews stay concise**. Home uses Jaeyoung Lee as the title and Real-Time Systems · Robotics as its search and Open Graph description. The common preview image remains the original blue pattern in `static/og-image.png`.
- **Freshness is explicit**. Curated pages show their last meaningful content review; build or styling changes do not refresh that date.
- **Editorial structure stays consistent**. Research, Projects, and About use ordinary headings, lists, and horizontal dividers. Repeated research and selected-work items may use one shared typographic entry pattern, without cards or boxes.
- **Visual hierarchy is deliberate**. Public pages share one page-start rhythm, clear title levels, and subdued dividers instead of inheriting stacked theme margins.

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
├── research/          # Curated current research direction
│   └── _index.md
│
├── about/             # Curated public profile
│   └── _index.md
│
├── contact/           # Public contact links
│   └── _index.md
│

```

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

Additional Work is grouped by domain in this display order:

1. Robotics
2. Systems & Infrastructure
3. AI Applications
4. Data Analysis & Forecasting

The AI Applications group includes the personal work, knowledge, and dashboard
systems alongside the existing knowledge-assistance, agent, and recommendation projects.

**Each project page should answer**

- What problem did I solve?
    
- How did I approach it?
    
- What did I learn?
    

---

### 3. Research (`content/research/`)

**Purpose**

> Explain research interests, the systems background behind them, and how the direction is evolving.

**Contains**

- Three stable research areas in the existing order, with VLA & Robotic Systems labeled Current Focus
- Systems Background: operating systems and system programming, AI infrastructure, and data engineering
- A concise Research Trajectory
- Explicit boundaries between ongoing hypotheses and established results

**Does NOT contain**

- Automatic weekly meeting uploads
- Raw experiment logs or lab-internal notes
- Unstable claims presented as finished results

---

### 4. About (`content/about/`)

**Purpose**

> A clean, curated public profile.

**Contains**

- Profile introduction, including university, majors, and current focus
- Experience & Leadership
- Education
- How I Think

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
|Research|What do I study, and how is my research evolving?|
|About|What is my official profile?|
|Contact|How can someone reach me?|





## One-Sentence Summary

> This site is not a blog.  
> It is a **curated researcher profile grounded in current questions and selected work**.
