# Little Wings — Reference Image System

## Objective
Maintain visual consistency with a **small, reusable set of high-value master and scene references**.

## Core Principle

Do **not** generate a separate reference image for every clip.

The AI should first ask:

> **Can the current approved/reference image safely represent this entire scene or production part?**

If yes, reuse it.

Generate a new reference only when the visual state genuinely changes.

## Reference Hierarchy

1. **Master Character References** — permanent identity canon.
2. **Master Environment References** — permanent environment canon.
3. **Scene Reference States** — temporary composition references for a particular story/episode.
4. **Generated Video Clips** — outputs, not canon by themselves.

## Scene Reference Reuse Rule

For a scene, keep using the same scene reference image while all of the following remain true:
- same characters
- same environment
- same important props
- same clothing
- same general composition
- no new character
- no major new object
- no major spatial change

A dialogue change or small action change alone does **not** require a new reference image.

## Reference Change Triggers

Create a new scene reference state when:
- a new character enters
- a major new object/prop is introduced
- the location changes
- the character grouping changes substantially
- a meaningful costume/appearance change occurs
- the camera/composition changes so much that the previous reference is no longer sufficient

## Master Reference Principle

Do not generate a separate master reference for every scene.

Prefer reusable master references such as:
- individual character masters
- children + dining environment
- children + mother + dining environment
- full family + dining environment
- clean individual environment masters

## Reference Metadata

Every approved reference should eventually have:
- reference_id
- type
- characters
- environment
- purpose
- canon_status
- version
- source_file
- approval_date

## Selection Rule

Automation should select the **smallest sufficient set** of approved references that fully covers the current visual state.

If the video-generation tool has a practical reference-image limit, optimize for that limit instead of attaching every available reference.

## Reference Role Separation

When multiple references are used, each reference should have one explicit role, for example:
- Character identity
- Existing character continuity
- Environment
- New prop/object
- New character

Do not attach redundant references merely because they exist.

## Failure Rule

If no suitable reference exists, flag the scene for reference creation instead of silently inventing a new canon design.

A newly generated scene reference is temporary until explicitly approved as canon.
