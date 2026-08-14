---
name: engagement-ethics
description: >-
  A design-review instrument for auditing your own product's retention mechanics:
  where engagement stops creating value and starts extracting it, and what to do
  when the growth metric and the user's interest point in opposite directions. Use
  before shipping streaks, autoplay, variable rewards, or notification loops, when
  choosing a north-star metric, or when engagement is up and something feels wrong.
domain: discovery
stage: any
lineage: "Natasha Dow Schüll — *Addiction by Design*; Nir Eyal — *Hooked* (as counterpoint)"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Engagement Ethics

> Every retention mechanic makes leaving harder than staying. The only question is whether you managed that by becoming more valuable or by becoming harder to leave.

## The question this answers

- Is this feature earning attention or extracting it?
- Engagement is up and something feels wrong — is the gain real?
- What do I do when the quarterly target and the user's interest genuinely diverge?
- Which of our mechanics would be indefensible if described accurately in public?

## When to run it

Run it as a gate before shipping anything designed to increase session length,
frequency, or return rate: streaks, autoplay, variable rewards, loss-framed
notifications, infinite feeds, in-product currencies. Run it when choosing a
north-star metric, annually across the whole surface, and when regulation lands on an
adjacent category.

**Do not run this when** the product has no engagement to audit. Reviewing retention
ethics on a product nobody returns to is procrastination in a moral costume. This is
also not a legal review — consumer protection, gambling, and children's privacy law
each have their own counsel — and not a substitute for a safety review where harm is
direct.

## The method

### 1. State the alignment, or state the conflict

Write two sentences: what the user came to accomplish, and what your primary metric
counts. Then ask: **if the user accomplished their goal faster, would your metric go
up or down?**

| Relationship | What it means | What is required |
|---|---|---|
| Rises when the user succeeds faster | Aligned | Normal product judgment |
| Indifferent to user success | Proxy risk; you will drift | Replace the metric |
| Rises when the user succeeds slower or not at all | Structural conflict | Name it in writing, install a counterweight metric of equal standing |

Most products that end up extractive never decided to be. They chose a metric whose
gradient pointed away from the user and followed it for two years. Unstated conflicts
get resolved by whoever owns the dashboard.

### 2. Audit the four mechanism classes

These four levers produce compulsive rather than voluntary use. The audit question is
not "do we use this" — nearly every product does — but "what does it do to a user
already struggling to stop?"

| Class | What it does | Audit question |
|---|---|---|
| Stopping cues removed | Deletes the natural end of a session: no clock, no last item | Where does a session end by design rather than by exhaustion? |
| Tempo | Removes friction until interaction outruns deliberation | Is there any point where the user decides rather than reacts? |
| Odds and near-outcomes | Perceived probability diverges from real; near-misses read as progress | Would this still work with the true odds shown next to it? |
| Adaptive personalization | The system learns what holds this user and serves more of it | Does the model optimize for satisfaction, or for return? |

Grade each mechanic you find, and gate accordingly.

| Level | Description | Gate |
|---|---|---|
| 1 | Engaging, clear stopping points, honest feedback | Ship |
| 2 | Intense but bounded; the exit is visible | Ship with review |
| 3 | Active retention pressure: loss framing, streak anxiety, exit friction | Only with its counterweight in the same release |
| 4 | Time or value perception deliberately distorted | Named executive owner plus written justification |
| 5 | Extraction from users who cannot regulate: obscured real-money cost, targeting a struggling cohort | Red line. Remove what exists. |

### 3. Run the three reversal tests

**The informed-user test.** If you showed the user the design document — the intent,
the experiment results, why that notification fires at that hour — would they endorse
their own usage? A mechanic that only works while invisible is not a feature.

**The exit test.** Seconds and clicks from wanting to leave to being gone: canceling,
exporting data, deleting the account, silencing notifications. Compare against signup.
A ratio above roughly 3:1 is a decision someone made, and the first thing quoted back
at you.

**The heavy-user test.** The sharpest instrument here. Take the top 0.1% by time or
spend, compute what share of revenue they carry, then look at their behavior: session
lengths, time of day, spend velocity, support contacts, refunds. Extractive businesses
have a signature — a small cohort funds the company, their usage does not look like
enthusiasm, and nobody wants to open that dashboard. Revenue from users whose pattern
you would not want a family member to have is not a power-user segment. It is a
dependency, and the part of revenue a regulator or platform removes overnight.

### 4. Ship counterweights in the same release, not the same year

For any mechanic at level 3 or above, the counterweight is part of the definition of
done: whatever the mechanic removes, put back on the user's side.

| Mechanic | Counterweight that actually works |
|---|---|
| No natural end to the session | Session summaries, elapsed time, breakpoints |
| Autoplay and continuous feed | Opt-in per session, not a setting buried at install |
| Abstracted currency, credits, tokens | Real-money equivalent at the point of decision |
| Near-outcome and progress framing | Honest probability, honest progress |
| Adaptive retention targeting | Exclude distress-signaling cohorts from retention campaigns |
| Exit friction | One-screen cancellation, complete data export |

One rule stops this becoming decoration: a safeguard designed by the team whose bonus
depends on the mechanic will be designed to fail, so someone outside that team sets its
adoption and efficacy targets.

### 5. Have a procedure for the divergence, before it happens

There will be a quarter where the target requires a mechanic you graded 3 or 4. Agree
the procedure in advance: name the conflict in a paragraph, propose the counterweight,
define the condition under which you would remove the mechanic, record who decided.
Keep a red-line list, owned by someone with standing to say no. It is only real if it
has cost you something at least once.

## Failure modes

**Revenue concentration in the harmed tail** — a small cohort of extreme users funds
the P&L. Tell: nobody has computed revenue share by usage decile, or it exists and is
never shown. → Compute it quarterly, in the growth pack. Concentration beyond what a
healthy distribution predicts is a business risk before it is an ethical one.

**Flow-washing** — depletive immersion described as delight, stickiness, magic. Tell:
internal language celebrates users losing track of time. → Enriching immersion leaves
the user with more capability than they started with. Less time, money, and
self-regard is not flow.

**Consent theater** — defaults engineered so the extractive option is the path of least
resistance. Tell: the opt-out sits two levels deeper than the opt-in. → Opting out must
cost no more clicks than opting in, in the same register.

**Ethics as a comms function** — a responsible-use page, a wellbeing dashboard nobody
opens. Tell: the mechanic shipped, nothing changed. → A program that never delayed a
feature has not happened.

**Metric laundering** — the north star is a proxy that improves when users are
distressed: time in app, notification-driven sessions, re-engagement rate. Tell: it
rose in a quarter when qualitative feedback got worse. → Use a metric that improves
only when the user gets what they came for, plus a counter-metric.

**Competitive absolution** — "everyone in the category does this." Tell: the
justification references a competitor rather than a user. → The category is not a
standard, it is a shared exposure. Categories get re-regulated together, and the
cleanest audit trail survives it.

**Agency as deflection** — "adults make their own choices." Tell: the argument appears
only when a mechanic is challenged, never when success is claimed. → Agency is real and
operates inside an environment you designed. You cannot take credit for shaping
behavior in the growth review and disclaim it here.

## Outputs

- A mechanic inventory: every retention lever, mapped to its class and graded 1–5
- An alignment statement: is the primary metric aligned, indifferent, or in conflict
- A revenue-by-usage-decile analysis with a written read on the heavy-user cohort
- Exit-test measurements: clicks and seconds to cancel, export, and silence, vs signup
- A counterweight backlog, release-gated to the mechanics that require them
- A red-line list with an owner, plus an escalation memo template

## Pairs with

- [`gtm/growth-loops`](../../gtm/growth-loops/SKILL.md) — that skill installs the mechanics this one audits;
  run them together or the loop wins by default
- [`gtm/gtm-measurement`](../../gtm/gtm-measurement/SKILL.md) — choosing a north-star metric whose gradient points
  at user success
- [`discovery/jobs-to-be-done`](../../discovery/jobs-to-be-done/SKILL.md) — the alignment test needs an honest account of
  what the user came to accomplish
- [`brand/positioning`](../../brand/positioning/SKILL.md) — reputational exposure from mechanics you would not
  describe out loud

## Lineage

Natasha Dow Schüll's *Addiction by Design* is fifteen years of ethnographic fieldwork
on machine gambling, and it is a critique, not a manual: it argues that compulsive use
is manufactured by design and then attributed to the individual. It supplies the
concepts this audit runs on — engineered loss of stopping cues, the gap between real
and perceived odds, and the observation that the industry's preferred fix always
targets the user's behavior rather than the machine. Nir Eyal's *Hooked* describes much
the same loop from the builder's chair, which makes it the useful counterpoint. Where
this departs from both: intent does not settle the question. The tests I trust are
empirical — where revenue concentrates, whether the counterweight shipped, how long it
takes to leave. Those are auditable; stated intentions are not.
