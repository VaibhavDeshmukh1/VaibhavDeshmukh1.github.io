---
title: "Project 1 Progress: Week 3"
date: 2026-07-05
permalink: /posts/2026/07/project-1-week-3/
reading_time: "2 min read"
tags: AI bootcamp research arXiv
---

Week three moved from bootcamp training to actual research infrastructure work.

I completed Notebook 1, which teaches how to build a reliable daily paper fetcher that avoids duplicates and doesn't lose data. The notebook addresses real engineering problems like paper revisions, API rate limits, and system failures. I worked through exercises on ID parsing, database operations, checkpoint logic, and error detection.

Professor Chen approved running the live fetcher. I set `RUN_LIVE = True` and the system connected to real arXiv, pulling 18 actual papers from the past 24 hours. Real data flowing through the system confirmed the fetcher works end-to-end.

Friday's team meeting introduced the larger project vision. The goal is understanding how to give AI agents precise instructions so they execute reliably. Vague prompts produce inconsistent results. Specific prompts with clear inputs, outputs, and constraints work better.

My team will spend the next week establishing a shared repository, validating the fetcher across multiple categories, proving the duplicate-handling logic, building a prompt library, and designing an initial graph schema. The focus is on proving the pipeline works end-to-end rather than building something complete.
