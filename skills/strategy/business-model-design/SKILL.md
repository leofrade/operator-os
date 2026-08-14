---
name: business-model-design
description: >-
  Turns a business model canvas from a documentation exercise into a diagnostic: which
  blocks carry weight at your stage, which are invention, and where the joints between
  them break. Use when unit economics do not work and nobody agrees why, when designing
  a new product line or pricing model, when evaluating a partnership or acquisition, or
  when two teams describe the same business differently.
domain: strategy
stage: any
lineage: "Alexander Osterwalder & Yves Pigneur — *Business Model Generation*"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Business Model Design

> A canvas is not a plan. It is a consistency check: a set of claims that have to survive being read next to each other.

## The question this answers

- Which part of this model is load-bearing, and which parts did we copy off a template?
- Why does it work on the slide and not in the P&L?
- What has to be true for this to make money, and which of those things have we tested?
- When we change the price, the channel, or the segment, what else breaks?

## When to run it

Run it when unit economics are wrong and the leadership team gives three different explanations. Run it before launching a second revenue line, before an acquisition or a deep partnership, and when a pricing change is proposed that touches how value is delivered rather than just how much you charge.

**Do not run this when** the problem is local and named — a churn spike, a discount policy, a single channel underperforming. The canvas is a whole-system tool, and pointing it at a local problem produces a long workshop and no decision. Do not run it in a startup's first month; seven of the nine boxes will be invention and the artifact will be treated as knowledge. And do not present a completed canvas as evidence to a board or an investor. It is a hypothesis map, and the credibility you spend defending invented boxes is expensive.

## The method

**Move 1 — Fill it in the order money moves, and mark every claim.**

Sequence: who the buyer is → what they currently pay to solve this → how you reach them → how you charge → what it costs to serve → what you must own to do it → who you depend on → what relationship the buyer expects.

Nothing enters a box without a source. Tag each item:

```
(A) observed  — we have data or a signed contract
(B) inferred  — reasonable from adjacent evidence
(C) invented  — we made it up and it sounds right
```

Count the Cs. On a first pass, five or six is normal and fine. The number is not the finding; where they sit is.

**Move 2 — Weight the blocks by stage. This is the whole diagnostic.**

Blocks are not equal, and which ones matter changes as the company changes.

| Stage | Load-bearing | Usually fiction on a first draft | Test first |
|---|---|---|---|
| Pre-PMF | Buyer, value, revenue mechanism | Partnerships, key activities, cost structure | Will this specific buyer pay this way |
| Go-to-market | Channel, relationship, revenue mechanism | Key resources, partnerships | CAC and payback per channel |
| Scale | Cost structure, key resources, partnerships | Buyer definition (has drifted), value (has gone stale) | Whether the buyer is still one segment |

Decision rule: you are allowed to be wrong about non-load-bearing blocks. Any block that is load-bearing at your stage and marked **(C)** is the next experiment, and it outranks whatever is currently on the roadmap.

**Move 3 — Check the four joints. Models break between blocks, not inside them.**

1. *Buyer ↔ channel.* Does the channel reach this buyer at a cost the deal size supports? If CAC exceeds first-year revenue, the model is quietly assuming a renewal you have not earned. Say that out loud and put a number on the required retention.
2. *Value ↔ revenue mechanism.* Are you charging for the thing that creates the value? If value scales with transactions and you charge per seat, value and revenue diverge over the life of the account and you will face permanent pricing pressure from your best customers.
3. *Revenue ↔ cost structure.* Is marginal cost per additional customer falling, flat, or rising? Rising means you have a services business modeled as a product. That can be a good business. It is not the one in the deck.
4. *Key resources ↔ partnerships.* Which partner could raise their price and take your margin? A load-bearing input with no contract and no substitute is the model's real risk, and it usually sits in the smallest box on the page.

**Move 4 — Stress the model against one archetype shift at a time.**

Rather than redesigning from nothing, test whether one structural move applies. Each has a precondition; without it, the move is a wish.

| Shift | Precondition that makes it real |
|---|---|
| Subsidize one side of a two-sided market | You can name which side is price-sensitive and which will pay, and show the paying side's willingness to pay rises with the free side's volume |
| Change the revenue mechanism rather than the price — usage, outcome, or subscription instead of asset sale | You can meter the thing accurately and the buyer accepts the meter as fair |
| Unbundle — split businesses whose economics fight each other | The piece you keep holds the compounding asset; the pieces you shed have genuinely incompatible economics |

Attempt one at a time. Two simultaneous archetype shifts produce a model nobody inside the company can explain, which shows up first as inconsistent sales pitches.

**Move 5 — Write the falsification list.**

Three sentences: "This model fails if ___." Each with a metric, a threshold, and a review date. If you cannot write three, you have not modeled anything — you have described the current business in nine boxes.

## Failure modes

**Canvas as documentation** — filled in retrospectively, everything accurate, nothing decided. The tell: nobody disagreed while filling it in. → Mark every item A/B/C. Disagreement about the tags is the output.

**Nine blocks of equal airtime** — the workshop spends as long on partnerships as on revenue. → Use the stage table and timebox the non-load-bearing blocks to five minutes each.

**Value written as adjectives** — seamless, integrated, intelligent. → Replace with the thing the buyer stops doing or stops paying for, and the number attached to it.

**One canvas covering three segments** — different buyers, channels, and prices on one sheet. The tell: the value statement needs "and" more than twice. → Different channel or different willingness to pay means a different canvas. Split it.

**Cost structure taken from the plan** — modeled costs instead of observed ones. The tell: the model's gross margin differs from last quarter's actual by more than ten points. → Use actuals. If there are none, mark it (C) and stop treating it as known.

**The freemium hand-wave** — a free tier with no measured cost to serve and no observed conversion rate. → Two numbers before launch: monthly cost per free user, and conversion at ninety days from a real cohort. Without both you have a marketing plan.

**Invisible partner dependency** — a data source, integration, or distributor that the model cannot survive losing, sitting in the smallest box. → Ask once a quarter who can raise their price on you, and write the substitute or the contract term next to their name.

**Redrawing instead of testing** — the canvas gets prettier every quarter and never gets validated. The tell: the (C) tags from two quarters ago are still (C). → Every load-bearing (C) gets an owner and a date, or the exercise is decoration.

## Outputs

- A canvas with every item tagged observed / inferred / invented
- The stage-weighted load-bearing table, with the invented load-bearing blocks named as the current experiment queue
- Four joint checks with numbers: CAC versus first-year revenue, the value-to-charging-basis match, the marginal cost direction, and the named partner concentration risk
- One archetype shift assessed against its precondition, with a go or no-go
- A three-line falsification list with metrics, thresholds, and review dates

## Pairs with

- [`gtm/pricing-power`](../../gtm/pricing-power/SKILL.md) — sets the revenue mechanism the value-to-charging joint depends on
- [`strategy/value-innovation`](../../strategy/value-innovation/SKILL.md) — rebuilds the offer and cost structure when the joints will not close
- [`discovery/experiment-design`](../../discovery/experiment-design/SKILL.md) — converts each load-bearing invented block into a cheap test
- [`strategy/platform-thinking`](../../strategy/platform-thinking/SKILL.md) — the precondition work for the two-sided shift in Move 4
- [`strategy/disruption-radar`](../../strategy/disruption-radar/SKILL.md) — when the model that will not close its joints is one your own funding rules would veto, which is a disruption signal rather than a design failure

## Lineage

Alexander Osterwalder and Yves Pigneur built *Business Model Generation* with a large community of practitioners, and gave organizations a shared visual language for how value is created, delivered, and captured. The lasting contribution is that the language is common enough for a finance lead, an engineer, and a salesperson to argue over the same sheet of paper. This articulation departs from theirs by refusing to treat the blocks as equally weighted, and by adding three things their version leaves to the facilitator: evidence tagging, a stage-dependent view of which blocks are actually load-bearing, and explicit checks on the joints between blocks — because a completed canvas is mostly invention presented as fact, and the models I have watched fail did not fail inside a box.
