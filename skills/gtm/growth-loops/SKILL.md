---
name: growth-loops
description: >-
  Separates real compounding loops from funnels wearing loop vocabulary, using
  four tests — reinvestment, compounding, independence, and cycle time — and
  then sizes what a sub-1 loop is actually worth. Trigger when someone proposes
  a referral program, when a team claims viral or organic growth, when
  acquisition costs rise as spend scales, when designing an invite or
  user-generated-content mechanic, or when deciding whether growth should come
  from a loop or a channel.
domain: gtm
stage: scale
lineage: "Sean Ellis & Morgan Brown — *Hacking Growth*; Gabriel Weinberg & Justin Mares — *Traction*; Andrew Chen — the law of shitty clickthroughs; Jonah Berger — *Contagious*"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Growth Loops

> Most things called loops are funnels with a share button. The difference is whether output becomes input without a proportional increase in spend, and it is testable in two weeks.

## The question this answers

- Is our growth compounding, or are we buying it and calling it organic?
- We want a referral program. Will it do anything, and how would we know?
- Cost per customer keeps rising as we scale. Fixable or structural?
- The loop exists but growth is slow. Which arrow do I fix first?

## When to run it

Run this when someone proposes a viral mechanic and you must decide whether to fund it. Run it when acquisition cost rises faster than volume, meaning the channel is saturating and you need growth that does not price against itself, or when a team reports organic growth and you want to know whether it survives a spend freeze.

**Do not run this when** retention is below your category's floor; a loop on a leaking bucket accelerates the leak. **Do not run this when** the buyer is a small population of high-value accounts — a few hundred targets produce a sales motion and an expansion motion, not compounding mechanics, and calling that a loop distorts expectations. **Do not run this when** you need revenue in 60 days; loops pay out over cycle times, usually longer than the asker's runway.

## The method

### Move 1 — Draw the funnel and the loop separately, on the same page

A funnel is linear with an external input: spend goes in one end, customers come out the other, and the output does nothing for the input. A loop is a closed circuit where the output of one cycle becomes the input of the next.

```
FUNNEL:   spend → impressions → clicks → signups → customers → (end)
LOOP:     new user → produces an artifact/invite/signal → that reaches
          non-users → some convert → new user
```

Write your claimed loop as an arrow chain and put a measured number on every arrow — from your data, not an estimate. A team that cannot fill in every arrow has an ambition, not a loop.

### Move 2 — Run the four tests

| Test | Pass condition | Failure verdict |
|---|---|---|
| Reinvestment | A new user's ordinary use of the product creates something that reaches a non-user | If reaching non-users needs a new marketing action, it is a channel |
| Compounding | Marginal cost per acquired user declines as volume rises | Flat or rising unit cost means the mechanic scales linearly — a channel |
| Independence | Freeze paid spend; volume degrades gradually over a full cycle | Volume collapses within one cycle — the loop was a spend artifact |
| Cycle time | Measured in days, and short enough to matter at your planning horizon | Unmeasured cycle time means the loop is undated and unbudgetable |

Any failed test means the mechanic is a channel. Not a criticism — channels build companies. It is a labeling correction with budget consequences: channels are optimized on cost per acquisition and payback, loops on cycle time and conversion per arrow, and the wrong optimization wastes quarters.

The independence test is decisive and almost nobody runs it, because it costs two weeks of volume. Run it anyway. A two-week pause costs less than four quarters of believing you have an engine.

### Move 3 — Measure K honestly, then size what it is worth

K is new users produced per existing user per cycle. Measure it at the far end — activated accounts, not invitations sent. Teams measuring sends report a healthy K while acquiring nobody.

```
K = (invitations or exposures per user) × (conversion to activated user)

Cumulative users from a seed of N:   N / (1 − K),  for K < 1
```

That formula is the honest framing of most loops, and it changes the decision:

| K | What it means | Correct use |
|---|---|---|
| < 0.2 | Rounding error | Do not fund a program around it |
| 0.2 - 0.5 | A 1.25x to 2x multiplier on paid acquisition | Reframe as CAC reduction — a discount on the channel, not an engine |
| 0.5 - 0.9 | Two to ten times amplification | Real leverage; protect it and shorten cycle time |
| ≥ 1.0 | Self-sustaining exponential | Rare, usually temporary; decays as the network saturates |

The reframe matters operationally. A loop at K = 0.4 does not free you from paid acquisition; it multiplies each paid cohort by 1 / (1 − 0.4) = 1.67x, so every acquired customer costs 60% of what you paid before — a 40% reduction. Framed that way it competes for budget against pricing and channel work on honest terms, and stops being sold as an escape from paid spend.

### Move 4 — Find the weakest arrow, fix one per cycle

Decompose K into arrows and attack the lowest-yield one. Invite copy routinely produces multiples, because most of it sells the sender's benefit rather than the recipient's payoff. Move the reward to the receiving side, or tie it to a milestone the recipient must reach; both volume and cohort quality change.

Rule: one arrow per cycle, measured against the previous cycle. Three at once produces a number you cannot attribute.

### Move 5 — Check the referred cohort's quality before scaling

Compare retention and expansion of loop-acquired users against organic ones. If referred users retain materially worse, the incentive is buying reward-seekers, and scaling degrades the business while the acquisition chart improves. Fix the incentive before the volume.

## Loop types and their real constraints

| Type | Mechanic | The constraint people ignore |
|---|---|---|
| Collaboration | Using the product requires bringing in a non-user | Needs a genuinely multiplayer workflow; forcing it degrades single-player value |
| Content or index | Usage produces indexable public artifacts that attract search demand | Compounds only if marginal cost falls; if each artifact needs a human, it is a content factory |
| Incentivized referral | Reward for bringing someone in | Cohort quality; the incentive selects for the wrong user unless it is tied to a milestone |
| Expansion | Successful accounts grow seats and refer peers | Slowest cycle time and the most durable; requires customer success staffing to turn |
| Paid reinvestment | Revenue funds acquisition of the next customer | Bounded by payback period, not network effects; legitimate, but arithmetic, not virality |

## Failure modes

**Funnel in loop clothing** — paid acquisition with a referral widget attached, reported to the board as an organic engine. The tell: the independence test collapses volume within one cycle, or growth tracks spend with a lag. → Relabel it a channel and optimize CAC payback. That is not a defeat; it stops the company underfunding acquisition on the theory that the loop will take over.

**K measured at the wrong end** — invitations sent per user is reported as K, producing a confident 1.4 while activated accounts stay flat. The tell: the dashboard tracks sends, opens, or clicks. → Count only activated accounts attributable to the loop. Everything upstream is a diagnostic, never the headline.

**Loop on a leaking bucket** — the mechanic works, users arrive, and the cohort curve still hits the floor by week four. The tell: total actives flat while acquisition climbs. → Stop loop work; retention is a prerequisite, not a parallel workstream.

**Incentive that buys the wrong user** — the referred cohort retains and converts worse than organic, but the acquisition number looks great, so the program scales and blended metrics rot. The tell: any meaningful retention gap between referred and organic. → Move the reward to the recipient, or gate it on a usage milestone rather than signup.

**Cycle-time blindness** — a loop with a real K of 0.6 and a 90-day cycle is funded as if it changes this quarter, and the team declares failure at week eight. The tell: nobody can state the cycle time in days. → Measure cycle time first; it sets the review cadence and the honest payback horizon.

**Saturation ignored** — a mechanic that worked at 10,000 users decays at 200,000 because the network is exhausted and the medium has learned to ignore it. The tell: K declining quarter over quarter with no change to the mechanic. → Track K as a time series, not a constant. Plan the next loop before the current one drops below 0.3.

## Outputs

- Loop diagram as an arrow chain with a measured value on every arrow
- Four-test scorecard with an explicit channel-or-loop verdict
- K on activated accounts, with the amplification multiplier and its budget reading
- Measured cycle time in days and the review cadence it implies
- Cohort quality comparison: loop-acquired versus organic, retention and expansion
- Arrow-level experiment list, one per cycle, each with a stop rule
- If the verdict is channel: the CAC payback analysis that replaces the loop plan

## Pairs with

- [`gtm/gtm-measurement`](../../gtm/gtm-measurement/SKILL.md) — none of these tests run without cohort-level source capture in place first
- [`gtm/monetization-model`](../../gtm/monetization-model/SKILL.md) — a paid reinvestment loop is bounded by payback period, a pricing decision
- [`gtm/audience-engine`](../../gtm/audience-engine/SKILL.md) — for the content and index loop type, where the constraint is marginal production cost
- [`discovery/experiment-design`](../../discovery/experiment-design/SKILL.md) — arrow-level experiments need stop rules or you read noise as lift
- [`discovery/engagement-ethics`](../../discovery/engagement-ethics/SKILL.md) — loops are where extractive retention mechanics get built; audit the mechanism before you compound it

## Lineage

The growth-experiment discipline and the loop framing come from Sean Ellis and Morgan Brown's *Hacking Growth*; the channel taxonomy and the rule of concentrating on one working channel from Gabriel Weinberg and Justin Mares in *Traction*; the observation that every acquisition mechanic decays as its medium saturates is Andrew Chen's; the social-transmission factors behind why anything gets shared are Jonah Berger's, in *Contagious*. Where this departs: the growth literature treats loops aspirationally and rarely supplies a falsification test, so teams adopt the vocabulary without the mechanics. The four tests, especially the independence test that requires actually freezing spend, exist to force the classification — as does the reframe of a sub-1 loop as a CAC discount rather than an engine, which is the least popular and most useful sentence here.
