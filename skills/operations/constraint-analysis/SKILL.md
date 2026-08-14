---
name: constraint-analysis
description: >-
  Finds the one place in a business that actually caps output, then routes every
  decision through it: identification procedure for systems with no visible
  queue, exploitation before investment, subordination of everything else, and
  the inertia check for when the constraint moves. Use when growth has plateaued
  despite everyone being busy, when deciding where to add headcount or spend,
  when lead times keep slipping, or when local efficiency metrics look good and
  results do not.
domain: operations
stage: any
lineage: "Eliyahu M. Goldratt — *The Goal* and the Theory of Constraints"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Constraint Analysis

> Every system has exactly one thing limiting its output at any moment. Effort spent anywhere else feels like progress and produces none.

## The question this answers

- Everyone is busy and fully utilized. Why is output flat?
- Where do I put the next hire, the next dollar, the next month of engineering?
- Why do lead times grow while capacity keeps being added?
- We fixed the bottleneck. Why did nothing improve?

## When to run it

Run it before any capacity decision — headcount, tooling, budget — and whenever a
business works harder without producing more: lengthening delivery times, work
piling up somewhere, high utilization alongside missed commitments.

**Do not run this when** the constraint is obviously demand and you know it. That
is a market and positioning problem, and flow analysis on an under-loaded system
produces elegant optimization of idle capacity. Also skip genuinely novel work,
where the output is learning and there is no repeatable flow to constrain.

## The method

### 1. State the goal and the unit of throughput

Throughput is the rate at which the system converts work into money through
completed, delivered, accepted output. Not activity, not utilization, not units
produced and stored. Pick one unit and hold it fixed: signed contracts per month,
delivered projects per quarter, features live in production. Alongside it, track
the money tied up in undelivered work and the money spent converting one into the
other. Most teams have the priority backwards: cutting expense has a floor,
raising throughput does not.

### 2. Find the constraint — including where nothing piles up visibly

In a factory the constraint announces itself: material piles up in front of it
and every expediter goes there first. In a sales organization, an engineering
team, or a services firm there is no pile, so you have to make the queue visible.
Run five tests and take the answer two or more agree on.

| Test | How to run it | What it reveals |
|---|---|---|
| Wait ratio | Per stage, measure elapsed time entry to exit and hands-on working time. Divide. | The stage with the highest ratio *and* a growing queue. A stage at 40:1 is where your lead time lives. |
| Calendar depth | Whose calendar is booked furthest out? Who does everyone schedule around? | Human constraints appear as scheduling latency before any dashboard shows them. |
| Expedite trail | When something is urgent, whose desk do people go to, and who is asked to skip the line? | People route around the system straight to the constraint. |
| Doubling test | If this capacity doubled tomorrow, does throughput rise? | Only one answer is yes. If doubling a team changes nothing, it is not the constraint. |
| Starvation check | Which resource, idle, stops the whole flow — and which can idle harmlessly? | Idleness at the constraint is the only idleness that costs output. |

Typical answers outside manufacturing, none visible on an org chart:

- **Sales organization.** Rarely rep count. Usually the supply of qualified
  opportunities, one solutions engineer every deal needs, or a security-review
  and legal queue adding three weeks to every close.
- **Engineering team.** Rarely engineer count. Usually code review, a shared
  environment, a QA stage, or product decisions arriving slower than the team
  can implement them.
- **Services firm.** Almost always one or two senior people whose signature
  every engagement requires.

Then classify. A physical constraint is capacity: hours, seats, machines. A
policy constraint is a rule, metric, or approval creating the queue artificially.
Below a few hundred people most constraints are policy constraints in a capacity
costume, and those are free to remove.

### 3. Exploit before you spend a cent

Get the maximum out of the constraint as it stands. Four moves, in order:

1. **Stop losing its minutes.** No context switching, no meetings that could be
   asynchronous, no admin someone else could do. A constraint doing
   non-constraint work is the most expensive thing you own.
2. **Put the quality gate in front of it.** Reviewing the brief before the senior
   architect touches it costs an hour; finding out later costs a week.
3. **Feed it only real demand.** Speculative work at the constraint is capacity
   converted directly into nothing.
4. **Sequence by real urgency**, not batch convenience or volume of complaint.

The number that wins this argument: an hour lost at the constraint costs the
system's entire operating expense divided by the constraint's productive hours.
Compute it once and say it out loud. It is usually an order of magnitude above
what anyone assumed.

### 4. Subordinate everything else, and mean it

Every other resource runs at the pace the constraint can absorb, not its own
maximum. Release new work only when the constraint is ready for it, with a
protective buffer ahead. In knowledge work this is a work-in-progress limit, the
highest-return operational change most teams can make.

Accept the consequence out loud: non-constraint resources will sit idle, and that
is correct. Activating them produces work-in-progress, longer lead times, and no
extra throughput.

Buffer sizing: enough to absorb normal upstream variation, no more. Watch the
holes — the times the constraint nearly ran dry. Repeated holes from one source
is a chronic problem worth fixing; no holes ever means the buffer is too large
and is inflating lead time. A buffer here is not waste; it is insurance priced in
constraint time.

### 5. Elevate, only now

Now spend: add capacity, hire, buy the tool, subcontract, split the work onto a
less efficient alternative. Doing this before steps 3 and 4 is how companies buy
capacity they already had.

### 6. Go back to step 1, and hunt the inertia

When you break a constraint it moves — usually somewhere nobody is watching,
sometimes out of operations and into the market. The rules, metrics, and habits
built around the old constraint survive it and are now actively destructive.
Every time it moves, review every policy created to protect the previous one.
This is the step everyone skips, and it is why the second round of improvement
usually delivers less than the first.

## Failure modes

**Optimizing a non-constraint** — automation or a redesign lands on a stage that
was never limiting. Tell: the local metric improved and the delivery date did
not. → Run the doubling test before approving the work. If doubling that capacity
would not raise throughput, it is cost with no return.

**Utilization as a virtue** — leadership tracks how busy each team is and rewards
high numbers. Tell: utilization above 90% everywhere and lead times still
growing. → High utilization at non-constraints manufactures work-in-progress.
Measure flow time and throughput instead.

**Mistaking a policy for a physical limit** — "we need three more people in
review," when review is slow because of a batching rule nobody has revisited.
Tell: the fix is always headcount, and the queue returns within two quarters of
each hire. → Classify before spending. Remove the rule, re-measure.

**The founder as the constraint** — every decision, customer, and hire routes
through one person who cannot see it from inside. Tell: calendar depth points at
them, and they call it being busy rather than a system limit. → Apply exploit and
subordinate to that person as ruthlessly as to any machine: strip non-constraint
work, gate inputs, treat handing off a decision class as elevating capacity.

**Inertia after the constraint moves** — priority flags, buffer, and weekly
meeting still protect a bottleneck that stopped being one nine months ago. Tell:
nobody can explain a rule beyond "we have always done it this way." → Date-stamp
every constraint policy; review when it changes, delete by default.

**Refusing to see a market constraint** — capacity is abundant and nobody wants
to say demand is the limit. Tell: operations keeps optimizing while the pipeline
is thin. → Exploitation changes shape: short reliable lead times and dependable
promise-keeping become the weapon, because a saturated competitor cannot offer
them.

## Outputs

- The system's goal and its throughput unit, in one line
- The five-test table filled in, with the constraint classified physical or policy
- The computed cost of an hour lost at the constraint
- An exploitation list: what stops consuming constraint capacity, with owners
- A subordination rule: work-in-progress limit or release cadence, plus buffer
  size and position
- An elevation proposal gated behind the exploitation list
- A dated register of policies protecting this constraint

## Pairs with

- [`operations/daily-management`](../../operations/daily-management/SKILL.md) — stabilize the constraint's process
  first; an unstable bottleneck cannot be exploited reliably
- [`operations/okr-system`](../../operations/okr-system/SKILL.md) — the constraint should decide what the
  quarter's objectives are about, not the loudest team
- [`strategy/scaling-playbook`](../../strategy/scaling-playbook/SKILL.md) — for the constraints that move
  predictably as a company grows

## Lineage

The Theory of Constraints is Eliyahu M. Goldratt's, laid out in *The Goal* as a
novel and developed across his later work: the three operational measures, the
five focusing steps, drum-buffer-rope, and the observation that most real
constraints are policies rather than machines. His deepest point is the framing
rather than the method — a system of local optima is not an optimal system, and
every efficiency metric ignoring this makes things worse confidently. Where this
departs: Goldratt wrote for a plant, where the constraint is a visible physical
queue. The operators who most need this run sales organizations, engineering
teams, and services firms, where the queue is invisible and the constraint is
often a person or an approval. I have replaced the shop-floor heuristics with
five tests that work when nothing piles up, made the physical-versus-policy
classification mandatory before any spend, and put the inertia review on a
register.
