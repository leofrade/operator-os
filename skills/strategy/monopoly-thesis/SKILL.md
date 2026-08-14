---
name: monopoly-thesis
description: >-
  A scored self-assessment that tells a founder whether a venture can own a market or
  is a better version of something that already exists, and whether it is fundable yet.
  Use before a raise, before committing a year to a direction, when choosing between
  two ideas, when a deck claims a small share of a huge market, or when someone asks
  what makes this defensible and the answer is a feature list.
domain: strategy
stage: pre-pmf
lineage: "Peter Thiel & Blake Masters — *Zero to One*"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Monopoly Thesis

> Competition is usually evidence that you picked a problem someone has already solved. The work is proving you can own a market small enough that nobody is fighting you for it yet.

## The question this answers

- Is this genuinely new, or a nicer version of a thing that exists?
- What is the smallest market we could hold more than half of within two years?
- Are we ready to raise, or would a competent investor find the hole in twenty minutes?
- What do we believe that our competitors' spending shows they do not?

## When to run it

Run it before a fundraise, before committing twelve months of build to a direction, and when choosing between two viable ideas. Re-run it after any pivot that changes the buyer.

**Do not run this when** you have a working motion at scale and the real question is execution quality — this frame becomes an excuse to avoid competing. Do not run it on a business that is honestly a good services company with healthy margins; not everything worth owning is a monopoly, and forcing the frame produces fiction that then gets pitched. And do not run it as a fundraising exercise. The output is a list of things wrong with your company. If you run it to generate deck slides, you will score in pitch voice and learn nothing.

## The method

**Move 1 — State the contrarian claim so it can be wrong.**

```
Most operators in [category] believe X.
We believe [not-X].
If we are right, [specific consequence] happens within [timeframe].
Evidence they believe X: [a competitor's investment decision in the last 18 months
that only makes sense if X is true].
```

The evidence line is the test. If you cannot name a rival's budget, hire, or roadmap choice that only makes sense under X, your claim is not contrarian — it is unstated, and everyone already agrees. Widely shared complaints ("this industry is broken", "buyers hate the incumbents") are consensus wearing a contrarian jacket.

**Move 2 — Define the market until it is embarrassingly small.**

Write down the buyer list. Not a segment description — a list. If you cannot name 100 specific accounts or bound a population precisely, you have a category, not a market.

Threshold: could you plausibly hold more than 50% of that list within 18 to 24 months, using the team you have or can hire in two quarters? If the answer depends on a sales organization you have not built, cut the market smaller and re-ask. "One percent of a very large market" is the standard failure. Invert it: what is the definition under which you would be at half?

**Move 3 — Score seven dimensions, alone, in writing.**

The dimensions: **breakthrough** (is the thing an order of magnitude better on something a buyer names, not 20% better), **timing** (why is now different from three years ago), **beachhead** (large share of a small market from Move 2), **team** (right people, and can they sell), **distribution** (a named channel with known economics), **durability** (position defensible in ten years), **secret** (an insight the market has not priced).

The scoring protocol is the part that matters, because these dimensions are famous enough that founders can answer them fluently and dishonestly:

1. Score 1–10 alone, in writing, before any discussion.
2. For every score above 6, write the one piece of evidence a hostile stranger could verify. **No verifiable evidence, the score drops to 4.** This rule does most of the work.
3. Have one co-founder and one outsider with domain knowledge score independently. Any dimension with a spread of 3 or more is not scored — it is unresolved, and resolving it is a task.
4. Do not average. The statistics that matter are the minimum and the count below 5.

Reading the result:

| Profile | Meaning | Action |
|---|---|---|
| Nothing above 7 | Nothing here is exceptional | Not a company yet. Re-scope or stop. |
| Two or more below 4 | Multiple unresolved fatal risks | Do not raise. You will get funded on story and die on substance. |
| One below 4, rest at 6+ | A single named risk | Raise only if you can state the experiment that resolves it, its cost, and its deadline. |
| Minimum at 6, two at 9+ | Fundable | Raise. Lead with the two nines; do not hide the six. |

Weight the fixables differently. Distribution and team are usually buyable with time and money. Timing and secret are not — a 3 on timing is fatal in a way a 3 on distribution is not, and founders routinely treat them as equivalent.

**Move 4 — Pressure-test durability against the copy.**

Assume your current advantage is public and cloned in eighteen months. What still holds? Acceptable answers compound with use: network effects, scale economics with a real cost curve, proprietary data inside a feedback loop, switching costs the buyer has already paid. Unacceptable answers: a feature lead, a head start, a partnership without exclusivity, brand you have not yet earned.

**Move 5 — Pick one distribution channel before you build.**

Distribution follows a power law: one channel almost always dominates and the rest are noise. Name it, then write CAC, payback period, and whether the deal size supports the motion. Watch the dead zone — contract values that are too large for pure self-serve and too small to pay a rep are a structural problem, and the fix is changing price or motion, not adding channels.

**Move 6 — Write the memo you would not send to an investor.**

One page: the claim, the buyer list, the minimum score and which dimension holds it, the single experiment that would move it, and the date. If the memo says "do not raise yet", that is the output. It is worth more than the round.

## Failure modes

**Contrarian theater** — a claim that gets nods at every conference. The tell: nobody argues with it. → If it does not make a smart peer visibly uncomfortable, it is consensus.

**Market defined to fit the slide** — one definition in the deck, another in sales conversations. The tell: the TAM grows between the intro call and the term sheet. → Use the sales definition everywhere, including with investors.

**Group scoring** — the team scores in a room, anchors on the loudest voice, and everything lands at 7 or 8. → Score alone and in writing first. The disagreements are the actual finding.

**Scoring the story instead of the company** — every dimension comes back 8 or above. → Apply the evidence rule mechanically. A score you cannot document drops to 4 with no debate.

**Mistaking early for right** — the answer to "why now" is a trend line rather than a discontinuity. The tell: the why-now slide would have been equally true two years ago. → Name the specific thing that became true in the last 24 months. A technology getting steadily better is not a why-now; a price crossing a threshold or a rule changing is.

**Product as distribution strategy** — "the product sells itself", no named channel, no CAC. → If you cannot see the salespeople, you are the salespeople, and that has a cost and a ceiling.

**Treating the score as a gate to pass** — quietly revising numbers upward until the profile is fundable. → The score has one job: telling you where the next 90 days go. Optimizing it destroys its only use.

**Saying "monopoly" out loud** — internal clarity leaking into external language, which attracts incumbents, regulators, and copycats to a market you have not finished taking. → Own the market quietly. Describe it publicly as small and specific.

## Outputs

- A one-paragraph contrarian claim in the falsifiable format, with the competitor-behavior evidence line
- A named buyer list or bounded population, with the share you intend to hold and by when
- Seven independent score sheets, the gap analysis between scorers, and the minimum
- A durability paragraph naming the compounding mechanism, or an admission there is not one
- One channel with CAC, payback, and dead-zone check
- A raise / do-not-raise recommendation with the single resolving experiment, cost, and deadline

## Pairs with

- [`strategy/value-innovation`](../../strategy/value-innovation/SKILL.md) — when the score fails on breakthrough, this is how you rebuild the offer rather than the pitch
- [`discovery/experiment-design`](../../discovery/experiment-design/SKILL.md) — turns the one unresolved dimension into a cheap, decisive test
- [`strategy/venture-financing`](../../strategy/venture-financing/SKILL.md) — what a fundable profile has to survive on the other side of the table
- [`gtm/chasm-crossing`](../../gtm/chasm-crossing/SKILL.md) — sequencing the beachhead outward once you actually hold it
- [`discovery/venture-design`](../../discovery/venture-design/SKILL.md) — converts a thesis that survives the score into the beachhead, quantified value, and paid minimum product it has to be built out of

## Lineage

Peter Thiel and Blake Masters wrote *Zero to One* out of a Stanford lecture series, arguing that creating something new is categorically different from copying what works, that durable businesses escape competition rather than win it, and framing a set of questions every venture has to answer. The questions are the durable part. This articulation departs from theirs by turning discussion into a scored instrument with an evidence rule, an explicit "do not raise yet" threshold, and a distinction between fixable and unfixable weaknesses — because the underlying questions are now well enough known that founders can answer all of them fluently while learning nothing about their own company.
