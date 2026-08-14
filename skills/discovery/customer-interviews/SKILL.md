---
name: customer-interviews
description: >-
  Runs discovery conversations that produce evidence instead of encouragement, by
  forcing past-tense specifics, neutralizing praise, and closing for a real
  commitment. Use when planning or reviewing customer interviews, writing a
  discovery script, auditing interview notes, choosing who to talk to, deciding
  whether a problem is worth building for, or diagnosing why conversations feel
  positive but nothing converts.
domain: discovery
stage: pre-pmf
lineage: "Rob Fitzpatrick — *The Mom Test*"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Customer Interviews

> Customer conversations produce garbage by default. The interview is not data collection — it is a procedure for making it hard for the other person to be polite to you.

## The question this answers

- "I have a dozen conversations lined up. What do I ask so the answers are worth anything?"
- "Everyone says they love it and nobody buys. What am I doing wrong in the room?"
- "How many conversations until I can stop and start building?"
- "This person seems interested. Is that signal or manners?"

## When to run it

Run this when you are deciding what to build, who to sell to, or whether a problem carries budget — and the honest answer is that you are guessing. Run it before the spec, the pricing page, the first sales hire. Run it again when growth goes flat, because flat growth at small scale is usually a discovery failure in a marketing costume.

**Do not run this when** the open risk is technical rather than commercial. If the question is "can this be built", conversation cannot settle it — build something disposable and measure. Skip exploratory interviews once you have paying users doing repeated work in the product: behavior outranks testimony, and interviews turn diagnostic.

## The method

### 1. Fix the segment as a who-where pair

Write one sentence before scheduling anything: **who** they are, specifically enough to name three real people, and **where** you find more of them. "Operations managers at regional freight carriers, found at the state trucking association's monthly meetup" is a segment. "Logistics companies" is a wish.

Decision rule: if you cannot name the place, keep slicing. Ask which subset wants this most, why, and what they do about it today — the workaround tells you where they congregate. A segment you cannot reach is a market study. Inconsistent findings usually trace back to a segment that was really three.

### 2. Write the three questions and apply the fear test

For each batch, write the three things you must learn. Not topics — questions whose possible answers would change your plan. Then apply the fear test: at least one should be uncomfortable to ask, because a bad answer costs you the plan. If none scare you, you wrote the safe ones. Useful prompt: assume the company failed eighteen months from now — what killed it? Ask about that.

Decision rule: if you cannot say what you would do differently under each of the two likeliest answers, the question is decorative. Rewrite it or cancel the meeting.

### 3. Interrogate the past, never the future

Every question should be answerable by recalling something that already happened. The future is where people are generous with you.

| Instead of | Ask |
|---|---|
| "Would you use this?" | "Walk me through the last time you dealt with that." |
| "Would you pay $X?" | "What are you spending on this today — tools, hours, people?" |
| "Is this a big problem?" | "What did it cost you the last time it went wrong?" |
| "How do you usually handle it?" | "Show me how you handled it this week." |

Two questions earn a place every time. **"What else have you tried?"** produces the price anchor, the switching cost, and proof the problem already cost them effort. **"Who else should I talk to?"** goes at the end, and turns one conversation into a chain.

Threshold: at least one dated, concrete incident per person. Zero incidents means the problem is theoretical for them, whatever their enthusiasm suggests. Three in a row with no incident means the wrong segment, not bad luck.

### 4. Neutralize the three contaminants live

- **Praise** — "I love it." Deflect back to their life: "Thanks. Sounds like you handle a lot of this already — how are you managing it today?" Never record praise as a finding.
- **Generalities** — "I always...", "we'd definitely...". Anchor to an instance: "When was the last time?" then "What happened?" People describe an idealized self in the general tense and a real one in the past.
- **Feature requests** — they start designing your product for you. Do not take the order. Ask why they want it, what it would let them do, how they cope now.

Rule: understand requests, do not obey them. They own the problem. You own the solution.

### 5. Close for a commitment priced in time, reputation, or money

A conversation that ends warmly and vaguely was entertainment. Ask for something that costs them.

| Currency | Weak | Real |
|---|---|---|
| Time | "Let's stay in touch" | A scheduled working session with an agenda |
| Reputation | "I know some people" | A named introduction sent this week |
| Money | "Send me pricing" | A deposit, a signed letter of intent, a paid pilot |

Score every meeting on the currency collected. "Tell me when you launch" is a polite decline and scores zero. "Can I buy the prototype" scores high. Rule: it is not a lead until you have given them a concrete chance to reject you.

### 6. Debrief within 24 hours, then decide

Same day, move notes somewhere searchable and tag each item: pain, goal, workaround, budget signal, obstacle, emotion. Record emotional intensity — anger and embarrassment predict spend; mild agreement does not. Decide as a batch, not per conversation:
- **Consistent problems and goals across 3–5 people in one segment** → stop interviewing, build the test.
- **Ten-plus conversations, still contradictory** → the segment is too broad. Slice and restart; do not add interviews.
- **Consistent problems, nobody spends a currency** → real annoyance, no budget. Find the version of this problem someone already pays to solve.

## Failure modes

**Interviewing your friends** — the roster is people who like you, owe you, or work near you. They give the answer that keeps things pleasant, and their enthusiasm is indistinguishable from demand. → At least half of any batch must have no prior relationship with you. If a friend is genuinely in the segment, have someone else run it, or stay strictly in the past tense so their goodwill has nothing to attach to.

**The leading question** — you describe the idea, then shape the question so agreement is the easy answer. The tell: their answer restates your framing in your own vocabulary. → Delay mentioning the idea as long as you can stand, and score your script beforehand. Any question describing your product gets cut or moved to the last five minutes.

**Collecting compliments** — the report says "great meeting, they loved it," and holds no number, date, or dollar figure. Praise costs nothing, so it is worth nothing. → Ban praise from write-ups. Every claim must attach to something that happened: an incident, a tool they pay for, a workaround.

**Talking to the wrong role** — the person who feels the pain has no budget, and the budget holder was never in the room. What you learned is true and unfundable. → Ask early: "Where would the money come from, and who signs?" Then get the signer into a later conversation. One hour with the economic buyer beats five with sympathetic users.

**Mistaking interest for commitment** — "I would definitely buy this" is the most expensive sentence in discovery: it reads as a purchase and is a prediction from someone with nothing at stake. → Convert it or discard it. Answer with an ask — a deposit, a letter of intent, a pilot date, an introduction to the buyer. What they do next is the data; what they said is not.

**Pitching under cover of research** — pushback appears and you start handling objections, reframing until they soften. You have turned a learning conversation into a sales call and won a false positive. → Treat lukewarm as information, not objection. Anyone will agree your idea is good if you are persistent enough; unless they are producing a check, persuading them corrupts the sample.

**Formality theater** — consent preambles, one-to-five scales, an hour block that costs four. Formality makes people perform, and performers flatter. → Ask the most important question in five minutes where they are.

## Outputs

1. A **segment statement** as a who-where pair, plus slicing questions if still too broad.
2. The **three learning questions**, with the uncomfortable one flagged.
3. An **interview script**: opening frame, past-tense sequence with probes, the two mandatory questions, close.
4. A **commitment ladder** — what counts as time, reputation, and money here, ranked.
5. For submitted notes, an **audit** flagging praise recorded as data, unanchored generalities, undug requests, missing incidents, and whether a commitment landed.
6. A **batch decision**: build, slice, or keep interviewing.

## Pairs with

- [`discovery/jobs-to-be-done`](../../discovery/jobs-to-be-done/SKILL.md) — converts clean incidents into a job statement and outcome metrics instead of a feature list.
- [`discovery/build-measure-learn`](../../discovery/build-measure-learn/SKILL.md) — interviews name the riskiest assumption; this settles it with behavior.
- [`discovery/venture-design`](../../discovery/venture-design/SKILL.md) — turns a validated segment into a beachhead choice, quantified value, and unit economics.
- [`revenue/value-messaging`](../../revenue/value-messaging/SKILL.md) — the phrasing customers use for their pain here is your messaging source text.

## Lineage

These rules descend from Rob Fitzpatrick's *The Mom Test*, which made the essential point that the defect is in your questions rather than in your customers' honesty: ask about their life instead of your idea, ask about the past instead of the future, talk less. Steve Blank's insistence that founders do this personally is assumed throughout.

This version departs by targeting operators who already have traction and can fool themselves more elaborately — so it weights the commitment ladder, the batch stop rule, and treating an unfundable role in the room as disqualifying rather than minor.
