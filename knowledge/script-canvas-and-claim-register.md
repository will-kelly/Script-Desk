# Script canvas and claim register

Both artifacts get completed before any script prose exists. The canvas defines the argument; the register validates it.

## Script canvas

Fill every field from real input or flag it. No plausible guesses.

| Field | Question | Entry |
|---|---|---|
| Audience | Who specifically is watching? | [ ] |
| Decision | What should they understand or decide afterward? | [ ] |
| Operational problem | What recurring situation creates the need? | [ ] |
| Failure mode | Why doesn't the existing approach work? | [ ] |
| Technical mechanism | What changes technically? | [ ] |
| Proof | What evidence supports the argument? | [ ] |
| Scenario | What concrete workflow demonstrates it? | [ ] |
| Tradeoff | What limitation, requirement, or architectural choice should be acknowledged? | [ ] |
| Business consequence | Why does the technical change matter operationally? | [ ] |
| Takeaway | What's the single sentence worth remembering? | [ ] |
| CTA | What's the natural next action? | [ ] |

Flag values: `[NEEDS SME]` (technical fact only an SME can supply), `[NEEDS INPUT]` (business/audience fact only the user can supply), `[NEEDS PROOF: description]` (assertion awaiting evidence).

Open flags on **technical mechanism, proof, or tradeoff** block scripting. Open flags elsewhere block final delivery.

## Claim register

One entry per major assertion the video will make.

| ID | Claim | Proof | Visual | Implication | Status |
|---|---|---|---|---|---|
| C1 | [assertion] | [artifact] | [what the viewer sees] | [why it matters] | VALIDATED / UNVALIDATED |

Worked example:

| ID | Claim | Proof | Visual | Implication | Status |
|---|---|---|---|---|---|
| C1 | Self-service reduces platform-team intervention | Workflow demonstration + validated SME explanation | Developer provisioning an environment without a ticket | Platform engineering moves toward reusable capabilities rather than fulfillment work | VALIDATED |

### Proof standards

Acceptable proof: workflow demonstration, observable architecture behavior, named customer evidence the user supplies, published third-party data the user supplies or cites, validated SME explanation.

Not proof: "everyone knows," competitor marketing, an unattributed statistic, the writer's intuition, SME enthusiasm without a mechanism.

### Status rules

- `UNVALIDATED` claims never appear in the spoken track as assertions. Options: convert to a question the video raises, downgrade to a hedged observation with the hedge visible, or cut.
- Never invent metrics, benchmarks, percentages, customer names, or analyst citations to move a claim to VALIDATED. The register holds `[NEEDS PROOF]` until the user supplies evidence.
- Register IDs appear in the final script as production notes so every narration line traces back to its validation.
