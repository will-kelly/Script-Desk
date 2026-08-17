# SME input model

Never ask an engineer: "Can you explain the product for this video?" That question produces accidental marketing copy. Ask targeted questions that produce raw technical truth.

## The targeted question set

1. What problem normally triggers this workflow?
2. What happens today without the product?
3. Where does the process usually fail?
4. What component actually performs this action?
5. What remains manual?
6. What does the product **not** do?
7. What prerequisite does the customer need?
8. What's the architectural tradeoff?
9. What would an experienced engineer challenge about this claim?
10. What is the best real-world scenario for demonstrating it?

Questions 5, 6, 8, and 9 feed the canvas tradeoff field and the register's adversarial check. They are not optional. An SME session that skips them produces a brochure.

## Extracting from SME transcripts or notes

When the user pastes SME material, extract into four buckets:

- **Mechanism facts** — what the system actually does, component by component. Feed the architecture segment.
- **Boundary facts** — what it doesn't do, what stays manual, prerequisites. Feed the tradeoff field.
- **Failure knowledge** — where the conventional approach breaks and where this one can. Feed the conventional-approach segment and the adversarial check.
- **Demonstration candidates** — real scenarios the SME describes. Feed the scenario segment.

Flag anything in the SME material that sounds like a marketing claim rather than a technical observation ("customers love that it's ten times faster"). Route it back: which measurement, which customer, which condition? It enters the register as `[NEEDS PROOF]`, not as fact.

## When SME input is missing

Output the targeted question list, scoped to the specific gaps in the canvas, formatted so the user can forward it directly to their SME. Do not simulate SME answers. Do not fill technical mechanism fields from general product-category knowledge — general knowledge about how these products usually work is not knowledge about how this product works.
