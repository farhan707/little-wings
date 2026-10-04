# Little Wings — Production Output Schema

This schema defines the minimum structured data returned by the automation engine.

```yaml
production:
  series: "Little Wings"
  bible_version: "1.0"
  status: "DRAFT"

story:
  title: ""
  summary: ""
  lesson: ""
  language: "Urdu"

canon:
  characters: []
  environments: []
  references: []

scenes:
  - scene_id: "SCENE_001"
    purpose: ""
    environment_id: ""
    reference_ids: []
    clips:
      - clip_id: "CLIP_001"
        duration_seconds: 8
        characters: []
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
  dialogue_assignment: "PASS"
  lip_sync: "PASS"
  motion: "PASS"
  continuity: "PASS"
  canon_safety: "PASS"
  overall: "PASS"

new_assets_required:
  characters: []
  environments: []
  references: []

approval_required:
  canon_changes: []
  new_characters: []
  new_environments: []
```

## Required Rules

- IDs must use the canonical registry IDs whenever they already exist.
- `duration_seconds` should normally be between 5 and 10.
- `speaker` must be null for clips with no dialogue.
- A dialogue clip must have exactly one primary speaker whenever practical.
- `lip_sync` must be `STRICT` for dialogue clips.
- Every permanent reference must be verified as APPROVED before production.
- `approval_required` must explicitly list any proposed canon change.
