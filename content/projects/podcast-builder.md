---
title: "Podcast Builder"
description: "A reusable workflow for short, NPR-style multi-speaker podcast episodes as an alternative entry point into faculty-facing pre-reads and course materials."
date: 2026-09-18
draft: false
cluster: "teaching-tools"
weight: 60
workstream: "03-teaching-tools/podcast-builder"
status: planning
pillar: ["build", "teach"]
owner: ["TBD"]
---

Podcast Builder produces short (10–12 minute) NPR-style conversations among multiple speakers as an alternative entry point into material faculty and students would otherwise only get as a written pre-read. A general-purpose AI model handles source analysis, pedagogy framing, script architecture, and production editing; ElevenLabs (Studio, Text-to-Dialogue API, hosted MCP) handles voice casting, multi-speaker synthesis, and export. The faculty-facing workflow stays simple — advanced model in, finished audio out — while the automation layer this project builds does the coordination between the two.

The pattern originates in the cloned-voice podcast pipeline built for the Legal Education at Model Velocity microsite, and generalizes it into something repeatable rather than bespoke per course.

## What we're doing

- Build the API/automation layer that drives ElevenLabs Studio and Text-to-Dialogue from a locked script and a small voice-casting spec, without faculty needing to touch MCP or API calls directly.
- Standardize the production inputs an episode needs: script, voice bible/episode plan, production and performance notes, casting criteria.
- Pilot the workflow on a real episode rather than a demo: an alternative audio entry point into the pre-read for the 2026 faculty retreat's AI session.
- Generalize what works into a template other courses and programs can reuse.

## Why this matters

A well-produced pre-read still asks a lot of a reader's time before they've decided the topic is worth it. A short, well-produced conversation lowers that barrier and can carry nuance — disagreement, qualification, someone changing their mind mid-argument — that a summary flattens out. Making that format cheap enough to produce per-course, rather than reserved for flagship microsites, is what turns it from a one-off into infrastructure.

## Status

Planning. Workflow being built alongside its first real pilot: an episode accompanying the September 2026 faculty retreat's AI pre-read.
