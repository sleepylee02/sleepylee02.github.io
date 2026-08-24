```table-of-contents
```

# GitHub.io Site Structure & Content Guide

This document defines the **content structure and philosophy** of my GitHub Pages website.
The goal is to present a **researcher-focused personal site** with a concise public research narrative and selected project evidence.

---

## Core Concept

- **No traditional blog or weekly public log**. Research is curated around the current question, trajectory, and stable public evidence.
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

- Grouped by domain, not by year:
    
    - AI Systems & Serving
        
    - Data Engineering & Streaming
        
    - OS / Systems
        

**Each project page should answer**

- What problem did I solve?
    
- How did I approach it?
    
- What did I learn?
    

---

### 3. Research (`content/research/`)

**Purpose**

> Explain the current research question, why it matters, and how the direction is evolving.

**Contains**

- Three stable research areas that connect foundations, methods, and the current application domain
- One current research question
- A small set of active investigation axes
- A concise account of how the framing changed
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
|Research|What question am I working on now, and how is it evolving?|
|About|What is my official profile?|
|Contact|How can someone reach me?|





## One-Sentence Summary

> This site is not a blog.  
> It is a **curated researcher profile grounded in current questions and selected work**.
