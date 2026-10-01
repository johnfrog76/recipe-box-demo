---
description: The contract for scaling a recipe by servings.
---
# Spec: scale a recipe by servings

> GitHub: https://github.com/johnfrog76/recipe-box-demo/issues/6

| Decision | Rule |
|---|---|
| D-1 | A recipe has a base serving count; scaling multiplies every quantity by target / base |
| D-2 | A countable unit (egg, clove) rounds up to a whole number |
| D-3 | A quantity marked `to taste` or `pinch` does not scale |
| D-4 | Quantities are rationals end to end; the display picks the nearest kitchen fraction |

## Acceptance

- 4 to 6 servings: 1/3 cup becomes 1/2 cup, 1 egg becomes 2 eggs, a pinch stays a pinch.
