# PACT framework reference

The video is not a miniature blog post or a narrated product brochure. It is a guided decision journey: operational problem → technical reality → useful decision.

**PACT: Problem → Architecture → Consequence → Takeaway.** Works from ~2-minute explainers through 10-minute technical marketing videos.

## 1. Problem — establish the operational tension

Goal: make the technical viewer recognize the situation before any solution appears.

Answer: what is happening, who experiences it, what breaks or slows or costs more, and why conventional approaches fail.

Script formula: **current state + friction + consequence.**

Banned opening pattern: "Modern enterprises are undergoing unprecedented digital transformation…"

Target opening pattern: "Your platform team standardized Kubernetes deployment. Your application teams still open tickets every time they need a production environment."

The opening must give the video something to resolve.

## 2. Architecture — show what is actually happening

This is where technical credibility separates the video from generic marketing content.

Cover as relevant: components, workflow, dependencies, data movement, control points, integration points, human responsibilities.

Governing question: **what does the audience need to understand about the system for the rest of the argument to make sense?** Everything else gets cut.

This section pairs with diagrams, animations, terminal captures, and workflow graphics — plan the visual track accordingly.

## 3. Consequence — translate architecture into meaning

Never jump from "here's how it works" to "book a demo." Ask: so what changes because the system works this way?

Work all three levels, explicitly:

| Level | Question |
|---|---|
| Technical | What becomes easier, safer, faster, or more reliable? |
| Operational | What workflow or organizational bottleneck changes? |
| Business | What becomes possible that wasn't practical before? |

Example (platform engineering):
- Technical: developers consume standardized environments.
- Operational: platform teams stop manually fulfilling routine requests.
- Business: the organization scales development without scaling platform-support workload at the same rate.

## 4. Takeaway — give the viewer a decision

The ending answers: what should the viewer now believe, investigate, change, or do? Four ending types:

- **Diagnostic** — "If your platform team spends more time fulfilling requests than improving the platform, the problem may not be infrastructure. It may be the interface between developers and infrastructure."
- **Strategic** — "Successful internal platforms don't eliminate platform engineering. They move platform engineers from ticket fulfillment toward designing reusable capabilities."
- **Product-oriented** — "That's the problem [product] is designed to address: exposing governed infrastructure capabilities through workflows developers can consume directly."
- **Action-oriented** — "Start by identifying the five infrastructure requests your platform team handles most frequently. Those are your strongest self-service candidates."

The CTA follows the takeaway as a logical next step. Never bolt an advertisement onto the end.

## Runtime map (4–6 minute baseline; scale proportionally)

| Time | Segment | Job |
|---|---|---|
| 0:00–0:20 | Cold open | Expose the contradiction, failure mode, or unexpected observation |
| 0:20–0:50 | Stakes | Why the problem matters operationally |
| 0:50–1:30 | Conventional approach | What teams usually do and where it breaks (room for the lightly contrarian POV) |
| 1:30–3:00 | System walkthrough | Input → workflow → control → output. The technical center |
| 3:00–4:00 | Scenario | The architecture in an actual operating situation |
| 4:00–4:45 | Implications | Technical behavior → operational consequences |
| 4:45–5:15 | Decision | Framework, question, recommendation, or next step |
| 5:15+ | CTA | Only now, the commercial action |

## The two-track rule

Technical video lives or dies by what the viewer sees. Every segment carries a spoken track and a visual track:

| Spoken track | Visual track |
|---|---|
| Explain problem | Show broken workflow |
| Introduce component | Highlight architecture component |
| Describe interaction | Animate data/workflow movement |
| Explain command | Show terminal or UI |
| Discuss consequence | Show before/after state |
| Summarize principle | Display short takeaway |

**Narration rule: never make the narrator describe something the viewer can understand faster by seeing it.** Show the click path; narrate why the action matters.
