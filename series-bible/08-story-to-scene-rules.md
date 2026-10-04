# Little Wings — Story-to-Scene Rules

## Input
A story or story concept.

## Transformation Pipeline
Story
→ Story Analysis
→ Character Identification
→ Location Identification
→ Reference Planning
→ 30-Second / Production-Part Planning
→ Scene Breakdown
→ Dialogue Assignment
→ Action Assignment
→ Camera Assignment
→ Prompt Generation
→ QA

## Production-Part Strategy

For short videos with a target runtime of approximately 30 seconds, do **not** automatically break the story into many tiny clips.

Default production structure:

- Divide the story into approximately **3 logical production parts**.
- Target approximately **8–10 seconds per part**, respecting the generation tool's maximum duration.
- Prefer one coherent visual/action beat per part.
- The three parts should also be easy to assemble during editing.
- A 30-second story does not require 8–12 separate micro-clips unless the story genuinely needs them.

Example:

**Part 1:** Setup / problem  
**Part 2:** Explanation / discovery  
**Part 3:** Resolution / payoff

The exact number of parts may change when story structure requires it, but unnecessary fragmentation should be avoided.

## Scene Reference Continuity

A scene should use **one primary reference image** for as long as the visual composition remains unchanged.

Reuse the same scene reference image across consecutive generated parts/clips when:
- the same characters remain present
- the same environment remains present
- no important new object is introduced
- no important costume change occurs
- no new character enters
- the composition remains production-safe

Do **not** create a new reference image merely because the dialogue or action changes.

### Reference Change Trigger

Create/select a new scene reference only when there is a meaningful visual change, such as:
- a new character enters
- a major new object/prop becomes important
- the location changes
- the character grouping changes substantially
- a significant costume/appearance change is required
- the existing reference can no longer represent the intended composition clearly

When a new reference is required, treat it as a new **scene reference state**, not automatically as new canon.

## Clip Length

Normal production parts/clips should target **8–10 seconds** when supported by the generation tool.

### Short-Form Exception
For reels, shorts, teasers, reactions, very short dialogue, or moments that genuinely require tighter pacing, clips may be **2–7 seconds**.

A short clip is not automatically a canon violation.

However, short clips must not become the default merely to split a scene into many small pieces. The automation should prefer the fewest practical clips that preserve:
- dialogue clarity
- action readability
- lip-sync
- continuity
- editing simplicity
- final runtime

## Scene Design

Each production part should have:
- one primary action
- one clear emotional beat
- explicit character IDs
- explicit location
- explicit speaker
- simple camera direction
- the active scene reference ID

Avoid packing many unrelated actions into one part.

## Multi-Speaker Rule
Prefer one speaker per generated part. If two speakers are required, keep dialogue short and explicit.

## Scene Continuity
Adjacent parts must preserve:
- character appearance
- age and relative size
- clothing
- location
- props
- lighting
- time of day
- emotional state when relevant
- camera relationship
- active scene reference

## Output Schema
Every production part should contain:
- part_id
- scene_id
- duration_seconds
- location_id
- character_ids
- reference_ids
- scene_reference_state
- action
- dialogue
- speaker_id
- camera
- visual_prompt
- lip_sync_instruction
- continuity_notes
- qa_status
