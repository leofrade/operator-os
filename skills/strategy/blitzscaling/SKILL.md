---
name: blitzscaling
description: >-
  Decides whether to trade capital efficiency for speed, then runs the campaign if
  the answer is yes. Use when a competitor starts scaling into your market, when the
  board pushes for a much larger raise, when choosing between margin and market
  share, when planning hypergrowth hiring, or when someone says "we need to move
  faster" without naming what arriving first is actually worth.
domain: strategy
stage: scale
lineage: "Reid Hoffman & Chris Yeh — *Blitzscaling*"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Blitzscaling

> Speed is only worth paying for when the market pays a permanent premium to whoever arrives first. Everywhere else, blitzscaling is an expensive way to lose slowly.

## The question this answers

- Is this market genuinely winner-take-most, or does it only feel urgent?
- What does winning the race cost, and what specifically happens to us if we lose it?
- Which single constraint is capping growth right now, and what do we deliberately let break to remove it?
- When do we stop burning, and what tells us the campaign is over?

## When to run it

Run this when all three preconditions hold: (1) the market structure gives increasing returns to whoever gets scale first, (2) you have evidence of product/market fit rather than a belief in it, and (3) capital exists at the size the race requires. Also run it defensively, the moment a funded competitor starts spending like they believe the market is winner-take-most — even if you disagree, their spending changes the market.

**Do not run this when** growth is linear in spend with no compounding mechanism, when you are still testing which customer you serve, or when capital access is one investor's mood away from disappearing. In regulated, relationship-mediated, or capacity-constrained markets — professional services, most industrial B2B, anything gated by licensing or physical throughput — arriving first buys little, and the correct strategy is compounding efficiency. Blitzscaling those markets converts a decent business into a dead one.

## The method

### Move 1 — Run the precondition test before anything else

Blitzscaling is a bet, not a posture. Price the bet before you place it.

```
GATE 1 — STRUCTURE (must score 2+ on at least one)
  Direct network effect: value to user N rises with user N+1        0-3
  Two-sided liquidity: supply density improves demand conversion    0-3
  Data/learning loop: unit quality improves with cumulative volume  0-3
  Switching cost that compounds with tenure                         0-3
GATE 2 — EVIDENCE
  Retention curve flattens rather than decaying to zero            yes/no
  Organic or referred share of new accounts is rising              yes/no
GATE 3 — FUEL
  Committed capital covers 18-24 months at planned burn            yes/no

Rule: a zero on Gate 1, or a "no" on either Gate 2 line, ends the exercise.
Missing only Gate 3 means you have a fundraising problem, not a strategy.
```

The most common real outcome is a hard zero on Gate 1. A market can be large, fast-growing, and fashionable while still being fragmentable — thousands of viable competitors, none advantaged by size. Fragmentable markets punish speed. Say so before the plan is written, because once the round closes nobody wants to hear it.

### Move 2 — Price both outcomes, not just the upside

Write two numbers. First: the cost of winning — capital to the tipping point where the compounding mechanism carries growth without subsidy, plus a 50% overrun. Second: the cost of losing — what the company is worth after you have spent that capital, hired the org that spend implies, and finished second. If the losing case is a recoverable business at lower valuation, the bet is takeable. If the losing case is zero, you are betting the company, and that decision belongs in a board minute with your name on it, not in a growth plan.

### Move 3 — Name the binding constraint and remove exactly that one

Growth is capped by one thing at a time. Diagnose it against four candidates: addressable demand, distribution, gross margin, or the compounding mechanism itself. Test by asking what happens if you double spend on each — the constraint is the one where doubling spend changes nothing. Then attack only that one. Teams under pressure fund all four simultaneously and get four half-built capabilities.

Distribution is the constraint far more often than founders believe, and it is the one technical teams are least equipped to see. A merely good product with excellent distribution beats an excellent product with poor distribution almost every time.

### Move 4 — Buy the right to be badly managed

Deliberate inefficiency is the point, not a side effect. Decide in advance what you will let break and write it down: hiring bar for non-critical roles, documentation, career ladders, quarterly planning, support response times, cost per transaction. Then over-raise relative to plan — optionality is what you are buying, and the gap between an 18-month and a 30-month runway is the gap between negotiating and accepting.

The list matters more than the raise. An undocumented decision to run badly is indistinguishable from incompetence, and your best operators will leave over it.

### Move 5 — Triage fires by lethality, not by noise

You will always have more problems than capacity. Rank by three factors: which fire kills the company soonest, which can actually be put out now with available people, and which one, extinguished, makes two others smaller. Most consumer and self-serve businesses burn in roughly this order of lethality — distribution, product, revenue model, operations, competition. B2B inverts the first two. The skill is not firefighting; it is watching a real fire burn and not flinching, because the fire next to it is the one that kills you.

### Move 6 — Define the stop condition in writing, before you start

Blitzscaling is a campaign with an end, not an identity. Set exit criteria at the start: a share threshold, a date, a competitive event ("the second-place player stops raising"), or a unit-economics floor you refuse to breach. Review monthly. Companies that never define the end mistake burn for ambition and discover, three years later, that they built an organization that only knows how to spend.

## Failure modes

**Cargo-cult burn** — the plan reads like a hypergrowth plan, but growth is linear in spend, CAC is flat or rising, and retention is unchanged. There is no compounding mechanism; you are buying revenue at retail. → Stop the campaign, cut to an efficient growth model, and reinvest in whatever would create a compounding mechanism. Better to be a good business than a failed great one.

**Confusing a fast market with a winner-take-most market** — growth rates get used as proof of market structure. They are unrelated. Fast fragmentable markets attract capital, produce dozens of funded competitors, and end with everyone at 4% share and no margin. → Test structure with the Gate 1 scoring, not with growth rate.

**Raising for the narrative** — the round is sized to signal leadership rather than to fund a specific race. The company then has to act like a leader to justify the price, spending against a plan nobody believes. → Size the round against Move 2's two numbers. If the story requires a number the plan does not, fix the story.

**Letting the wrong fire burn** — leadership triages toward the fires they know how to fight, usually operational ones, while distribution quietly stops working. → Rank fires by lethality in writing each month, and force the ranking through a group that includes someone who owns growth.

**Hiring for the stage after next** — an executive built for a 500-person organization joins a 40-person one, brings process the company cannot absorb, and is bored within two quarters. → Hire for the next 12–18 months of scale, with an explicit conversation about what happens when the role outgrows the person. Being right for now beats being right eventually.

**Shipping the externality and paying later** — speed defers the harms: fraud, safety, data misuse, an incentive that quietly breaks something for users. At scale these stop being edge cases and become the story. → Separate risks that damage one part of the system from risks that can destroy the system itself. Systemic ones get fixed now, at full speed cost. Everything else gets monitored and logged.

**Never declaring the end** — burn persists past the point where it buys anything, because stopping feels like admitting the thesis was wrong. → Enforce the Move 6 stop condition. The transition to efficiency is a separate, planned, announced change of mode.

## Outputs

- A completed precondition scorecard with an explicit go / no-go and the reasoning
- Two numbers: cost of winning (with overrun) and value of the company if you lose
- A named binding constraint with the single funded plan to remove it
- A written accepted-debt list, time-boxed, with an owner for each item
- A monthly fire ranking by lethality, and the fires being deliberately ignored
- A written stop condition and the plan for switching back to efficiency

## Pairs with

- [`strategy/monopoly-thesis`](../../strategy/monopoly-thesis/SKILL.md) — establishes whether the market structure rewards being first at all, which is Gate 1's real question
- [`strategy/platform-thinking`](../../strategy/platform-thinking/SKILL.md) — designs the compounding mechanism that blitzscaling is meant to accelerate
- [`gtm/growth-loops`](../../gtm/growth-loops/SKILL.md) — the distribution machinery you fund once the constraint is named
- [`strategy/scaling-playbook`](../../strategy/scaling-playbook/SKILL.md) — the organizational work that keeps the company functional while you deliberately break parts of it

## Lineage

Reid Hoffman and Chris Yeh named and popularized blitzscaling in *Blitzscaling*, drawing on Hoffman's work at PayPal, LinkedIn, and Greylock. The core insight is theirs: in some markets, speed is worth more than efficiency, and first-to-scale becomes durable advantage.

This articulation departs from theirs on emphasis. The book reads as advocacy — the question is mostly how to blitzscale, not whether. Enough companies have now applied the playbook to markets with no compounding mechanism, and burned the capital anyway, that the honest version puts the precondition test first and treats a failed test as the expected result. That correction holds wherever capital is priced rather than free; in a market where growth is funded regardless of unit economics, the precondition test is what everyone skips. The stop condition, the two-number bet pricing, and the accepted-debt list are additions from operating practice, not from the book.
