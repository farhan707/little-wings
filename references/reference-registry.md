# Little Wings — Reference Registry

## Purpose
Machine-readable index for approved and pending visual references.

| Reference ID | Type | Characters | Environment | Status | File |
|---|---|---|---|---|---|
| REF_MASTER_GIRL_001 | MASTER | CHAR_GIRL_001 | — | PENDING | — |
| REF_MASTER_BOY_001 | MASTER | CHAR_BOY_001 | — | PENDING | — |
| REF_MASTER_MOTHER_001 | MASTER | CHAR_MOTHER_001 | — | PENDING | — |
| REF_MASTER_FATHER_001 | MASTER | CHAR_FATHER_001 | — | PENDING | — |
| REF_MASTER_CHILDREN_DINING_001 | MASTER | CHAR_GIRL_001, CHAR_BOY_001 | ENV_DINING_001 | PENDING | — |
| REF_MASTER_MOTHER_CHILDREN_DINING_001 | MASTER | CHAR_GIRL_001, CHAR_BOY_001, CHAR_MOTHER_001 | ENV_DINING_001 | PENDING | — |
| REF_MASTER_FAMILY_DINING_001 | MASTER | CHAR_GIRL_001, CHAR_BOY_001, CHAR_MOTHER_001, CHAR_FATHER_001 | ENV_DINING_001 | PENDING | — |

## Important
These IDs are reserved registry entries. They do not claim that the corresponding image files are already approved.

Automation must check `Status` before using a reference as canon.
