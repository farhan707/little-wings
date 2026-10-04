# Little Wings — Automation QA Rules

## PASS/FAIL VALIDATION

### Character QA
PASS only if every character has a valid canonical ID or is explicitly marked NEW_CHARACTER_REQUIRED.

FAIL if:
- an approved character is redesigned
- clothing changes without approval
- face/hair/proportions change
- an unknown character is silently mapped to an existing character

### Reference QA
PASS only if every permanent reference is marked APPROVED in `references/reference-registry.md`.

FAIL if a PENDING reference is treated as canon.

### Environment QA
PASS only if the environment ID exists and its layout remains consistent.

FAIL if:
- furniture moves without story reason
- window/layout changes
- lighting changes arbitrarily
- major permanent props disappear

### Dialogue QA
PASS only if:
- speaker is identified
- exact supplied dialogue is preserved
- dialogue is assigned to a visible character
- language matches the production requirement

### Lip-Sync QA
PASS only if:
- only the active speaker's lips move
- silent characters' mouths remain closed
- no wrong-character speaking occurs
- dialogue timing is clear

### Motion QA
PASS only if each clip has one clear primary action and movement is physically plausible.

### Continuity QA
PASS only if:
- character positions make sense between adjacent clips
- props remain consistent
- environment remains consistent
- food/items do not magically appear or disappear

### Canon QA
PASS only if the production plan does not silently modify established canon.

Any permanent change must be listed under `approval_required`.

## RELEASE GATE

A production plan is READY only when:

- all required QA checks = PASS
- no unresolved canon conflict exists
- all permanent references = APPROVED
- all required new assets are identified
- every dialogue clip contains strict lip-sync instructions

Otherwise status must remain `DRAFT` or `BLOCKED`.
