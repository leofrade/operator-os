---
name: experiment-design
description: >-
  Turns a business assumption into a test that can actually fail, with the kill
  number written down before the test runs. Use when validating an idea before
  building, choosing between a landing page and a concierge test, deciding how
  much evidence a decision requires, setting persevere/revise/kill criteria,
  auditing a team whose experiments always succeed, or planning a discovery sprint.
domain: discovery
stage: pre-pmf
lineage: "David Bland & Alexander Osterwalder — *Testing Business Ideas*"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Experiment Design

> An experiment you cannot lose is not an experiment. It is a press release with a sample size.

## The question this answers

- What is the one thing that, if false, makes this whole idea worthless?
- What is the cheapest test that would actually change my mind?
- How much evidence do I need before I am allowed to spend engineering months?
- The test came back positive — is that a signal, or did I design it to come back positive?

## When to run it

Run it when you are about to commit capital or calendar time on the strength of a
belief nobody has checked: a new product line, a new segment, a pricing change, a
build estimated in months. Run it whenever someone says "obviously customers want
this."

Use [`discovery/build-measure-learn`](../../discovery/build-measure-learn/SKILL.md)
instead when the unit is not one test but the cadence: how long a full cycle takes,
how to account for progress before revenue exists, and whether the venture itself
should pivot. This skill designs the test; that one runs the loop the tests live
inside, before and after code exists.

**Do not run this when** the answer is already available for free — a competitor
has proven the market, your support queue holds the answer, or the build is two days
and the test would take two weeks. Below a certain cost of being wrong, ship it and
watch. Skip it too for regulated or safety-critical decisions, where the correct
instrument is expert review, not a field test.

## The method

### 1. Convert the plan into claims that can be false

Extract statements in the form: *We believe [specific, falsifiable claim about a
named segment].* Vague claims are unfalsifiable and useless. "SMBs care about
compliance" is not a claim. "Operations managers at 50–200 person logistics firms
will pay a monthly fee to avoid manual document filing" is.

Sort them into three risk classes, and check you have claims in each:

| Risk class | The question | Where teams under-test |
|---|---|---|
| Desirability | Does anyone want this enough to change behavior? | Rarely; this is the fun one |
| Viability | Does the money work at achievable prices and costs? | Almost always under-tested |
| Feasibility | Can we build and operate it at that cost? | Over-tested by technical founders |

### 2. Rank by consequence, not by curiosity

For each claim, score two things 1–5: **how load-bearing** it is (if false, does
the idea die or just get worse?) and **how little evidence** you have from the
field, as opposed to from a deck. Multiply. Test the top item first. Anything
scoring 5 and 5 is the only work that matters this week.

### 3. Pre-register the number that would make you stop

Before the test exists, write four lines and get them agreed by whoever holds the
budget:

```
We believe        [claim]
We will test by   [experiment, subject count, timebox]
We will measure   [one primary metric, defined precisely]
We are wrong if   [number below which we stop / change direction]
```

The fourth line is the entire discipline. If you cannot state a number that would
make you abandon the idea, you are not testing. Timestamp it, and do not touch it
once data starts arriving.

### 4. Match evidence strength to the size of the decision

Evidence gets stronger along four axes. Weak evidence is cheap and fine for
direction; strong evidence is required before you spend real money.

| Axis | Weak | Strong |
|---|---|---|
| What you observe | What people say | What people did |
| Setting | Interview, survey, demo | Their real workflow, their real week |
| Cost to the subject | An email address | Money, a signature, reputation |
| Reversibility for them | Trivial to walk away | Painful to walk away |

The rule: **the strength of evidence must exceed the cost of being wrong.**
A landing page can justify another two weeks of discovery. It cannot justify a
six-month build. Before a build that size you want money changing hands or a signed
commitment from a named buyer — a pre-sale, a paid pilot, a letter of intent with a
date in it. Before hiring a sales team you want that repeated with a second buyer
you did not personally charm.

Escalate fidelity as uncertainty drops. A workable ladder for a B2B idea:
problem interviews → a one-page offer put in front of buyers → manual concierge
delivery for three customers → a paid pilot → a single-feature build. Each rung
costs roughly ten times the last, and skipping rungs gets paid back in build.

Choose the rung by what it lets you observe, not by what the team enjoys building.
A demand test answers whether anyone wants it, in days; concierge delivery answers
whether the outcome is worth anything, and teaches you the workflow you would
otherwise have guessed at. Write software only after manual delivery has proven the
value and has itself become the bottleneck. Manual delivery expires: doing it by
hand a quarter after the value is proven means you run a services business.

### 5. Run two tests per load-bearing claim, using different mechanisms

One experiment produces an anecdote with a spreadsheet attached. Two that disagree
beat one that confirms, because the disagreement tells you which instrument was
lying. Pair a stated-preference test with a revealed-preference one on the same
claim: a survey plus an ad campaign, an interview plus a mock sale. When they
diverge, believe the one where someone gave something up.

### 6. Decide in a fixed meeting, in writing

At the end of the timebox, one hour, same agenda: what we believed, what we
observed (numbers, not impressions), what we now think, what we do next. Three
permitted outcomes — **persevere** (the next claim, or this one at higher
fidelity), **revise** (the claim was wrong in a way the next test can correct),
**kill** (the claim is dead, and everything downstream of it is now unfunded). A
meeting that cannot produce "kill" is a status update.

Read the result against the number you registered, not the story that grew around
it while the test ran. One question closes the meeting: would we have called this a
failure if we had not already spent the money. Keep the call scoped to the claim.
When several load-bearing claims die in a row, the question becomes whether the
venture should change shape — and that belongs to
`discovery/build-measure-learn`, which reads the trend across cycles.

### 7. Set the ethical perimeter before you go live

Any test touching real customers needs, in writing beforehand: which segment is
exposed, how many people, start and end dates, what brand appears on it, maximum
financial exposure, and how to switch it off. Simulated purchases terminate before
money is captured, or refund the same day. Selling what you cannot deliver is not
an experiment.

## Failure modes

**Confirmation testing** — the sample is your network, the question is leading, the
metric is chosen after the fact. Tell: your last six experiments all succeeded. → A
healthy discovery program kills roughly half of what it tests. Give someone the job
of arguing the null result, and recruit strangers.

**Goalpost drift** — the result comes in at 3% against a target of 10%, and the
team explains why 3% is encouraging given the traffic quality. Tell: the success
criterion is being discussed after the data exists. → Pre-registration, timestamped,
read out loud at the start of the decision meeting.

**Fidelity mismatch, both directions** — a signup form used to justify a platform
rebuild, or an MVP built to answer a question five calls would have settled. Tell:
the test costs are out of proportion to the decision. → Ask what this test unblocks
and what being wrong would cost. Size the instrument to that number.

**Email addresses as demand** — 400 waitlist signups become a slide claiming
validated demand. Tell: nobody has been asked for anything that costs them
something. → An email address measures curiosity. Charge something, even a deposit,
or route the traffic to a real checkout that fails gracefully.

**The zombie experiment** — a test that has been "running" for two months with no
end condition. Tell: nobody can say when it finishes or what would end it. → Every
test gets a stop date at creation. A timebox that expires without a conclusive
result is itself a result: the effect is too small to detect cheaply, which usually
means too small to matter.

## Outputs

- A ranked claim register: claim, risk class, load-bearing score, evidence score,
  status
- A pre-registered test card per claim, with the failure threshold and the timebox
- An evidence log: what was observed, sample size, strength on the four axes
- A decision memo per claim ending in persevere / revise / kill, with an owner
- An ethics perimeter note for customer-facing tests: exposure, duration, brand,
  kill switch
- The untested claims currently blocking the next funding or build decision

## Pairs with

- [`discovery/customer-interviews`](../../discovery/customer-interviews/SKILL.md) — the low-fidelity end of the
  ladder, and where most bad evidence is generated
- [`discovery/build-measure-learn`](../../discovery/build-measure-learn/SKILL.md) — the loop these tests sit
  inside: cycle time, cohort accounting, and the venture-level pivot call
- [`strategy/business-model-design`](../../strategy/business-model-design/SKILL.md) — the model supplies the claims;
  this skill decides which one gets tested first
- [`gtm/gtm-measurement`](../../gtm/gtm-measurement/SKILL.md) — for turning validated claims into
  instrumented funnel metrics after launch

## Lineage

Treating a business plan as a stack of testable hypotheses runs from Steve Blank's
customer development through Eric Ries, and was made operational as a working
library by David Bland and Alexander Osterwalder in *Testing Business Ideas*, which
contributed the evidence-strength axes and the insistence on sequencing cheap tests
before expensive ones. Where this departs: the published catalog invites teams to
browse experiments like a menu, and most do, ending up with an activity plan rather
than a decision plan. The pre-registered failure threshold is the only
non-negotiable part — the choice of experiment matters far less than writing down,
in advance, the number at which you walk away.
