# Little Wings — Video Generation Rules

## Primary Goal
Generate coherent, edit-friendly animation while preserving Little Wings canon.

## Production Strategy

For a video of approximately 30 seconds:
- Prefer approximately **3 coherent production parts**.
- Target **8–10 seconds per part** when the generation tool supports it.
- Avoid unnecessary micro-clips.
- Each part should be straightforward to place on the editing timeline.

The production plan may use fewer or more parts when the story genuinely requires it.

## Reference Strategy

Use one active scene reference image for as long as possible.

Keep the same reference across consecutive parts when:
- characters are unchanged
- environment is unchanged
- important props are unchanged
- composition remains suitable

Change the reference only when a meaningful visual state change occurs.

## Prompt Language
Visual prompts should normally be written in English for stronger model reliability.

Dialogue remains in the required spoken language.

## Clip Design
Each part should normally be 8–10 seconds and focus on one coherent action/beat.

Do not split a simple scene into multiple tiny clips only to satisfy an old 5–10 second rule.

## Motion
Prefer:
- natural walking
- natural hand movement
- subtle head movement
- believable reactions
- gentle camera movement

Avoid excessive motion and simultaneous complex actions.

## Strict Lip-Sync
Use this instruction whenever dialogue is present:

**IMPORTANT STRICT LIP-SYNC: Only the character currently speaking may move their lips and mouth. Silent characters must keep their mouths closed. Never animate the wrong character speaking. Match each dialogue line to the exact character shown speaking.**

## Character Continuity
The generation prompt must preserve approved:
- face
- hair
- clothes
- accessories
- body proportions
- age appearance
- relative size between characters

## Environment Continuity
Use the approved environment reference and preserve:
- major layout
- furniture
- props
- lighting
- camera relationship
- overall visual identity

## Reference Limit Awareness

If the generation tool becomes less consistent when additional references are added, prefer a smaller reference set with clear roles.

Never sacrifice established character/environment consistency merely to attach every available reference.

## Generation Failure
If identity, lip-sync, anatomy, environment, age/relative-size, or continuity fails, mark the part for regeneration rather than accepting a visibly inconsistent result.


## Video-to-Video Continuity

When supported by the generation tool, use the previous generated video as the primary reference for the next clip when the scene has not materially changed.

Recommended chain:
**Master References → Clip 1 → Clip 2 → Clip 3**

Clip 1 establishes the scene using approved references. Clip 2 uses Clip 1 as its continuity reference. Clip 3 uses Clip 2 as its continuity reference. Repeat until a meaningful visual change requires re-anchoring.

Re-anchor with approved references when a new character enters, a major new object becomes important, the location changes, costume/appearance changes, character grouping changes substantially, or visual drift is detected.

The previous video reference does not override canon. Approved master references remain the source of truth.
