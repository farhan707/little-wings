# Little Wings — Production Output Schema

This schema defines the minimum structured data returned by the automation engine.

```yaml
production:
  series: "Little Wings"
  bible_version: "1.1"
  status: "DRAFT"
  target_runtime_seconds: 30
  production_parts: 3

story:
  title: ""
  summary: ""
  lesson: ""
  language: "Urdu"

canon:
  characters: []
  environments: []
  references: []

scene_reference_states:
  - state_id: "REF_STATE_001"
    purpose: ""
    reference_ids: []
    active_from_part: "PART_001"
    active_until_part: "PART_002"
    change_reason: ""

parts:
  - part_id: "PART_001"
    scene_id: "SCENE_001"
    purpose: ""
    duration_seconds: 10
    environment_id: ""
    character_ids: []
    active_reference_state: "REF_STATE_001"
    speaker: null
    dialogue: ""
    emotion: ""
    action: ""
    camera:
      shot: ""
      angle: ""
      movement: ""
      framing: ""
    lighting: ""
    lip_sync: "STRICT"
    continuity_notes: ""
    video_prompt: ""

qa:
  character_identity: "PASS"
  environment_continuity: "PASS"
  age_relative_size: "PASS"
  reference_strategy: "PASS"
  dialogue_assignment: "PASS"
  lip_sync: "PASS"
  motion: "PASS"
  continuity: "PASS"
  canon_safety: "PASS"
  editability: "PASS"
  overall: "PASS"

new_assets_required:
  characters: []
  environments: []
  references: []

approval_required:
  canon_changes: []
  new_characters: []
  new_environments: []
  new_reference_states: []
```

## Required Rules

- IDs must use canonical registry IDs whenever they already exist.
- For approximately 30-second videos, default to approximately 3 production parts, normally 8–10 seconds each.
- Do not create micro-clips merely to split dialogue or reactions when one coherent part can contain them.
- `speaker` must be null for parts with no dialogue.
- A dialogue part should have exactly one primary speaker whenever practical.
- `lip_sync` must be `STRICT` for dialogue parts.
- Every permanent reference must be verified as APPROVED before production.
- Every scene should identify its active reference state.
- Reuse an active reference state until a meaningful visual change requires a new one.
- `approval_required` must explicitly list any proposed canon change.
