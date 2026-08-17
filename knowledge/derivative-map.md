# Derivative map — the validated script as source asset

The approved script is not the end of the pipeline. It is the source asset in a governed knowledge transformation chain:

**SME knowledge → claims → video argument → validated script → production → derivatives**

Derivatives are generated only after the Stage 6 validation gate passes. This ordering is the point: derivatives inherit the script's validation, so a claim error never multiplies across nine formats.

## Standard derivative set

From one validated script, offer:

| Derivative | Source segments | Notes |
|---|---|---|
| Technical article | Full PACT arc | Rebuild for reading, don't transcribe narration |
| Architecture explainer | Architecture + scenario | Pairs with the visual-track diagrams |
| Short video clips | Cold open, scenario, decision | Each clip must stand alone with its claim intact |
| LinkedIn posts | Cold open contradiction, consequence levels, diagnostic takeaway | One argument per post |
| Sales-enablement snippets | Consequence (three levels) + tradeoff | Include the tradeoff — reps get burned by scripts that hide it |
| Demo narration | System walkthrough + scenario | Visual track becomes the demo path |
| FAQ | Boundary facts, tradeoffs, SME adversarial answers | The "what it doesn't do" material finally earns its keep |
| Executive summary | Consequence (business level) + takeaway | Decision-framed, one page |
| Technical diagrams | Visual track specifications | Hand to design with the claim IDs attached |

## Rules

- Every derivative carries its claims' register IDs in production notes, same as the script.
- A derivative may narrow a claim, never widen it. "Reduces intervention for routine requests" cannot become "eliminates tickets" in the LinkedIn version.
- If a claim is later invalidated, the register identifies every derivative that carried it. That traceability is why the IDs exist.
- Derivatives requested from an unvalidated script get refused with the open flags listed.
