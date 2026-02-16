---
title: "ROS2 + YOLO Hazard Detection System"
date: 2026-02-16
draft: false
tags: ["systems", "ros2", "robotics", "real-time"]
---

## Problem
I wanted to build a practical perception pipeline that can detect hazards in a robotics context and examine real-time constraints in system behavior.

## Context and Constraints
- Built as an implementation-focused project
- Need to coordinate perception and runtime behavior in a ROS2 workflow
- Real-time characteristics matter for practical reliability

## Approach
- Integrated YOLO-based detection into a ROS2 pipeline
- Designed the flow from input stream to detection output for practical testing
- Focused on system integration and runtime consistency

## Trade-offs
- Detection accuracy versus runtime response constraints
- Pipeline complexity versus debuggability
- Feature expansion versus stable end-to-end behavior

## Result Snapshot
- Built a functioning hazard-detection pipeline in ROS2
- Verified end-to-end integration from sensing input to detection output
- Identified key bottlenecks for future real-time tuning

## What I Learned
Real-time behavior is a systems-level property, not a single-model property.
Even strong model outputs can fail practical constraints if scheduling and pipeline timing are not controlled.

## Next Step
- Add explicit latency breakdown by pipeline stage
- Test trade-offs between detection settings and response behavior
