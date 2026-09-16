---
name: purpose-narrative
description: >-
  Extracts a company's operating belief from its actual history, tests it for
  falsifiability, and reorders the story so belief precedes method precedes
  product — then audits whether incentives contradict the stated purpose.
  Trigger when writing a manifesto, founding story, or about page, when a pitch
  lands as a feature list, when values are decorative nouns nobody uses, when
  onboarding cannot explain why the company exists, or after a founder exit.
domain: brand
stage: any
lineage: "Simon Sinek — *Start With Why*"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Purpose Narrative

> A purpose statement is a claim about what you will refuse to do. If it does not constrain a decision someone would otherwise have made, it is wall art.

## The question this answers

- Why does our pitch land as a feature list even when the features are good?
- What do we actually believe, as opposed to what sounded good in the offsite?
- Our values are on the wall and nobody has ever used one to settle an argument. What went wrong?
- The founder left. How much of the company's story leaves with them?

## When to run it

Run this when you are writing a founding story, a manifesto, an about page, or a first-ninety-days onboarding narrative. Run it when a competent pitch keeps failing to move anyone, when new hires cannot explain what the company is for after a quarter, or when values exist but have never been cited in a real decision.

**Do not run this when** the problem is commercial rather than narrative. If deals stall on differentiation, buyers compare you to the wrong alternatives, or reps improvise their own pitch, run [`brand/positioning`](../../brand/positioning/SKILL.md) first — purpose sits on top of positioning and cannot substitute for it. Do not run it as a rescue for a product nobody wants; a belief cannot compensate for weak retention, and dressing weak retention in purpose language is how companies end up with a story their own employees privately mock.

## The method

Be honest about what this framework is and is not. The claim that starting with why *causes* commercial success is not testable — the famous examples are selected after the fact, and the neuroscience usually cited for it is decoration, not evidence. What survives scrutiny is narrower and still useful: narrative order changes comprehension and recall, a stated belief constrains decisions when it is specific enough to be violated, and a purpose that contradicts the incentive system is worse than no purpose at all, because it teaches everyone that the company's stated words are noise.

Work the moves in order. Move 4 is the one most teams skip, and skipping it is what produces the cynicism.

### Move 1 — Excavate, do not draft

Purpose is recovered from decisions, not generated in a workshop. Pull the record: why the founder started, what they walked away from, the customers they refused, the money they turned down, the feature everyone asked for that they would not build. Interview the three longest-tenured employees separately and ask what the company has consistently done that a rational competitor would not.

**Exit criterion:** you can name three real decisions, with dates, that a purely revenue-maximizing operator would have made differently. Fewer than three and you do not yet have a purpose — you have a preference.

### Move 2 — Write it so it can be violated

Draft one sentence: what you believe, and what that belief refuses. Then test it.

```
Falsifiability test
1. Name a profitable opportunity this belief forbids.        No → too vague
2. Could a direct competitor put this on their site?         Yes → too generic
3. Would anyone in the industry argue the opposite?          No → it is a platitude
4. Does it survive without the words empower, innovate,
   transform, passion, world-class?                          No → rewrite

Pass 4/4 or it is not a purpose statement.
```

"We believe people deserve better tools" fails all four. "We believe compliance work should be verifiable by the person doing it, not by an auditor twelve months later — so we will not ship features that only a specialist can operate" passes.

### Move 3 — Convert values into verbs with a decision rule

Nouns cannot be enforced. "Integrity" cannot be coached, scheduled, or reviewed. Rewrite each value as an instruction plus the tradeoff it costs you.

| Noun on the wall | Verb form | The cost it implies |
|---|---|---|
| Transparency | Publish the reasoning behind reversals, including your own | Slower decisions; visible mistakes |
| Craft | Ship late rather than ship something you would not demo | Missed dates, occasionally a lost deal |
| Customer obsession | Refuse configurations you cannot support at scale | Declined revenue you can name |

A value with no stated cost is not a value; it is a preference everyone already holds. The cost column is the whole exercise.

### Move 4 — Audit incentives before publishing anything

This is where purpose work usually dies. Lay the stated belief next to the compensation plan, the promotion criteria, the top three dashboards, and the last five things that got someone praised in public. Mark every direct contradiction.

Fix the contradiction or change the statement. Publishing a belief your comp plan punishes is not aspiration, it is a credibility loss you will pay for in every subsequent internal announcement. If quota accelerators reward volume while the stated purpose is fit, the purpose is already dead and everyone in the room knows it.

**Exit criterion:** zero unresolved contradictions between the statement and what the company measures and pays for.

### Move 5 — Reorder the narrative, then test it in one channel

Only now write the story: belief, then how you work, then what you sell as evidence of both. The order matters because it gives the listener a reason to care before you ask them to evaluate specs — but the belief has to be followed quickly by proof, or you sound like a company with nothing to demo.

Do not roll it out everywhere. Run it in one channel against the current version for four weeks — one landing page, one outbound sequence, one first-call opening. Compare a real conversion metric, not applause.

**Exit criterion:** a measured difference in one channel, or an honest verdict that the story is neutral and the constraint lies elsewhere.

## Failure modes

**Retrofitted purpose** — the belief is reverse-engineered from what already worked, so it explains the past and predicts nothing. The tell is that it fits every decision you have ever made. → Return to Move 1 and demand decisions that cost money.

**The unfalsifiable statement** — it survives review because nobody can disagree with it, which is exactly the problem. The tell is unanimous approval in the first meeting. → Apply the Move 2 test; a purpose with no opponent constrains no one.

**Purpose without proof** — the pitch opens with belief and never reaches evidence, so a technical buyer files it as marketing. The tell is prospects politely asking to skip ahead. → Belief first, proof within ninety seconds. In enterprise sales, purpose earns attention; it does not close.

**Incentive contradiction** — the wall says one thing, the comp plan pays for another, and employees resolve the conflict correctly by following the money. The tell is a value nobody has cited in a decision this year. → Move 4. Change the plan or delete the value.

**Borrowed neuroscience** — the argument is defended with brain-layer claims rather than with what the company actually does. The tell is a deck slide about the limbic system. → Cut it. Defend the narrative order on comprehension and recall, and defend the belief with decisions.

**Purpose as compensation substitute** — mission language is used to justify below-market pay or unreasonable hours. The tell is purpose invoked most loudly during retention conversations. → Purpose is not currency. Pay properly and let the belief do the work it can do.

**Founder-dependent story** — the belief lives only in one person's retelling and evaporates on their exit. The tell is that nobody else can tell the origin story without hedging. → Document the three decisions from Move 1 and make them part of onboarding, so the story is institutional rather than biographical.

## Outputs

- A decisions dossier: three or more choices, with dates, that a revenue-maximizing operator would have made differently.
- A one-sentence belief statement with its 4/4 falsifiability score recorded.
- Three to five values in verb form, each with the cost it imposes.
- An incentive-contradiction table with a resolution per row.
- A narrative in belief-method-product order, in the three formats you actually use: landing page, first-call opening, and internal onboarding.
- The single-channel test plan, with the metric and the review date.

## Pairs with

- [`brand/positioning`](../../brand/positioning/SKILL.md) — establishes the frame this narrative sits on top of; run it first if buyers are comparing you to the wrong things.
- [`revenue/value-messaging`](../../revenue/value-messaging/SKILL.md) — supplies the proof layer that must follow the belief within ninety seconds.
- [`brand/presentation-craft`](../../brand/presentation-craft/SKILL.md) — sequences this narrative into slides and decks without letting the belief crowd out the evidence.
- [`brand/founder-narrative`](../founder-narrative/SKILL.md) — the individual-level counterpart; this file is the company's belief, that one is the person who carries it.

## Lineage

Simon Sinek's *Start With Why* is the source of the belief-before-product ordering and of the insistence that values expressed as nouns are unenforceable. Both hold up in practice, and the second is underrated — rewriting values as verbs with explicit costs is one of the cheapest high-yield exercises available to a founding team.

This articulation departs from the source on the parts that do not survive contact with evidence. The Golden Circle is presented there as a causal theory, but it is unfalsifiable as stated and its canonical examples are selected after their success; the supporting brain-anatomy argument is popular neuroscience rather than a finding. What is kept here is the operational residue: narrative order, values as verbs, and the discipline of naming what a belief forbids. What is added is the incentive audit, on the view that a purpose statement contradicted by the compensation plan is not merely ineffective — it actively teaches an organization to discount everything else leadership says.
