# Little Wings — AI Automation System

## Purpose

This directory defines how AI converts a Little Wings story into a production-ready plan while preserving established canon.

## Core Rule

The AI receives the story as the creative input, but the Series Bible and approved references remain the source of truth for everything already established.

## Pipeline

Story
→ Story Analysis
→ Character Identification
→ Environment Identification
→ Canon Reference Selection
→ Scene Breakdown
→ Clip Timing
→ Dialogue Assignment
→ Action Assignment
→ Camera Assignment
→ Character Lock
→ Environment Lock
→ Lip-Sync Lock
→ Video Prompt Generation
→ QA

## Automation Files

- `MASTER_AUTOMATION_PROMPT.md` — governing prompt for the story-to-production workflow.
- `PRODUCTION_OUTPUT_SCHEMA.md` — required machine-readable output structure.
- `QA_AUTOMATION_RULES.md` — automated validation rules before production.

## Canon Safety

Automation must never invent a replacement character, redesign an approved environment, or silently promote generated assets to canon.

Only references with status `APPROVED` in `references/reference-registry.md` may be treated as permanent canon.
