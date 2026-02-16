---
title: "GPU Batching Prototype"
date: 2026-02-16
draft: false
tags: ["systems", "gpu", "serving"]
---

## Problem
Single-request inference caused low GPU utilization and unstable throughput.

## Context and Constraints
- Goal: improve throughput while keeping latency stable
- Constraint: small local test environment and limited GPU memory
- Target: predictable behavior under bursty traffic

## Approach
- Implemented micro-batching with queue timeout
- Compared fixed-size batching and adaptive batching
- Measured latency and throughput under multiple request rates

## Trade-offs
- Larger batch size improved throughput but increased tail latency
- Short timeout reduced waiting but underutilized GPU in low traffic

## Result Snapshot
- Throughput: improved in medium/high load scenarios
- Latency: stable at small batch sizes, degraded at aggressive settings
- Next step: add scheduler policy based on queue depth

## What I Learned
Batching is not only a model issue. Queue policy and system-level scheduling dominate real performance behavior.
