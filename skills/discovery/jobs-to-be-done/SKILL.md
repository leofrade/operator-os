---
name: jobs-to-be-done
description: >-
  Converts messy customer conversations into a stable job statement and a ranked
  set of outcome metrics, using the cheap subset of outcome-driven innovation that
  a team without a research budget can actually run. Use when defining what job a
  product is hired for, writing outcome statements, choosing which unmet need to
  attack, deciding between premium and cheaper positioning, or diagnosing a
  roadmap that is a pile of feature requests.
domain: discovery
stage: pre-pmf
lineage: "Anthony Ulwick — *Jobs to Be Done: Theory to Practice*; Clayton Christensen — *Competing Against Luck*"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Jobs To Be Done

> Customers cannot tell you what to build, but they can tell you exactly how they judge whether it worked. Stop collecting requests; collect the metrics they grade you on.

## The question this answers

- "My roadmap is a list of things customers asked for. Which ones matter?"
- "What does this actually compete against, and why do we keep losing to spreadsheets?"
- "We know the problem. Which part do we solve first?"
- "Should we be the expensive better option or the cheap sufficient one?"

## When to run it

Run this once you have a working segment and interview notes containing concrete incidents. Input is transcripts and observed behavior; output is a job statement and a ranked list of unmet outcomes that survives a roadmap argument. Run it when the team argues about features with no shared criterion for saying no, or when you need a positioning claim that is not a slogan.

**Do not run this when** you have not spoken to customers: this organizes evidence, it does not manufacture it. It is also not a substitute for shipping. Time-box the whole exercise to two weeks — it is finished when it has killed one roadmap item and promoted another, and if nothing moved it was decoration.

**Honest boundary.** The complete outcome-driven method — dozens of practitioner tasks, surveys of hundreds to thousands of respondents, cluster analysis to find need-based segments — is a consulting engagement built for corporations with research staff and six-figure study budgets. Pre-product-market-fit with ten customers, running it is theater: you cannot reach statistical validity, so you produce precise-looking numbers your sample cannot support. What follows is the subset that pays for itself at small scale.

## The method

### 1. Write the job statement, then try to break it

One sentence: an action verb, the object acted on, the context that bounds it. "Keep a distributed team's shared records accurate." "Move oversized freight legally between two points." No emotions, no technology, no product. Then attack it:

| Test | Question | Failure signal |
|---|---|---|
| Stability | True twenty years ago, still true in twenty more? | It names a technology or a channel |
| Solution-freedom | Could a rival satisfy this with software, a service, or a person? | Only your product could |
| Scope | Could you own the job end to end within a few years? | You cannot fund it, or someone else owns the larger job |

Decision rule: if it fails stability or solution-freedom, rewrite before anything else — everything downstream inherits the defect. Most first drafts describe the product with the brand name removed.

Then set the altitude. Too narrow and a rival covering the whole job absorbs you as a feature; too broad and you cannot address it. Aim for the widest job you could credibly own in three years, then test against the status quo: name what people hire today to do it. "A spreadsheet and two phone calls" means the altitude is right. "Nothing, it never comes up" means it is too narrow or does not exist.

### 2. Map the job in three phases and hunt the edges

Sketch three phases: **getting set up** (deciding, gathering inputs, preparing), **doing the thing**, and **verifying and closing out** (checking, correcting, filing, handing off). Walk each with a customer and record where time is lost and where errors start.

Why this is worth an afternoon: most products optimize the middle, and most of the pain lives at the edges. Setup and verification hold the workarounds, the duplicate entry, the anxiety. A roadmap living entirely in the middle is competing on the crowded stretch.

### 3. Harvest outcome statements — twenty, not two hundred

An outcome is how the customer measures success at a step, written measurably, with no solution in it.

```
[minimize | increase] + [time, number, frequency, likelihood] + [of what] + [in what context]

"Minimize the time needed to confirm a submitted record was accepted."
```

Pull these from transcripts you already have, not from a workshop. Every complaint, workaround, and request converts into one: ask what the person was trying to measure when they got annoyed. "I want bulk upload" becomes "minimize the time needed to enter a batch of records."

Threshold: twenty to thirty across the three phases is enough to decide with. The formal method produces over a hundred, which only pays off if you survey a large sample against them. Quality gate: measurable, controllable by whoever does the job, free of implied solutions. If you cannot imagine two very different products both improving it, rewrite it.

### 4. Rank importance against satisfaction — by hand

Take the list to eight to fifteen people in the segment. For each outcome, ask how much it matters and how well their current approach handles it. You need the gap, not the decimal. Sort into three piles:

- **High importance, low satisfaction** — the opportunity. Everything you build first comes from here.
- **High importance, high satisfaction** — table stakes. Match it, never lead with it; marketing that leads here sounds like every competitor.
- **Low importance, high satisfaction** — overserved. Strip cost out, or concede it to a cheaper rival.

Decision rule: if nothing lands in the first pile, this segment has no innovation opportunity — it is well served, so change segments or compete on cost. That is a legitimate answer, and cheap to learn here.

The formal version scores this over large samples to find clusters with the same unmet outcomes. If your market is large and you can fund a real study, buy it. Do not fake it with twelve responses.

### 5. Let the ranking pick the posture

| What you found | Posture |
|---|---|
| Intense unmet outcomes, willingness to pay more | Clearly better, priced higher — narrow segment, high service expectations |
| Unmet outcomes plus a cost structure you can beat | Better and cheaper — strongest position, hardest to build, unanswerable by incumbents |
| Mostly overserved people, plus non-consumers priced out | Worse and far cheaper; accept inferiority deliberately, move upmarket later |

One threshold to hold onto: people do not switch for marginal gains. If your improvement is not large enough that a user would describe it unprompted, assume they stay. Slight improvement is available only to incumbents defending a base.

## Failure modes

**The job statement is your product with the brand filed off** — "manage compliance documents in one place" dies the moment a competitor bundles it. The tell: no incumbent exists for the job as written except software like yours. → Ask what the person was accomplishing such that documents came up at all, and write the statement one level above the artifact.

**Outcomes that are features in costume** — "provide a bulk upload button" scored as an outcome. The customer cannot measure it, and it forecloses the design space. → Apply the two-products test: if you cannot name two genuinely different ways to improve the statement, it is a solution. Rewrite it as a quantity they would notice changing.

**Importance without satisfaction** — the team ranks what matters most, builds the top of that list, and ships something competent at exactly what customers already get elsewhere. The most common way a roadmap wastes a year. → Never act on importance alone. The gap is the whole signal; a high-importance, well-served outcome is a requirement to match, not an opportunity.

**False precision from a small sample** — scoring formulas and cluster charts derived from fourteen interviews. It looks like research, it is arithmetic on noise, and it is persuasive to boards. → At small n, report ranks and gaps, never scores, and keep sample size visible.

**Confusing the job executor with the buyer** — you optimize for the operator and lose the deal, because the buyer was measuring payback period, switching risk, and whether anyone gets fired for choosing you. → Keep a short separate list of the buyer's financial and risk outcomes and check your top opportunities against it. Otherwise you have a great product and no purchase order.

## Outputs

1. A **job statement** with the three tests applied and results shown.
2. A **three-phase job map** annotating pain, workarounds, and time loss.
3. Twenty to thirty **outcome statements**, sorted by phase, each traceable to a transcript.
4. An **importance-versus-satisfaction sort**, with sample size on it.
5. A **posture recommendation** with its evidence.
6. A **roadmap delta**: what this kills, what it promotes, and the outcome each promoted item moves.

## Pairs with

- [`discovery/customer-interviews`](../../discovery/customer-interviews/SKILL.md) — supplies the raw incidents; this is unusable without them.
- [`discovery/venture-design`](../../discovery/venture-design/SKILL.md) — unmet outcomes become the quantified value proposition and competitive position.
- [`brand/positioning`](../../brand/positioning/SKILL.md) — the top unmet outcome is the only honest source of a differentiated claim.
- [`discovery/build-measure-learn`](../../discovery/build-measure-learn/SKILL.md) — turns "we believe this outcome is unmet" into a falsifiable test.
- [`strategy/monopoly-thesis`](../../strategy/monopoly-thesis/SKILL.md) — tests whether the top unmet outcome defines a market narrow enough to own, or is a feature someone larger will absorb.

## Lineage

Anthony Ulwick built outcome-driven innovation on the insight that customers can state the metrics by which they judge a job even when they cannot design the solution, and formalized it into a research process with a real track record inside large firms. Clayton Christensen popularized the causal framing: people hire products to make progress, and the competitor is often a workaround or nothing at all.

This departs in one deliberate way. Ulwick's rigor depends on research at a scale most startups cannot fund, and a hollow version produces confident nonsense. So this keeps the discipline that is cheap — the statement tests, the outcome structure, the importance-satisfaction gap — says plainly that the scored, survey-based portion is a consulting engagement, and gives the small-team substitute with its limits attached.
