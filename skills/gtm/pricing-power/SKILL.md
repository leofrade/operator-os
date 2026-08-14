---
name: pricing-power
description: >-
  Sets price from evidence of what buyers will pay rather than from competitor
  averages or cost-plus, by choosing the billing unit first, gathering
  willingness-to-pay signal at a method appropriate to sample size, and
  packaging into tiers with a single upgrade gate. Trigger when setting or
  revising price, designing tiers or a value metric, running price research or
  experiments, or when deals stall on the number.
domain: gtm
stage: any
lineage: "Madhavan Ramanujam & Georg Tacke — *Monetizing Innovation*; Peter van Westendorp — Price Sensitivity Meter; André Gabor & Clive Granger — price-response research"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Pricing Power

> Price is the first product decision, not the last, and every month you defer it you build something whose economics nobody has tested.

## The question this answers

- What number goes on this, and what evidence supports it rather than a feeling?
- What do we charge for — seats, usage, outcomes — and what does that do to adoption?
- Are we too cheap? What would tell us, other than customers not complaining?
- How do we raise price without a churn event?

## When to run it

Run before launch, at any pricing revision, when a value metric changes, and on a quarterly cadence whether or not anyone asked.

**Do not run quantitative price research when** the sample is small. Below roughly fifty in-segment respondents, a survey produces the appearance of rigor without the substance, and those numbers get quoted in decisions for years; use structured interviews instead. Do not run this at all when you cannot state the value you create in units the buyer already tracks — that is a positioning problem, and research will only measure the confusion.

## The method

### Move 1 — Choose the billing unit before the number

The unit shapes behavior more than the amount. A unit that grows with the customer's success makes expansion automatic. A unit that grows with their cost makes them ration your product.

| Unit | Fits | Breaks when |
|---|---|---|
| Flat fee | Simple products, early stage | Value varies widely across accounts |
| Per seat | Tools where every added user gains | Buyers limit rollout to control spend |
| Per usage | Infrastructure, APIs, variable consumption | Revenue is unforecastable; buyers fear the bill |
| Per outcome | High-value services with a countable result | Attribution is contestable or costly to measure |

Four tests: it correlates with value received; both sides can audit it; it grows as the account grows; the customer never has to suppress adoption to control it. When true value is unmeasurable, pick a proxy that moves with it and say so plainly.

**Exit criterion:** you can defend why a customer paying twice as much receives roughly twice the value.

### Move 2 — Gather willingness-to-pay evidence at a method your sample supports

Match method to sample size. Running a method your data cannot support is worse than guessing, because it launders the guess as a finding.

| Sample available | Method | What it gives you |
|---|---|---|
| 5–30 buyer conversations | Structured WTP interviews | Direction, budget anchors, value language |
| 150+ in-segment respondents | Price sensitivity survey | An acceptable range, floor and ceiling |
| 300+ respondents | Price-response testing across points | A demand curve, a revenue-maximizing point |
| Any | Presale against a real invoice | Truth; the rest forecasts this |

In interviews, anchor on what they spend today on the alternative, including the human-labor version. Ask what price is an immediate yes and what price forces internal approval — that gap is your negotiating room and often the shape of your tiering. Then ask whether they would buy at double. Hesitation is data; an instant confident number means you are underpriced.

Discount stated intent hard: people overstate willingness to pay, commonly by a third to a half. The only unbiased instrument is an invoice, which is why a presale to a handful beats a survey of hundreds.

### Move 3 — Price from value created, then sanity-check against alternatives

Estimate the annual value created for a typical account — cost removed, revenue enabled, risk priced — and capture a defensible share. In most categories that share sits between five and thirty percent; below five you cannot fund service, above thirty the buyer builds it themselves.

Then check the number against the alternatives the buyer actually considers, which are rarely your competitors: a spreadsheet, an internal process, a person hired to do it. Where nobody publishes prices, that comparison is the entire benchmark. Cost sets your floor and nothing more; competitor pricing is evidence about their strategy, not your value.

### Move 4 — Package into tiers with exactly one gate

Three tiers, built so the middle one is where the majority lands: an entry tier that captures price-sensitive buyers and anchors the floor, a main tier carrying most revenue, and a high tier that anchors the ceiling.

Gate on one dimension — volume, collaboration, integrations, compliance, or support level — and let it drive every upgrade. Multi-dimensional gating produces a comparison table nobody can read and a sales conversation about features rather than outcomes.

**Threshold:** if fewer than half of new customers land in the middle tier, the gate is in the wrong place or the entry tier is too generous.

### Move 5 — Test safely and review on a cadence

Never charge different prices to buyers who talk to each other; in a tight vertical, they all talk. Safe instruments: cohort pricing with existing customers grandfathered, new-visitor page tests, and quoting different points across consecutive sales conversations — twenty per point minimum before reading anything into it.

Review quarterly on four things: conversion by tier, retention by tier, losses citing price versus losses citing fit, and delivered value now versus when the price was set. Raise price when retention is strong, deals close without negotiation, and delivered value has grown — a combination that appears well before anyone internally feels ready to act on it.

Announce increases with a long runway, honor existing terms for a defined period, and pair the increase with something added. Customers rarely churn over a price rise; they churn over being surprised.

**B2B translation.** Published pricing research assumes consumer-scale samples that enterprise sales never produces. Substitute deal-level evidence: quote-to-close by price point, discount depth by segment, loss reasons your reps record. Watch pocket price rather than list — the number after discounts, terms, and concessions — because that is what funds the business and where erosion hides. Buyer and user also differ in sensitivity: the user compares you to tools, the budget holder compares you to headcount, and the second comparison supports a far higher number. Procurement benchmarks you against every comparable it can find, so publish a defensible logic rather than a number you cannot explain. And segment-wide price consistency beats optimizing a single deal: one leaked discount resets the anchor for every renewal in that vertical.

## Failure modes

**Survey theater** — thirty respondents produce a precise-looking optimal price that gets quoted for two years. The tell is a pricing decision citing a percentage with no sample size beside it. → State sample size next to every number; treat anything under fifty as directional.

**Competitor-anchored pricing** — the team averages three competitors and shaves ten percent. The tell is that nobody can explain the price except by reference to someone else's. → Price from value created; use competitors only to check you are inside what the market will consider.

**A unit that punishes adoption** — per-seat pricing on a product whose value comes from broad rollout, so buyers under-deploy on purpose. The tell is flat seat counts with rising usage per seat. → Change the metric at the next contract cycle; no discount fixes a misaligned unit.

**Tier proliferation** — five tiers and a matrix of add-ons, because every lost deal added an exception. The tell is a pricing page that needs a call to interpret. → Collapse to three, gate on one dimension, move real exceptions into a negotiated tier.

**The price nobody has raised** — unchanged for three years while the product doubled in scope. The tell is deals closing at full price with no negotiation, which founders read as success rather than as money left behind. → Test a higher point with the next cohort and grandfather everyone existing.

**Discount instead of qualification** — price gets cut to close deals that were never good customers. The tell is discounted accounts carrying higher support load and lower retention. → Route price objections back to qualification before conceding; a buyer who cannot afford the value is usually the wrong buyer.

## Outputs

- A billing unit with its four-test justification and the rejected alternatives.
- WTP evidence from a method matched to sample size, with the sample size stated.
- A value-created estimate and capture rate, arithmetic shown.
- Tier definitions with one named upgrade gate and the expected distribution.
- A test plan: instrument, duration, minimum volume, rollback criteria.
- A quarterly review template and the grandfathering policy for increases.

## Pairs with

- [`gtm/offer-design`](../../gtm/offer-design/SKILL.md) — builds the package this price attaches to; run first if the value gap is thin.
- [`gtm/freemium-economics`](../../gtm/freemium-economics/SKILL.md) — whether a free tier belongs in the structure at all.
- [`gtm/monetization-model`](../../gtm/monetization-model/SKILL.md) — sequences what gets sold once this price is accepted.
- [`discovery/customer-interviews`](../../discovery/customer-interviews/SKILL.md) — source of qualitative WTP evidence at small samples.
- [`revenue/channel-strategy`](../../revenue/channel-strategy/SKILL.md) — partner margin is a permanent subtraction from this price; it sets the floor before you commit to a number.

## Lineage

The value-first discipline — decide what to charge for and validate willingness to pay before building — comes from Madhavan Ramanujam and Georg Tacke's *Monetizing Innovation*, with its argument that pricing is a product design input rather than a launch-week decision. The survey instrument descends from Peter van Westendorp's 1976 price sensitivity work, and the price-response testing from André Gabor and Clive Granger's research on price as a quality signal. The value-metric and tiering vocabulary reflects a decade of practitioner writing on subscription and usage-based pricing.

This articulation departs from that tradition by refusing to run quantitative methods below their valid sample sizes, and by weighting a small presale above a large survey. In most companies the honest answer to "what will they pay" arrives from twelve invoices faster and more reliably than from three hundred survey responses.
