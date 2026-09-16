---
name: gtm-measurement
description: >-
  Builds the go-to-market measurement stack in the order that survives being
  wrong — money events first, activation second, attribution third — and names
  the metric that misleads at each stage of growth. Trigger when defining a
  tracking plan, choosing analytics tools, setting UTM conventions, structuring
  a CRM pipeline, building a growth dashboard, prioritizing conversion
  experiments, or diagnosing why a channel is not converting.
domain: gtm
stage: scale
lineage: "Dave McClure — pirate metrics (AARRR); Sean Ellis & Morgan Brown — *Hacking Growth*; Eric Ries — *The Lean Startup* (actionable vs. vanity metrics); Chris Goward — PIE prioritization"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# GTM Measurement

> You cannot rebuild history. Every week without instrumentation is a cohort you will never be able to analyze, and the cost lands in the quarter you most need the answer.

## The question this answers

- What do I instrument first, given that I cannot instrument everything before launch?
- Which channel actually produced this revenue, and how confident should I be in that answer?
- Why does the dashboard look healthy while the bank account does not?
- Which of my current metrics is quietly lying to me at this stage of the company?

## When to run it

Run this before a launch, when instrumentation is cheap and reversible. Run it when two people in a meeting quote different numbers for the same thing, when spend is about to increase and nobody can defend a cost per customer by channel, or when the pipeline lives in the founder's head.

**Do not run this when** you have fewer than roughly 30 customers or 100 activations per month. Below that volume, statistical machinery produces confident nonsense — talk to every customer individually and write down what they say. Analytics is a substitute for conversation only after conversation stops scaling. **Do not run this when** the real problem is that nobody has decided what the company is optimizing. Measurement systems built without a decision to serve become dashboards nobody opens.

## The method

### Move 1 — Name the one decision the data must support this quarter

Write it as a sentence: "By March we must decide whether to double down on outbound or move the budget to content." Every event and report either serves that decision or is deferred — the constraint that keeps a tracking plan at twelve events instead of ninety. If you cannot write the sentence, stop; instrumenting without a decision produces a warehouse and no answers.

### Move 2 — Instrument in this order, not in parallel

The order matters because the layers differ in how recoverable they are.

| Order | Layer | Why here | Recoverable later? |
|---|---|---|---|
| 1 | Identity and money events — signup, trial start, subscription started, plan changed, canceled with reason | Every other analysis joins to these; the cancellation reason field can never be backfilled | No |
| 2 | The single activation event — the one action that separates retained users from the rest | Defines time-to-value, the only early metric that predicts revenue | No |
| 3 | Acquisition source captured at signup and stamped on the user record | Attribution decays; a source not captured in the moment is gone | No |
| 4 | Behavioral breadth — feature usage, page flows, secondary funnels | Useful, but reconstructible from logs and later instrumentation | Mostly |

Ship layers 1-3 before launch; layer 4 can wait a quarter without permanent loss. Teams routinely invert this, arriving at launch with rich page analytics and no reliable record of who paid, from where, and why they left.

### Move 3 — Write the event contract before anyone writes code

One document, one owner, versioned. Naming fixed once: `object_action`, snake_case, past tense — `subscription_started`, not `StartSub`. Every event carries user id, account id, plan, and acquisition source, plus a plain-language trigger condition so QA can verify it fires once at the right moment.

Threshold: twelve events before launch, hard cap. Above twelve, the team has not decided what matters. Names are immutable after launch — a rename splits your history in two and you discover it six months later, mid-board-deck. Add new, deprecate old, never rename.

### Move 4 — Set attribution conventions, then set expectations about them

One naming guide, lowercase, no spaces, one shared builder, one owner who can veto ad-hoc parameters. Source is the platform, medium is the mechanism, campaign carries period and segment. Clerical, unglamorous, and the entire difference between a channel report and a mess.

Then be honest about the limits. Click attribution measures the last cheap thing before a decision that took eleven weeks. Add a free-text "how did you hear about us" field at signup as a corrective, not a supplement — when the two disagree systematically, paid is taking credit for demand that content and word of mouth created.

Decision rule: click attribution for optimization inside a channel; self-reported plus incrementality tests — turn a channel off for two weeks and watch total volume — for allocation between channels.

### Move 5 — Make the pipeline an instrument, not a narrative

Stages advance on buyer evidence, never seller activity. "Demo delivered" is an activity. "Buyer confirmed the problem is funded this fiscal year and named the approver" is evidence. Write every exit criterion as something the buyer did or said.

Non-negotiable deal fields: expected value, stage, next action with date and owner, champion, approver, blocker, loss reason from a fixed list. Review weekly on four numbers: coverage against target, win rate, cycle length, and the share of deals carrying a dated next action. The last one is the earliest warning of a pipeline that is fiction.

### Move 6 — Run experiments with a stop rule written before the start

Hypothesis in one sentence: if we change X for segment Y, metric Z moves N% because of evidence E. Score the backlog on potential lift, traffic importance, and ease; average the three; run the top item. Set sample size and end date before launching, minimum two weeks to cover weekday variation. Peeking is allowed; stopping early because it looks good is not.

### Move 7 — Route product usage into the pipeline without lowering the evidence bar

In self-serve or trial-led motions, usage inside the product is evidence too, sometimes better than anything a buyer says, because it is observed rather than reported. Define one usage threshold that has historically preceded conversion or expansion in your own data, not a borrowed benchmark: the activation event reached inside a set window, a plan limit hit, or the core action repeated enough to look habitual rather than accidental. Route accounts that cross it into three lanes: a self-serve nudge if usage stays inside plan limits, a sales or customer-success alert if a limit was hit or a second seat activated, and a paid implementation offer if usage signals a team large enough to need onboarding the software alone will not deliver.

This does not relax Move 5's rule. A usage threshold earns a pipeline entry, not a stage advance; the account still needs buyer-confirmed evidence before it moves past qualification. Treat the two evidence types as sequential gates, not substitutes, or the forecast fills with accounts that used a feature once and never spoke to anyone.

**Threshold:** if fewer than one in four routed accounts convert to a qualified conversation, the usage threshold is too loose and is routing curiosity, not intent.

## Metrics that mislead, by stage

| Stage | The metric that misleads | Why it lies | Watch instead |
|---|---|---|---|
| Pre-PMF | Signups, traffic, follower count | Measures your effort, not the product's pull; grows with any push | Week-4 retention of each weekly cohort |
| Early GTM | Trial-to-paid rate | On small denominators it swings 15 points on three customers | Absolute count of activations, and time-to-value |
| Early GTM | Blended CAC | Averages a nearly free founder-network channel with paid, hiding that paid does not work | CAC by channel, with self-reported cross-check |
| Early GTM | Pipeline value | Inflated by deals with no dated next action | Coverage using only deals that moved stage in 21 days |
| Scale | LTV:CAC | LTV built on an assumed churn rate you have not yet observed for a full year | CAC payback period in months — observable, not projected |
| Scale | MoM MRR growth | One-time services and annual prepayments smuggled into recurring | Net revenue retention on cohorts twelve months old |
| Scale | Aggregate churn | Hides that your best segment is stable while an unfit segment leaves | Churn by acquisition channel and by segment |
| Scale (PLG) | Product-qualified-lead count | Rises with any change to the usage threshold, not with real buying intent | PQL-to-qualified-conversation conversion rate |

## Failure modes

**Dashboard theater** — a weekly report nobody acts on, built because reporting feels like management. The tell: no decision last quarter changed because of a number on it. → Cut to the metrics tied to the move-1 decision. Five numbers that trigger action beat thirty that describe.

**Event sprawl** — ninety events, half never queried, names drifting between platforms, and analysis now requires a guided tour. The tell: two events that mean the same thing under different names. → Archive anything unqueried for 90 days; cap new events at a fixed budget per quarter.

**Attribution litigation** — marketing and sales argue over credit while the actual question, where to put the next dollar, goes unanswered. The tell: a meeting about the model rather than the budget. → Stop arguing; run a two-week incrementality test on the disputed channel and let total volume decide.

**Stage inflation** — deals sit in late stages because moving them backward looks bad, so the forecast is confidently wrong every quarter. The tell: a stage where deals age past twice the average cycle. → Enforce buyer-evidence exit criteria and run a monthly demotion pass on anything without a dated next action.

**Peeking and early stopping** — a test is called at day four because the variant "is winning," and the effect vanishes in production. The tell: results that never replicate. → Set the end date before launch; treat unfinished tests as no result, not a weak result.

**Instrumenting after launch** — tracking is deferred until things stabilize, so the launch cohort, the most informative one the company will ever have, is analytically dark. The tell: "we'll add that next sprint," said the week before shipping. → Layers 1-3 are launch blockers, same severity class as a broken checkout.

**Usage theater** — a dashboard tracks "product-qualified leads" that nobody in sales trusts enough to call. The tell: the PQL count never appears in the weekly pipeline review from Move 5. → Enforce Move 7's one-in-four conversion threshold and audit it monthly; retire the signal if it fails twice running.

## Outputs

- Tracking plan: up to twelve events with trigger conditions and properties, plus the user-trait list sent on identify
- Definition of the activation event and its measured threshold
- UTM naming guide with per-channel conventions and a shared builder
- Pipeline stages with buyer-evidence exit criteria and required deal fields
- Weekly dashboard spec: metric, source, owner, and the decision it informs
- Experiment backlog with hypothesis, sample size, duration, and stop rule per item
- Pre-launch instrumentation checklist with go/no-go status
- Usage threshold and three-lane routing rule for product-led motions

## Pairs with

- [`gtm/launch-execution`](../../gtm/launch-execution/SKILL.md) — instrumentation layers 1-3 are launch gates, not follow-ups
- [`operations/okr-system`](../../operations/okr-system/SKILL.md) — these definitions are the inputs to any credible objective
- [`discovery/experiment-design`](../../discovery/experiment-design/SKILL.md) — for designing the tests this backlog schedules
- [`gtm/growth-loops`](../../gtm/growth-loops/SKILL.md) — loop math is unmeasurable without cohort-level source capture

## Lineage

The funnel decomposition traces to Dave McClure's pirate metrics; the experiment cadence to Sean Ellis and Morgan Brown in *Hacking Growth*; the actionable-versus-vanity distinction to Eric Ries in *The Lean Startup*; the potential-importance-ease scoring to Chris Goward's conversion work. This articulation departs by specifying an implementation order based on recoverability — which data can be rebuilt later and which is gone forever — and by naming, per stage, the metric that reliably misleads. That CAC payback beats LTV:CAC before a full year of churn is observed is an operating position, not a standard one; Move 7's evidence hierarchy is the same position applied to product-led pipelines.
