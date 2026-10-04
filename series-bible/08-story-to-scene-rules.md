# Little Wings — Story-to-Scene Rules

## Input
A story or story concept.

## Transformation Pipeline
Story
→ Story Analysis
→ Character Identification
→ Location Identification
→ Reference Selection
→ Scene Breakdown
→ Dialogue Assignment
→ Action Assignment
→ Camera Assignment
→ Prompt Generation
→ QA

## Clip Length
Target short clips suitable for current generation tools, normally **5–10 seconds**.

## Scene Design
Each clip should have:
- one primary action
- one clear emotional beat
- explicit character IDs
- explicit location
- explicit speaker
- simple camera direction

Avoid packing many unrelated actions into one clip.

## Multi-Speaker Rule
Prefer one speaker per shot. If two speakers are required, keep dialogue short and explicit.

## Scene Continuity
Adjacent clips must preserve:
- character appearance
- clothing
- location
- props
- lighting
- time of day
- emotional state when relevant

## Output Schema
Every scene plan should contain:
- scene_id
- clip_duration
- location_id
- character_ids
- reference_ids
- action
- dialogue
- speaker_id
- camera
- visual_prompt
- lip_sync_instruction
- continuity_notes
- qa_status
