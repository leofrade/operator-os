---
name: daily-management
description: >-
  Separates the work of holding a result from the work of raising it, then
  installs the routine that holds it: control items with action rules, written
  standards for the tasks that matter, and an anomaly-treatment loop with named
  roles. Use when quality depends on who happens to be working, when the same
  incident keeps recurring, when improvements decay a month after the project
  ends, or when a team is trying to improve a process that is not yet stable.
domain: operations
stage: scale
lineage: "Vicente Falconi Campos — *Gerenciamento da Rotina do Trabalho do Dia a Dia*, *O Verdadeiro Poder*; W. Edwards Deming and the Japanese TQC tradition"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Daily Management

> Every company runs two systems and almost none of them know it: one that holds the level you have reached, one that raises it. Confuse them and you spend years improving things that keep sliding back.

## The question this answers

- Why does the same incident keep happening, with a new explanation each time?
- Why did the improvement project's gains vanish four months after it ended?
- Which numbers should a team watch daily, and what happens when one moves?
- Are we ready to improve this process, or must it first behave the same way twice?

## When to run it

Run it when output quality depends on who happened to do the work, when the same
class of failure recurs monthly, or when a real gain has since decayed. Run it
before any improvement program on a process that is not yet repeatable.

**Do not run this when** the process is still being invented. Standardizing a
discovery loop, an early sales motion, or a research workflow freezes learning at
the moment learning is the output. Standards are for work whose right answer is
known. Also skip a process you are about to delete or automate away.

## The method

### 1. Sort every activity into maintain or improve, and say which out loud

| | Maintain (SDCA) | Improve (PDCA) |
|---|---|---|
| Target | Hold the current level | Move to a new level |
| Cycle | **S**tandardize → Do → Check → Act on deviations | **P**lan → Do → Check → Act to standardize |
| Trigger | A deviation from the standard | A gap between a goal and today's result |
| Owner | The people who run the process | A named project owner, with a deadline |
| Success | Nothing surprising happened | The number moved and stayed moved |
| Failure | Anomalies recur | The gain decays back to baseline |

The cycles differ in one letter and in everything that matters. SDCA starts from
a standard and acts on deviations. PDCA starts from a gap and ends by writing a
new standard — which is how it closes into an SDCA instead of staying a hero
project.

Rule: if a process is not under SDCA, do not run PDCA on it. You cannot tell
whether a change worked when the baseline moves for unexplained reasons.

### 2. Define control items and verification items, and separate them

- **Control items** measure the result the process delivers — quality, cost,
  delivery time, safety, the condition of the team. Each has one named owner.
- **Verification items** measure the causes driving the control item — the
  inputs you can actually touch.

Most teams instrument only control items, then hold meetings staring at a number
they cannot move directly. A control item with nothing beneath it is a
scoreboard, not a management system.

Each control item needs a target with a direction, a frequency set by how fast
the process drifts, and a standard action on deviation decided in advance.

```
CONTROL ITEM   Onboarding: days from signature to first productive use
Target:        <= 5 days    Frequency: weekly    Owner: one person
Verification:  % of kickoffs within 48h of signature
               % of accounts with data access granted at kickoff
               Open blocking questions per account
On deviation:  Owner-led review same day; written cause classified against
               the known failure list
```

### 3. Write standards only for the tasks that decide the outcome

Filter hard: write a standard only for tasks that materially affect the result
the customer experiences *and* are performed by a human with discretion.

Write it with the people who do the work, as the best currently known way —
provisional, versioned, owned. A standard nobody helped write is a document; one
the team wrote is how they work. Then train against it; untrained standards are
the commonest form of paper compliance.

Test: ask two people who do the task to describe the sequence independently. If
they diverge on anything affecting the result, write the standard.

### 4. Install the anomaly routine, with roles that do not overlap

An anomaly is any event outside the standard: an outage, a botched delivery, an
invoice error, a defect that reached a customer, a step someone improvised. All
work spent on anomalies adds cost and no value. It is not a normal part of
running a business; it is the tax on the parts of the system not yet under
control.

Three roles, three jobs. The failure is doing only the first:

| Role | Job | Time horizon |
|---|---|---|
| Person on the ground | Report it, take the containing action the standard defines | Minutes |
| Their lead | Analyze this occurrence, propose a countermeasure in the process | Days |
| The manager | Attack recurring anomalies at the level of process design and incentives | Weeks |

Each anomaly produces a short record: what happened, immediate action, cause,
permanent countermeasure, check that it worked. Records exist to be counted and
grouped, not filed. Monthly, sort by frequency and read the top three — your
improvement agenda, set by the operation rather than by opinion.

Threshold: the same anomaly class three times is not an incident. It is a defect
in the standard, and it escalates.

### 5. Convert every improvement into a standard, or forfeit it

A PDCA that ends at "the number improved" produced a temporary result. The final
act is rewriting the standard, retraining the people, returning the process to
SDCA at the new level. Skip it and you get the familiar pattern: a strong
quarter, a case study, a slow slide back to baseline as the people who did it
move on.

Exit criterion: standard updated, team trained, control item holding the new
level for two full measurement cycles.

### 6. Set improvement goals from gaps, and negotiate them both ways

A goal is a number, a direction, and a date; a problem is the distance between
that goal and today. Derive goals from four sources: the gap to a credible
benchmark, customer complaints, drift in your own results, and where leadership
says the business must be. Deploy by negotiation — the level above proposes, the
level below accepts or shows the means are missing. Targets imposed without that
exchange are received as weather.

## Failure modes

**Improving on unstable ground** — experiments run on a process whose baseline
swings 40% week to week. Tell: results are always "inconclusive," or reverse next
month. → Stabilize first: standard, training, anomaly routine.

**Firefighting as identity** — the operator who handles the most incidents gets
promoted. Tell: incident volume is flat year over year while the response is
heroic. → Make recurrence the metric. Reward the person who made a class of
incident stop happening.

**The standard nobody wrote** — a staff function produces procedure documents the
people doing the work have never read. Tell: the document says one thing,
everyone does another, and nobody sees a contradiction. → Rewrite with the
operators, version it, name an owner, retrain. When reality and the standard
disagree, decide which one is wrong.

**PDCA that stops at C** — good analysis, executed plan, reported result, no new
standard. Tell: the same improvement appears on next year's project list. → Make
the standard update the exit criterion, not a follow-up.

**Scoreboard management** — output metrics with no input metrics beneath them.
Tell: monthly meetings explain a number instead of acting on a cause. → Name
verification items and owners under every control item.

**Turnover as an HR metric** — churn is discussed as cost per hire. Tell: process
performance degrades in a predictable rhythm after each departure. → Turnover is
knowledge leaving the building, most of it tacit. No process holds stable while a
third of the people running it are new each year. Retention in critical roles is
an operating constraint.

## Outputs

- A two-column map: which activities are maintain, which are improve, and which
  improve items are illegitimate because the process is unstable
- A control-item sheet per critical process: target, frequency, owner,
  verification items, standard action on deviation
- A shortlist of tasks warranting a written standard, with owners and training
- An anomaly log plus the monthly frequency ranking that sets the agenda
- Per improvement project: standard updated, team trained, item held two cycles

## Pairs with

- [`operations/okr-system`](../../operations/okr-system/SKILL.md) — the improvement side of the split;
  quarterly goals set the PDCA agenda this routine locks in
- [`operations/constraint-analysis`](../../operations/constraint-analysis/SKILL.md) — which process to stabilize
  first, so the routine lands on the bottleneck
- [`operations/structured-problem-solving`](../../operations/structured-problem-solving/SKILL.md) — the analysis method for
  the cause step, when the anomaly log does not hand you the answer
- [`operations/management-os`](../../operations/management-os/SKILL.md) — the delegation model that keeps
  standards holding without the manager in every loop
- [`strategy/scaling-playbook`](../../strategy/scaling-playbook/SKILL.md) — when the standard breaks because
  headcount doubled rather than because the process drifted; the routine gets rebuilt at each threshold

## Lineage

This is the Brazilian articulation of total quality management built by Vicente
Falconi Campos, who took the Japanese TQC tradition — Deming's cycle, Ishikawa's
company-wide quality control, Hoshin Kanri for goal deployment — and turned it
into a system that reshaped much of Brazilian industry and public administration
from the 1990s on. Its distinctive contributions: the explicit SDCA/PDCA split,
the insistence that stability precedes improvement, the control-item versus
verification-item distinction, and the treatment of anomalies as pure cost with
named roles per tier. It is close to unknown in English-language startup
writing, which is a real loss: software has continuous improvement without the
maintenance cycle, which is why so many of its improvements do not stick. Where
this departs: the original was written for plants and standardizes aggressively.
I have narrowed the filter to outcome-critical, human-performed tasks, barred the
routine from processes still being invented, and dropped the goal-deployment
maturity ladder.
