# Script Desk — technical video script architect

A Claude Project that turns SME input into validated two-track technical marketing video scripts, then treats the validated script as the source asset for a governed derivative chain.

Built on the PACT framework (Problem → Architecture → Consequence → Takeaway) with claim gating: every assertion in the spoken track traces to a register entry with real proof, and derivatives are locked until the script clears a validation gate.

## The failure modes this exists to prevent

Most technical marketing videos fail the same four ways. Script Desk is architected against each one.

**1. The narrated brochure.** The video describes the product instead of resolving a problem. Countermeasure: the PACT structure forces an operational tension in the first 20 seconds and bans the "unprecedented digital transformation" opening species.

**2. The authoritative-sounding unvalidated claim.** A script sounds credible while containing assertions nobody checked. Countermeasure: the claim register (claim → proof → visual → implication). UNVALIDATED claims cannot enter the spoken track as assertions. No invented metrics, ever.

**3. The narrator describing what the viewer can see.** Countermeasure: two-track scripting with a hard narration rule — the visual track carries the mechanics, narration carries the meaning.

**4. Multiplying an error across nine formats.** Repurposing an unchecked script spreads a wrong claim into articles, clips, posts, and sales decks. Countermeasure: derivatives are gated behind validation, carry claim IDs for traceability, and may narrow a claim but never widen it.

## Architecture

Six-stage pipeline:

1. **Intake and canvas** — 11-field script canvas; gaps flagged `[NEEDS SME]` / `[NEEDS INPUT]`, never guessed
2. **SME synthesis** — targeted question set that extracts technical truth instead of accidental ad copy
3. **Claim register** — claim → proof → visual → implication, with proof standards
4. **PACT architecture** — segment mapping and runtime allocation
5. **Two-track script** — spoken + visual tracks with inline claim IDs
6. **Validation gate → derivative map** — checklist pass, then the script becomes the source asset

## Files

```
instructions.md                              — the pipeline, guardrails, and refusals
knowledge/pact-framework.md                  — PACT reference, runtime map, two-track rule
knowledge/script-canvas-and-claim-register.md — canvas and register templates
knowledge/sme-interview-guide.md             — SME question set and extraction model
knowledge/product-fact-sheet.md              — bracketed template; all product-specific detail isolated here
knowledge/derivative-map.md                  — post-validation derivative chain and traceability rules
test-harness.md                              — 12 scenarios, 9 seeded traps
```

## Pattern lineage

- **Claim gating against a product fact sheet** — extends Signal Desk's approach; the fact sheet is the only source a VALIDATED claim can cite
- **`[NEEDS SME]` flagging over smoothing** — from Signoff: unconfirmed facts get tagged, never absorbed into confident prose
- **No-invented-metrics guardrail** — from the Search Desk / no-invented-metrics pattern; numbers wait for evidence
- **Company-specific isolation in swappable knowledge files** — re-platforming to a new product means replacing `product-fact-sheet.md`, not rewriting the instructions
- **New contribution: validation-gated derivative chain** — the claim register's IDs travel into every derivative, so a later invalidation identifies everything that carried the claim

## Setup

1. Create a Claude Project, paste `instructions.md` as the project instructions.
2. Add the five knowledge files to project knowledge.
3. Fill `product-fact-sheet.md` for the target product. Leave nothing to inference — empty brackets are safer than plausible guesses.
4. Run the harness before first client use.
