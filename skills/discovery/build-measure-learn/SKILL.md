---
name: build-measure-learn
description: >-
  Runs the learning loop at company level: how long a full cycle takes, what an
  MVP is and is not, how to account for progress before revenue exists, and when
  to pivot the venture. Use when a team ships constantly and learns nothing, when
  planning an MVP, when totals look good and nothing works, when deciding whether
  to pivot or persevere, or when the loop has quietly stopped running.
domain: discovery
stage: pre-pmf
lineage: "Eric Ries — *The Lean Startup*; Steve Blank — customer development"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Build, Measure, Learn

> How long one full loop takes — belief to build to evidence to decision — decides whether you find the business before the money ends. Everything else describes how you spent the time.

## The question this answers

- "We ship every two weeks and the numbers do not move. What are we testing?"
- "Our totals are up and to the right. Why does nothing feel like it works?"
- "How do we show this quarter beat the last one, when revenue is near zero?"
- "Is it time to pivot, or are we quitting one quarter early?"

## When to run it

Run this when the company is searching rather than executing and you need to tell progress from motion: before product/market fit, or after it on a new line where the existing numbers do not apply. Run the pivot review on a fixed schedule, so it is a calendar event rather than a crisis meeting: panic favors whatever preserves the current story.

Use [`discovery/experiment-design`](../../discovery/experiment-design/SKILL.md) instead when the question is about one test: which assumption to attack first, which instrument is cheapest, what number would make you stop. That skill governs a single test; this one governs the cadence of many and the venture-level decisions they roll up into.

**Do not run this when** you already know the answer and are building against a signed commitment — executing a known requirement is not learning. Skip it for infrastructure, security, or compliance work, where the standard is done properly rather than learned quickly. And do not use it to defer a decision the evidence already supports; one more cycle is the most respectable form of avoidance.

## The method

### 1. Manage cycle time, not output

Measure the elapsed days from "we wrote down a belief" to "we made a decision because of what we observed." That is one loop. Take the median of the last five. Most teams have never computed it, because the calendar is full of work belonging to no loop.

Decision rule: before fit, a median above six weeks means the batch is too big, not that the market is slow. Cut scope until the cycle fits, even when the smaller test answers less. Two loops that each answer half the question beat one answering all of it a quarter later, because the second uses what the first found.

Choosing the cheapest instrument belongs to `discovery/experiment-design`. What matters here is that the choice shortens the cycle: teams reach for code because code feels like progress and hand-work feels like not having a company, and that inversion stretches the loop.

Treat runway as the number of loops you can still afford, not as months. Cutting costs buys months. Shortening the cycle buys attempts, and attempts are what find the business.

### 2. Apply the four-question test before saying "MVP"

| Question | Experiment | Release with a label |
|---|---|---|
| Outcome predicted in writing beforehand? | Yes, with a number | "We'll see how it goes" |
| A result that would stop the work? | Defined in advance | Nothing changes the roadmap |
| Cheapest form that produces the observation? | Yes, often manual | The version already planned |
| Changes a decision on the calendar? | A named one | It informs, generally |

Four yeses and it is an experiment. Any no and you are shipping a feature, which is fine — say so, hold it to release standards, claim no learning credit. The first two rows come from `discovery/experiment-design`; if they do not exist, the loop has nothing to measure.

This is where the term degraded. A minimum viable product is the fastest route through a full loop, not what you already planned with the polish removed. Half a good product and a bad whole product are different objects: early adopters tolerate narrow scope, not failure at the thing you claim to do. A broken test measures your execution, not their demand.

### 3. Account for progress in cohorts, never in totals

Cumulative counts only rise, so they cannot detect improvement. Group customers by arrival period and compare: does March's cohort activate, retain, and pay better than February's? That is the only comparison that shows whether your changes worked.

A usable metric shows cause and effect, means the same thing to everyone, and can be audited back to individual customers. Fail one and you are steering by a number you do not control.

Run three phases: **baseline** (honest current numbers, however bad), **tune** (do they move toward the model the business requires), **decide** (is the movement enough). Skip the baseline and you spend a year unable to prove you improved anything.

Pick one growth mechanism and one governing metric: retention if growth comes from keeping customers, referral rate if customers bring customers, payback period if you buy growth. Optimizing all three optimizes none.

### 4. Decide pivot or persevere on productivity, not sentiment

A pivot is a structured change to one element — the customer, the problem, how you capture value, how you reach people — holding the rest fixed so it stays testable. Changing everything at once starts a second company with the first one's cap table.

The rule that beats intuition: **is tuning getting more productive or less?** If each round moves the metrics less than the last, you have hit the ceiling of the current hypothesis. If each round still yields, persevere. Corroborating signals: newer cohorts do not outperform older ones; customers call the problem real but keep their workaround; nobody can state which hypothesis this quarter tests.

Name the bar in advance. A call made against a pre-committed number is a decision; one made while staring at the dashboard is a mood. Every pivot carries a new falsifiable prediction, which sends you back through `discovery/experiment-design` before anything is built against it.

### 5. Diagnose why the loop stopped running

Loops rarely stop for intellectual reasons. They stop for structural ones, and the causes are a short list.

| Symptom | Structural cause | Fix |
|---|---|---|
| Builds ship, no result is read | Measure has no owner | Make one person accountable for each loop's number |
| Results are read, nothing changes | Learning feeds no standing decision | Attach the loop to the roadmap or budget meeting |
| Nothing in the plan ever changes | The roadmap is committed a quarter out | Leave capacity uncommitted, or the answer cannot matter |
| Nobody proposes tests any more | Only shipping gets recognized | Report loops completed alongside features shipped |

Decision rule: if two or more rows apply, the problem is the operating system, not the team's judgment. Fix the structure first; more tests inside a broken loop produce more unread results.

## Failure modes

**MVP as a euphemism for bad software** — the team ships the planned product with half the features and none of the quality, then reads the poor reception as market feedback. It was execution feedback. → Run the four-question test before the word MVP enters a document. No threshold and no stopping result means it is a release: name it one and hold it to that quality bar.

**Vanity metrics** — the update leads with cumulative totals, so everything looks like growth. → Report by cohort with a fixed denominator and ban all-time totals from reviews. A metric that has never gone down is not measuring you.

**Batch size creep** — cycles lengthen a week at a time as more gets bundled into each release, and nobody notices because each decision was individually reasonable. Tell: the last loop took twice as long as one a year ago. → Publish median cycle time in the same review as revenue. What is not reported drifts.

**The pivot that is a rebrand, or never comes** — either the deck and vocabulary change while the underlying bet does not, or nothing changes for a year because vanity metrics supplied a sense of progress. → A pivot must carry a new falsifiable prediction; without one it is a redesign. Pre-commit the quarterly bar and review it on schedule: the vision may survive, the strategy is disposable.

## Outputs

1. A **cycle-time reading**: median days per loop over the last five, and the batch-size call that follows.
2. The **four-question classification** — experiment or release — with the build held to that standard.
3. An **innovation accounting sheet**: cohort definition, two or three metrics, the growth mechanism and its number, and the baseline.
4. A **pivot-or-persevere call**: the tuning trend, read against the pre-committed bar, naming the element that changes.
5. A **loop diagnosis** when cycles stall, naming the structural cause and its owner.

## Pairs with

- [`discovery/experiment-design`](../../discovery/experiment-design/SKILL.md) — designs and runs the individual test; this skill decides what the results add up to and how fast they arrive.
- [`discovery/customer-interviews`](../../discovery/customer-interviews/SKILL.md) — generates the assumptions worth testing, and interprets a failure before you blame the market.
- [`discovery/jobs-to-be-done`](../../discovery/jobs-to-be-done/SKILL.md) — supplies the outcome the loop should move, so the metric is the customer's.
- [`discovery/venture-design`](../../discovery/venture-design/SKILL.md) — the assumption list and paid minimum product; this is the cadence that works through both.
- [`gtm/offer-design`](../../gtm/offer-design/SKILL.md) — when the failing assumption is price, not product.

## Lineage

Eric Ries's *The Lean Startup* framed the startup as an institution built to learn under uncertainty and gave it three durable ideas: validated learning as the unit of progress, accounting designed for innovation rather than for stable businesses, and the pivot as an ordinary instrument rather than an admission of failure. Steve Blank supplied the prior insight that the facts are outside the building and founders must go get them.

This version departs in two places. It treats the MVP adversarially, because the term is now used mostly as cover for shipping poor work, and restating it faithfully is no longer useful. And it puts cycle time ahead of experiment quality, because the failure in practice is not that teams run bad tests — that is handled one level down — but that they complete three loops a year and narrate past every result that should have forced a decision.
