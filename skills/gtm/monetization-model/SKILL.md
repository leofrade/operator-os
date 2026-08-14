---
name: monetization-model
description: >-
  Designs the sequence of offers around a first sale so that cash collected in
  the first 30 days exceeds the cost of acquiring and serving the customer.
  Trigger when growth is capped by cash rather than demand, when payback is too
  slow to reinvest, when designing upsells, downsells, or recurring tiers, or
  when someone asks what to sell a customer next and when to sell it.
domain: gtm
stage: scale
lineage: "Alex Hormozi — *$100M Money Models*"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Monetization Model

> Growth is rarely limited by demand. It is limited by how long your cash stays trapped inside a customer you have already won.

## The question this answers

- Acquisition is profitable on paper, so why can we not afford more of it?
- What do I sell next, and when does the customer actually want it?
- Someone says no to the price. What goes in front of them instead of a discount?
- Should recurring revenue be the entry point or the destination?

## When to run it

Run this when a single offer converts reliably and the constraint has moved to cash timing: acquisition is profitable over a customer's life, but payback is slow enough that you can fund only a fraction of the demand you could create.

**Do not run this when** the first offer is not yet stable — sequencing on top of an unproven offer makes failure unattributable. Do not run it when refunds or early cancellations run above roughly one in twenty; that is a product problem, and more monetization just extracts more money from people who will ask for it back. And check first whether a regulator or procurement policy constrains how you may bill.

## The method

### Move 1 — Measure the cash gap, not the margin

Take the last full cohort you acquired. Compute what it cost to win and serve them against what they actually paid within thirty days. That difference is the cash gap, and closing it is the point of everything below.

| First-30-day cash vs. cost to acquire and serve | State | What to do |
|---|---|---|
| Below 1x | Cash-negative growth | Each new customer slows you down; fix before scaling |
| 1x to under 1.5x | Self-funding, barely | Add one expansion offer before increasing spend |
| 1.5x to under 2x | Self-funding with headroom | Increase spend one step at a time, re-measuring each cohort |
| 2x or above | Acquisition is self-financing | Scale acquisition to the limit of delivery capacity |

**Exit criterion:** you can state the ratio as a number. Not an estimate, not a lifetime figure — a thirty-day one.

### Move 2 — Fill four slots, one at a time

A monetization model is four slots around one core sale. Build in order, stabilize each before adding the next. Installing all four at once is the most common way this work fails: you cannot tell which change moved the number.

| Slot | Job | Built when |
|---|---|---|
| Entry | Convert a stranger into a paying customer at acceptable cost | Always first |
| Expansion | Sell the next thing at the moment the first thing creates the need for it | Once entry is stable for a full sales cycle |
| Recovery | Convert a no into a smaller yes without eroding price | Once you have logged the loss reasons |
| Recurring | Make the relationship renew by default | Last, once delivery is repeatable |

Build the entry offer on removing the buyer's first risk, not on a discount. Discounting to acquire trains a population that buys on price and renegotiates at renewal. Structures that put your money at risk against a result — deferred payment, outcome-linked rebate, first-milestone guarantee — acquire the same volume without setting a lower reference price.

### Move 3 — Time expansion to the problem your first sale created

Every solved problem exposes the next one. The expansion offer is not a bigger version of what they bought; it answers the problem their purchase just made visible. Sell it at the moment of visibility, which is the first delivered result, not the signature.

**Threshold:** below one in five taking it, the timing is wrong or the offer is disconnected from the revealed problem. Above one in two, you under-scoped the entry offer and should consider merging them.

Anchoring works here if used honestly: present the larger option first and be willing to sell it. A premium option you have no intention of delivering fails the first time someone says yes.

### Move 4 — Recover a no by changing what they get or when they pay, never the price for the same thing

A buyer who declines has declined this configuration, not every configuration. Two honest levers exist.

Change the payment shape: installments, a deposit against a later balance, annual prepay against a discount that reflects the cash and churn benefit you actually receive. Or change the scope: less quantity, lower service level, work shifted from you doing it to you supervising it. Name the reduced version so it reads as a different product, not a concession.

**The rule that protects you:** never sell the same thing to a second buyer for less than the first paid. Buyers in a vertical talk and procurement teams benchmark; one leaked disparity poisons every renewal in the segment. Reduce the deliverable alongside the number.

**Read temperature before conceding.** Ask how badly they want it, one to ten. Below eight, price is not the problem and another concession will not close it — return to the value case. At eight or above, a payment-structure change usually closes.

### Move 5 — Make recurring the destination, not the door

Subscriptions produce excellent lifetime economics and terrible early cash. A pure subscription entry collects one month of revenue against a full month's acquisition cost, which is why these businesses are so often capital-hungry.

Two structural levers beat pricing cleverness. Cadence: annual and quarterly commitments cut churn sharply against monthly, because the renewal decision is made less often. Commitment: an activation fee waived in exchange for a term makes leaving cost more than staying, without raising the headline rate. Put a retention incentive at the month where cancellations cluster, and give cancellation a defined cost equal to the benefit already received.

**B2B translation.** The mechanics change shape, and shape matters more than tactic. Expansion becomes land-and-expand across seats, sites, or business units — a procurement event, so the trigger is the customer's budget calendar as much as their moment of need. Recovery is scope reduction with the expansion path written into the contract: pilot pricing that steps up on a defined date, signed at the start rather than renegotiated later. Recurring is contract term and auto-renewal language, which is where retention is actually decided. Annual prepay is the most reliable cash-gap fix in B2B and usually costs a smaller discount than founders assume, because the buyer's incentive is budget consumption rather than savings. Consumer payment-plan gymnastics rarely survive procurement; multi-year terms with annual uplift do.

## Failure modes

**Downsell as price erosion** — the team learns any no converts with a discount, and within two quarters list price is fiction. The tell is average selling price falling while win rate holds flat. → Require a scope change with every price change, and manage the discounted-to-full-price ratio as a tracked metric.

**Upsell as churn accelerator** — expansion is pushed before the first result lands, the customer feels sold rather than served, and both offers get cancelled. The tell is expansion take-up correlating with higher first-year cancellation. → Gate expansion behind a delivered outcome as a system rule, not a rep's judgment.

**Cash engineering over a leaky bucket** — payment structures pull revenue forward and mask deteriorating retention. The tell is cash improving while each cohort's retention curve flattens lower. → Cash timing is a growth lever, not a repair. Check retention before and after any structural change and stop if the curve moves the wrong way.

**Refunds treated as cost of doing business** — the rate is accepted and never investigated. The tell is refund reasons clustering on one promise made in the sales conversation. → Above roughly five percent, stop selling and fix the delivery or the promise. Refund reasons are the highest-fidelity product feedback you get for free.

**Everything at once** — four offers launch in a quarter, revenue moves, nobody can say which one did it. The tell is a change log with no matching measurement window. → One change per cycle, measured over at least one sales cycle.

**Anchor you cannot deliver** — a premium tier exists to make the middle look reasonable, and then somebody buys it. The tell is panic in delivery when a top-tier deal closes. → Anchor only with something you would happily deliver at that price today.

## Outputs

- The thirty-day cash ratio for the latest cohort, with the arithmetic shown.
- A four-slot map: what fills each slot today, what is missing, the build order.
- One expansion offer with its trigger event and take-up threshold.
- A recovery ladder: payment-shape options and scope-reduction options, named.
- A recurring structure: cadence, term, commitment mechanism, cancellation terms.
- A single-change measurement plan with the window and the deciding metric.

## Pairs with

- [`gtm/offer-design`](../../gtm/offer-design/SKILL.md) — builds the core offer this sequence is arranged around.
- [`gtm/pricing-power`](../../gtm/pricing-power/SKILL.md) — sets the price levels these structures move money between.
- [`gtm/lead-engine`](../../gtm/lead-engine/SKILL.md) — consumes the cash this model frees, and sets the acquisition cost side of the ratio.
- [`strategy/business-model-design`](../../strategy/business-model-design/SKILL.md) — for when the sequence keeps failing because the underlying model is wrong.

## Lineage

The four-slot structure and the thirty-day cash discipline come from Alex Hormozi's *$100M Money Models*, whose most useful contribution is reframing growth as a cash-velocity problem rather than a demand problem, and insisting that a no rejects one configuration rather than the relationship.

This articulation departs in scope and tone. It drops the individual offer mechanics, which read as a catalog and age quickly, in favor of the four slots and the sequencing rule. It is also more conservative about consumer-style payment tactics in enterprise contexts, where price consistency across a buying network is worth more than any single recovered deal.
