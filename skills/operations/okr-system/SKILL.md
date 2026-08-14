---
name: okr-system
description: >-
  Installs a quarterly goal system that survives contact with a real company:
  three objectives, key results written as outcomes, a hard firewall between
  scores and pay, and a weekly check-in that moves confidence rather than
  percentages. Use when setting quarterly goals, rewriting key results, running
  a planning offsite, diagnosing why last quarter's OKRs were ignored, scoring a
  cycle, or deciding whether to adopt OKRs at all.
domain: operations
stage: scale
lineage: "Andy Grove — *High Output Management*; John Doerr — *Measure What Matters*"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# OKR System

> OKRs do not fail because people write them badly. They fail because someone attached them to money, and the organization quietly started aiming low.

## The question this answers

- What are the three things this quarter is actually for, and what are we deliberately not doing?
- Is this a key result or a to-do list item wearing a number?
- Why did we hit 100% of our goals and grow slower than last year?
- Should we adopt OKRs at all, or do we need something cheaper?

## When to run it

Run it when the company is large enough that people can spend a full week on
work no one else knows about — roughly 15 people and up, or earlier if you have
more than one team with its own backlog. Run it at the start of a planning
cycle, and again mid-cycle when you suspect the goals have gone stale.

**Do not run this when** you are pre-product-market-fit and the honest goal for
the quarter is "find out what to build." A ten-person team chasing one insight
does not need a goal-setting protocol; it needs a shorter feedback loop. Also do
not run it when the company is in a genuine crisis — a cash-out date inside two
quarters, a security breach, a founder split. Crises run on a single number and a
daily standup.

## The method

### 1. Cut to three objectives, and name what you dropped

Five is the number people quote. Three is the number that changes behavior. The
output of this move is not the three; it is the written list of what you
considered and rejected. If leadership cannot produce that list, they did not
prioritize — they enumerated.

Decision rule: if a team cannot state the quarter's objectives from memory, you
have too many. Cut until they can.

### 2. Rewrite every key result until it passes the inversion test

Most key results are outputs — things the team will do — disguised with a
number. The test that catches this in ten seconds:

```
INVERSION TEST
Ask: "Could we hit this number exactly, on time, and have the
      business be no better off?"

  YES  → it is an output. Rewrite it.
  NO   → it is a key result. Keep it.

Examples:
  "Ship the self-serve onboarding flow"        → YES. Output.
  "Launch 12 marketing campaigns"              → YES. Output.
  "Cut time-to-first-value from 9 days to 2"   → NO.  Keep.
  "Raise trial-to-paid from 11% to 18%"        → NO.  Keep.
```

Second gate: sufficiency. If every key result under an objective is fully
achieved, is the objective necessarily achieved? If you can imagine hitting all
of them and still failing, a key result is missing. Fix the set, not the wording.

Ship dates belong in the plan, not in the key results. A launch is how you
intend to move the number; it is not the number.

### 3. Classify committed vs. aspirational before the quarter starts, in public

Committed means 1.0 is the expectation and missing it triggers a written
explanation. Aspirational means 0.7 is a good outcome and 1.0 means the target
was too soft. Classifying at scoring time is retroactive excuse-making. Publish
the split on day one.

Rule of thumb: at most one aspirational objective per team per cycle. More than
that and nothing is really committed.

### 4. Build the compensation firewall and say it out loud

This is the single move that determines whether the system works. Scores feed
performance conversations as one input among several. Scores do not feed a bonus
formula. The moment a number determines pay, every competent person negotiates
the number downward before the quarter starts, and you have replaced ambition
with a procurement exercise.

Tell: last cycle's average score was above 0.9 across every team. That is not
excellence. That is sandbagging with good manners.

### 5. Run a weekly check-in on confidence, not on percent complete

Percent complete is a lagging, gameable number that always reads 60% until it
reads 20%. Instead, each owner reports a confidence level that the key result
lands by end of cycle, and whether it moved since last week.

| Signal | Reading | Action |
|---|---|---|
| Confidence flat and high | On track | Nothing. Do not discuss it. |
| Confidence dropped this week | Something was learned | Spend the meeting here |
| Confidence flat and low for 3 weeks | Stalled, and everyone knows | Re-plan or kill it |
| Confidence rose without new evidence | Wishful reporting | Ask what changed; if nothing did, revert |

Meeting rule: only discuss key results whose confidence moved. A status meeting
that walks every item in order is a status report read aloud.

### 6. Score, then hold one honest hour

Score each key result 0.0–1.0. Average to the objective. Then run the hour that
creates the compounding: what did we learn that we did not know twelve weeks ago,
which goal was wrong rather than missed, and what would have to be true for next
quarter's targets to be right? Write it down. A cycle without this hour is twelve
weeks of activity converted into zero institutional memory.

Kill rule: an objective carried unchanged into a third cycle is either a strategy
mislabeled as a quarterly goal, or unowned.

## Failure modes

**Compensation coupling** — scores are an input to the bonus formula. Tell:
targets get easier every cycle while the narrative gets more confident, and
scores cluster suspiciously between 0.9 and 1.0. → Sever the link explicitly and
announce it. Then deliberately celebrate a 0.6 on an aspirational goal that
taught you something, in the same forum where you would have celebrated a 1.0.

**Key results that are the roadmap** — "launch X," "hire 4 engineers," "migrate
the data warehouse." Tell: you could deliver every one of them and the P&L would
not notice. → Run the inversion test on every line. Move the deliverables into
the plan and put the customer-side or business-side change in the key result.

**Volume as seriousness** — 8 objectives and 30 key results, because cutting felt
like abandoning a team. Tell: nobody can recite the list; the document is
consulted only at scoring time. → Cap at three per team, force-rank the
remainder into a visible "not this quarter" list so the dropped work is
acknowledged rather than hidden.

**Rigid cascade** — every team's goals are mechanically derived from the level
above, top to bottom. Tell: front-line teams have goals they cannot influence,
and the planning cycle takes six weeks. → Push about half the goals bottom-up.
Leadership sets direction and the two or three company numbers; teams propose
how they contribute and negotiate the target upward or downward once.

**Set and forget** — defined in week one, reopened in week twelve. Tell: three
key results measure a metric no one has instrumented, and nobody noticed for two
months. → Weekly confidence check-in. Any key result without a live data source
by week two is void; either instrument it or replace it.

**Aspiration laundering** — everything is labeled aspirational, so nothing is
ever missed. Tell: the word "stretch" appears in retros far more often than in
planning. → Classification is locked at kickoff. Cap aspirational at one
objective per team. A missed committed goal requires a written cause, not a
reclassification.

**The unowned shared metric** — a key result belongs to "the company" or to two
teams jointly. Tell: it is green in one review and red in another. → Exactly one
named human owns each key result. Shared work gets a shared plan and a single
accountable owner, not shared ownership.

**Leadership exemption** — the CEO mandates the system and has no visible goals.
Tell: everyone can name their own goals and nobody can name leadership's. →
Publish leadership goals first and score them first, in front of the company,
including the ones that were missed.

## Outputs

- Three company objectives with 2–4 outcome-form key results each, every one
  labeled committed or aspirational, every one with a named owner
- The explicit "not this quarter" list of rejected candidates
- A rewrite log: each key result as originally proposed, the test it failed, and
  the outcome-form replacement
- A weekly check-in template keyed to confidence movement, not percent complete
- A scorecard with objective-level averages and a one-page cycle reflection:
  what we learned, which goal was wrong rather than missed, what changes next
- A written statement of the compensation firewall, published to the company

## Pairs with

- [`operations/management-os`](../../operations/management-os/SKILL.md) — the meeting cadence and delegation
  model that makes a quarterly goal system executable week to week
- [`operations/daily-management`](../../operations/daily-management/SKILL.md) — goals set the improvement agenda;
  daily management defends the level you already reached
- [`operations/constraint-analysis`](../../operations/constraint-analysis/SKILL.md) — use it before goal-setting, so
  the three objectives sit on the actual bottleneck rather than on the loudest
  team
- [`gtm/gtm-measurement`](../../gtm/gtm-measurement/SKILL.md) — for instrumenting the metrics your key
  results claim to move
- [`discovery/engagement-ethics`](../../discovery/engagement-ethics/SKILL.md) — run it before a retention or
  session-frequency key result ships, because that is the KR that quietly pays a team to make leaving hard

## Lineage

The mechanism comes from Andy Grove, who built objectives-and-key-results at
Intel out of management by objectives and made it operational in *High Output
Management*; John Doerr carried it to Google and wrote the popular account in
*Measure What Matters*, which added the committed-versus-aspirational split and
the surrounding practice of continuous conversations, feedback, and recognition.
Where this articulation departs from theirs: both treat the system as broadly
beneficial and the failure modes as implementation detail. In practice one
failure mode — coupling scores to pay — destroys the system so reliably that
everything else is secondary. I have compressed the framework to two gates and a
confidence-based weekly review, and dropped the multi-level cascade entirely,
because under a few hundred people it consumes more calendar than the goals are
worth.
