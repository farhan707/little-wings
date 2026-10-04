# Little Wings — Reference Registry

## Purpose
Machine-readable index for approved and pending visual references.

| Reference ID | Type | Characters | Environment | Status | File |
|---|---|---|---|---|---|
| REF_MASTER_GIRL_001 | MASTER | CHAR_GIRL_001 | — | **APPROVED** | Asset upload pending |
| REF_MASTER_BOY_001 | MASTER | CHAR_BOY_001 | — | **APPROVED** | Asset upload pending |
| REF_MASTER_MOTHER_001 | MASTER | CHAR_MOTHER_001 | — | **APPROVED** | Asset upload pending |
| REF_MASTER_FATHER_001 | MASTER | CHAR_FATHER_001 | — | **APPROVED** | Asset upload pending |
| REF_MASTER_CHILDREN_DINING_001 | MASTER | CHAR_GIRL_001, CHAR_BOY_001 | ENV_DINING_001 | PENDING | — |
| REF_MASTER_MOTHER_CHILDREN_DINING_001 | MASTER | CHAR_GIRL_001, CHAR_BOY_001, CHAR_MOTHER_001 | ENV_DINING_001 | PENDING | — |
| REF_MASTER_FAMILY_DINING_001 | MASTER | CHAR_GIRL_001, CHAR_BOY_001, CHAR_MOTHER_001, CHAR_FATHER_001 | ENV_DINING_001 | **APPROVED** | APPROVED CLEAN SINGLE-VIEW DINING ENVIRONMENT MASTER (asset upload pending) |

## Approved References

### REF_MASTER_GIRL_001
- Character: CHAR_GIRL_001
- Status: APPROVED
- Purpose: Primary individual identity reference for the older sister.
- Approved visual: 3D cartoon character sheet with front, 3/4, side, back, facial expressions, action poses, family context, and detail views.
- Approval: User-approved.
- Asset file: Conversation workspace; repository binary upload pending.

### REF_MASTER_BOY_001
- Character: CHAR_BOY_001
- Status: APPROVED
- Purpose: Primary individual identity reference for the younger brother.
- Approved visual: 3D cartoon character sheet with front, 3/4, side, back, facial expressions, action poses, family context, and detail views.
- Approval: User-approved.
- Asset file: Conversation workspace; repository binary upload pending.

### REF_MASTER_MOTHER_001
- Character: CHAR_MOTHER_001
- Status: APPROVED
- Purpose: Primary individual identity reference for the mother.
- Approved visual: 3D cartoon character sheet with front, 3/4, side, back, facial expressions, action poses, family context, and detail views.
- Canon details: Red traditional Pakistani outfit, matching red dupatta, shoulder-length dark hair, warm expressive facial features, consistent Little Wings 3D style.
- Approval: User-approved.
- Asset file: Conversation workspace; repository binary upload pending.

### REF_MASTER_FATHER_001
- Character: CHAR_FATHER_001
- Status: APPROVED
- Purpose: Primary individual identity reference for the father.
- Approved visual: 3D cartoon character sheet with front, 3/4, side, back, facial expressions, action poses, family context, and detail views.
- Canon details: South Asian/Pakistani father, dark formal suit with white shirt, short dark hair, warm expressive facial features, neat light stubble, consistent Little Wings 3D style.
- Approval: User-approved.
- Asset file: Conversation workspace; repository binary upload pending.

### REF_MASTER_FAMILY_DINING_001
- Characters: CHAR_GIRL_001, CHAR_BOY_001, CHAR_MOTHER_001, CHAR_FATHER_001
- Environment: ENV_DINING_001
- Status: APPROVED
- Purpose: Primary family composition reference for scenes where all four family members appear together in the dining environment.
- Approved visual: Clean single-view 3D dining environment master with no characters, designed as the primary video-generation environment reference. It preserves the established dining/kitchen layout, furniture, window, lighting, plants, shelving, refrigerator, rug, table runner, and breakfast props.
- Canon rule: Preserve character identity, seating relationship, dining layout, major props, and visual style when using this reference.
- Approval: User-approved.
- Asset file: User-approved clean single-view Dining Environment master generated in the current production workspace; repository binary upload pending.

## Important
Only references marked APPROVED may be used as permanent canon by automation.

Automation must check Status before using a reference as canon.
