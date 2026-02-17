```table-of-contents
```

# GitHub.io Site Structure & Content Guide

This document defines the **content structure and philosophy** of my GitHub Pages website.
The goal is to focus on a **portfolio-focused personal site** and a **Study Log** to track my progress.

---

## Core Concept

- **No traditional blog**. The Study Log serves as the continuous record.

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
├── study/             # What I am currently studying (Study Log)
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

### 3. Study Log (`content/study/`)

**Purpose**

> Keep a lightweight weekly record of what I recently read, what I am interested in, and what I presented.

**Operating Style**

- **Frequency**: Usually weekly (after advisor/lab presentation).
- **Source**: The presentation PPT I already make.
- **Format**:
    - Recent papers read (or revisited)
    - Current technical interests/focus
    - Short comment in diary style (3-6 lines)
    - PPT attachment (PDF or key slide images)
- **Goal**: Keep evidence of consistent progress with minimal overhead.

**Template**
```markdown
---
title: "Study Log: 2026-XX-XX"
date: 2026-XX-XX
tags: ["study-log", "weekly"]
---
## Recent Papers
- Paper A
- Paper B

## Current Interests
- Topic A
- Topic B

## Notes (Diary)
- What I found interesting this week
- What was confusing or difficult
- What I want to test next week

## Weekly PPT
[Download PPT/PDF](/files/2026-xx-xx-weekly.pdf)
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
|Study|What am I studying right now?|
|About|What is my official profile?|
|Contact|How can someone reach me?|





## One-Sentence Summary

> This site is not a blog.  
> It is a **living record of growth as a systems engineer and researcher**.
