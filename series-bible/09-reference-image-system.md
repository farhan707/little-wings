# Little Wings — Reference Image System

## Objective
Maintain visual consistency with a small set of high-value master references.

## Master Reference Principle
Do not generate a separate reference image for every scene.

Prefer master references that cover recurring character combinations and environments.

## Recommended Reference Types
- Children + breakfast table
- Children + mother + breakfast/dining environment
- Full family + dining/living environment
- Individual character master references
- Individual environment master references

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
Automation should select the smallest suitable set of approved references that fully covers the scene.

## Master vs Episode Reference
Master references define stable identity.
Episode references may define temporary scene-specific composition.

Episode references do not change master canon unless explicitly promoted.

## Failure Rule
If no suitable reference exists, flag the scene for reference creation instead of silently inventing a new canon design.
