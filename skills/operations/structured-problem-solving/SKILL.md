---
name: structured-problem-solving
description: >-
  Turns a vague business problem into an answer someone will act on: a sharp
  question, a hypothesis formed in the first hour, an issue tree that can
  falsify it, the two analyses that decide it, and a conclusion delivered
  answer-first. Use when facing an ambiguous strategic question, scoping an
  analysis, deciding what not to analyze, structuring a recommendation, or
  preparing to present findings to a board or executive team.
domain: operations
stage: any
lineage: "Ethan M. Rasiel & Paul N. Friga — *The McKinsey Mind*; Barbara Minto — *The Pyramid Principle*"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Structured Problem Solving

> A hypothesis you form in the first hour and try to kill beats a comprehensive analysis you finish in the sixth week.

## The question this answers

- What is the actual question here, as opposed to the one I was handed?
- Of the twenty analyses I could run, which two decide the answer?
- How do I know when to stop analyzing?
- How do I present this so a decision gets made rather than deferred?

## When to run it

Run it on questions that are ambiguous, consequential, and reversible only at
cost: whether to enter a segment, why a metric is deteriorating, which of three
options to fund. Run it when three smart people disagree and none can say why.

**Do not run this when** the answer is cheap to test. If the experiment costs a
fraction of the analysis, run the experiment; a week of structuring to avoid a
two-day test is procrastination with good posture. Also skip reversible
decisions — make them fast and correct them.

## The method

### 1. Fix the question before anything else

The problem as stated is usually a diagnosis someone already made. "How do we
reduce churn in the mid-market segment" presumes the churn, the segment, and the
lever. Rewrite it as one question with a decision attached, and have the person
who asked sign off on the rewrite.

Test: the question is sharp when you can name what a yes and a no each imply in
resources and action. If both lead to the same next step, find the question that
does not.

### 2. Write the hypothesis in the first hour

Take everything you already know — the data lying around, your instinct, the
pattern from adjacent situations — and commit to a probable answer before you
have earned it. This feels premature. It is the point. Testing a specific claim
is several times faster than gathering facts and hoping a conclusion emerges,
because it tells you which facts are irrelevant.

Then stress-test it cheaply before spending anything:

```
ASSUMPTION TEST — 15 minutes, before any analysis
1. List the assumptions that must ALL hold for the hypothesis to be true.
2. Mark each: known true / known false / unknown.
3. Any "known false" → the hypothesis is dead. Rewrite it now.
4. Rank the unknowns by cost to check and by how much they move
   the answer if wrong.
5. The top two are your first analyses. Everything else waits.
```

### 3. Build an issue tree, not a map of the world

Two structures get confused constantly, and picking the wrong one causes most
six-week analyses:

| | Logic tree | Issue tree |
|---|---|---|
| Nodes are | Components of the thing | Questions that must be answered |
| Answers | Describe the system | Prove or kill the hypothesis |
| Ends when | Decomposition is complete | The hypothesis stands or falls |
| Risk | Comprehensive and useless | None, if the questions are right |

Decompose one level at a time and keep each level MECE — mutually exclusive so
you do not analyze the same thing twice under two names, collectively exhaustive
so no path to the answer is missing. Two levels is usually enough. Three is a
project. Four means you are documenting the business, not answering the question.

The discipline that makes the tree work: phrase every branch so answering it
eliminates something. If its answer would not change your next move either way,
prune it.

### 4. Design the smallest analysis that decides it

For each surviving branch, write one line before doing any work: the analysis,
the data it needs, the likely source, and a sketch of the end product — the chart
with axes labeled and numbers blank. If you cannot sketch it, you do not know
what you are looking for.

Then apply three rules:

- **Priority.** Most of the answer comes from a small fraction of the possible
  analyses. Run the one that would most change your conclusion first; it often
  makes several others unnecessary.
- **Precision.** Business is not physics. Directionally correct and within an
  order of magnitude usually decides it. Refining an estimate that cannot change
  the decision is a hobby.
- **Triangulation.** When the data does not exist, bound it: an upper limit, a
  lower limit, an analogy. Three rough approaches converging beats one precise
  number you cannot get.

### 5. Interpret honestly, and let the data rewrite you

Two paths at every result. If the analysis supports the hypothesis, state the
action it implies. If it contradicts the hypothesis, rewrite the hypothesis —
never reshape the data or quietly drop the inconvenient analysis. Being wrong in
week one and right in week three is the design working.

Every output faces the so-what test: what does this tell us, and what would we do
differently? An analysis with no recommendation is trivia.

Sanity check before committing: how wrong would this number have to be to change
the recommendation? "Slightly" means run another analysis. "By a factor of three"
means stop working.

### 6. Deliver answer-first

Lead with the conclusion, then the two or three reasons supporting it, then the
evidence under each. The alternative — walking an audience through your reasoning
to a conclusion at the end — asks them to hold the whole analysis in their head
and pays out on the last slide. Executives interrupt at slide four and you never
reach the point.

Structure test: state the answer and its support in thirty seconds, out loud. If
you cannot, either you do not understand it or the structure is wrong. A
well-built issue tree is already the outline.

One message per exhibit, and the message is the title. A chart needing a
paragraph of narration is two charts.

Finally, no surprises. Walk key stakeholders through the findings individually
beforehand. Pre-briefing is not politics; it is how analysis becomes decision.

## Failure modes

**MECE as procrastination** — the tree gets more elegant every day and no
analysis has started. Tell: day eight, four levels, nobody can state the
hypothesis in a sentence. → Time-box structuring to one session. MECE is a check
you apply to a level, not a standard you reach before starting.

**Boiling the ocean** — every branch analyzed to the same depth, because cutting
one feels like sloppiness. Tell: nineteen analyses, none marked decisive. → Force
a ranking. Ask of each: if this came back the opposite way, would the
recommendation change? If not, delete it.

**Hypothesis lock-in** — the initial guess becomes the thing being defended, and
disconfirming data is recast as an edge case. Tell: nothing has changed in three
weeks. → Write the kill condition when you write the hypothesis: "we abandon this
if X." Give someone the job of arguing against.

**False precision** — three weeks refining a model to two decimals on an input
that does not change the answer. Tell: the debate is about methodology, not the
decision. → Run the sanity check. If the recommendation holds across a wide
range, present.

**Buried lede** — context, method, findings, recommendation on slide 34. Tell:
the meeting ends with "send us the deck." → Conclusion on slide one, three
arguments, evidence beneath. Depth on demand.

**No so-what** — an accurate chart that implies no action. Tell: the audience
nods and asks nothing. → Every exhibit earns its place by changing what someone
does. Otherwise, appendix.

**Framework theater** — the vocabulary of structure becomes the product. Tell:
pushback is about method, not substance. → Take the scaffolding down before
delivery and speak in the language of the business.

**Ambush at the readout** — the decision-maker hears the conclusion for the first
time in front of peers. Tell: the meeting becomes a debate about data quality. →
Pre-brief everyone who can block it.

## Outputs

- The rewritten question, one sentence, with what a yes and a no each imply
- A hypothesis with its assumption test done and its kill condition stated
- A two-level issue tree, MECE at each level, pruned branches marked
- A work plan: per branch, analysis, data, source, end-product sketch, owner,
  date
- The two decisive analyses, done, with the so-what written under each
- An answer-first summary: conclusion, three arguments, evidence, and a
  thirty-second spoken version
- A pre-brief list: who hears this beforehand, and what each will object to

## Pairs with

- [`operations/constraint-analysis`](../../operations/constraint-analysis/SKILL.md) — when the question is "why is
  output capped," this answers it faster than a general tree
- [`operations/daily-management`](../../operations/daily-management/SKILL.md) — supplies the anomaly data that
  usually contains the real problem statement
- [`discovery/experiment-design`](../../discovery/experiment-design/SKILL.md) — for when the assumption test says
  the cheapest way to resolve an unknown is to test it
- [`operations/okr-system`](../../operations/okr-system/SKILL.md) — for turning a recommendation into a goal
  someone owns

## Lineage

The problem-solving sequence comes from Ethan M. Rasiel and Paul N. Friga's *The
McKinsey Mind*, which codified the firm's practice for people outside it:
structure before facts, MECE decomposition, the initial hypothesis, the issue
tree, the work plan, 80/20 prioritization, and the discipline of the so-what. The
communication architecture — answer first, then arguments, then evidence, each
level summarizing the one below — is Barbara Minto's *The Pyramid Principle*,
developed at the same firm and the most durable thing consulting has given
general management. Where this departs: both assume teams with weeks and a
research department. Operators have neither, so I have made the assumption test a
hard gate before any analysis, capped the issue tree at two levels, and treated
the tree's function as elimination rather than description. Pre-briefing is part
of the method here, because an analysis that does not end in a decision has not
finished.
