---
name: deal-qualification
description: >-
  Scores an enterprise opportunity on the eight things that actually predict a
  close, finds the weakest one, and turns it into this week's action. Use when
  qualifying a deal, diagnosing a stalled opportunity, deciding whether to keep
  or kill it, running a pipeline review, building a forecast you have to defend,
  or testing whether a champion is real.
domain: revenue
stage: gtm
lineage: "Jack Napoli, Dick Dunkel & John McMahon (MEDDIC at PTC); Andy Whyte — *MEDDICC*"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Deal Qualification

> Most enterprise deals are not lost. They were never real, and it took two quarters to find out.

## The question this answers

- Is this opportunity real, or is it a well-attended conversation?
- What stage is it actually in, as opposed to the stage in the CRM?
- What single missing fact is holding this deal in place?
- Do I keep spending sales capacity here, or do I kill it and move on?

## When to run it

Run it when the deal is complex enough to lose slowly: multiple stakeholders, a
budget someone has to defend, a legal review, a cycle longer than six weeks.
Run it before every forecast commitment, and again the moment a deal goes quiet.

**Do not run this when** the sale is transactional, single-threaded by design,
or self-serve. A qualification framework applied to a two-call close adds
ceremony and subtracts speed. Also skip it for renewals where the only real
question is churn risk — that is an account health problem, not a qualification
problem.

## The method

### 1. Score the eight, honestly, in ten minutes

Eight dimensions. Score each 0–3: 0 = you have nothing, 1 = you have hearsay,
2 = you have it but with gaps, 3 = a named stakeholder ratified it.

| Code | Dimension | The one question |
|---|---|---|
| M | Value in currency | What is this worth to them in money, over what horizon? |
| E | Economic buyer | Who releases the budget without asking permission — and have you met them? |
| Dc | Decision criteria | What is the scorecard, and did you influence a line of it? |
| Dp | Decision process | What are the steps, dates, and gates between today and signature? |
| P | Paper process | Who signs, who reviews security, who onboards vendors, how long? |
| I | Pain and cost of inaction | What does doing nothing cost per month, and who said so? |
| C | Champion | Who argues for you in rooms you are not in? |
| Co | Competition | Who else, including doing nothing and building it internally? |

Total out of 24. Below 7, it is a lead. 7–12, you are still in discovery
regardless of what the CRM says. 13–18, qualified and in execution. 19+, you can
put it in a forecast you will not have to apologize for.

### 2. Ignore the total. Attack the weakest link

A deal at 18/24 with the economic buyer at 0 is dead and has not been told. The
score is a diagnostic, not a probability. The rule: your next action is always
the one that raises the lowest number. Write it as one sentence with an owner
and a date, or it did not happen.

### 3. Get the money into currency before anything else

Pain expressed in adjectives does not fund a project. Chain the question until
it lands on a number, then stop.

```
"Manual reconciliation" → so what?
→ "Three days a month" → so what?
→ "Team works overtime at close" → what does that cost?
→ "Roughly six figures a year in overtime and turnover" → and?
→ "It compresses operating margin, which the board is watching"
STOP. You now have money + strategy + someone's bonus.
```

If the customer has never done this math, they have never justified the project
internally, which means no one is defending it when budgets get cut.

### 4. Verify the champion instead of hoping

Champion, coach, and mobilizer are not synonyms, and the distinction is the
single largest source of slipped deals. Five yes/no questions:

1. In a closed room with the budget holder, do they argue your case?
2. Can they convene the economic buyer within five business days if you ask?
3. Is their personal outcome — promotion, bonus, reputation — tied to this?
4. Do they share sensitive process information before you ask for it?
5. Have they ever warned you about internal political risk?

Any "no" and you have a coach: useful for intelligence, useless for unblocking.
Coaches do not fail because they change their minds. They fail because you never
armed them. Give them the numbers, the one-paragraph recap of the business case,
and pre-written answers to the objections finance will raise.

### 5. Start the paper process before you need it

Legal review, security questionnaires, vendor onboarding, and procurement rules
run on their own calendar and do not care that you got a verbal yes. Ask for the
security questionnaire and the standard contract during evaluation, not after
the decision. This is the cheapest weeks-of-cycle-time you will ever buy.

### 6. Name the competitor you are actually losing to

Direct competitors are the visible ones and rarely the ones that beat you. The
real field: doing nothing, building it internally, and another project eating
the same budget line. "We have no competition" is not good news; it means you
have not found the alternative and it is winning by default.

### 7. Inspect, do not accept

In pipeline review, ask the eight questions per deal. If the rep cannot answer
six of eight with specifics, the deal is not at the stage it is reported at.
Move it back. Forecast categories should be gated on scores, not on tone of voice.

## Failure modes

**Champion-washing** — the rep calls someone a champion because that person is
warm, responsive, and pleasant. Tell: they have never once warned you about
internal risk. → Run the five-question test out loud in review. Downgrade to
coach and build a second thread.

**Economic buyer by proxy** — "my champion will take it to the CFO." Tell: you
cannot name the budget line or the last time the budget holder said anything.
→ Trade access for value: offer the buyer a business-case review, not a demo.
No access after two attempts is itself a qualification answer.

**Happy ears** — every signal is interpreted charitably; the deal has been three
weeks from closing for five months. Tell: the close date has moved twice and the
score has not changed. → Score movement, not date movement, is progress. A deal
whose score is flat for 30 days is stalled by definition.

**CRM theater** — the fields are filled in, the thinking never happened. Tell:
entries are labels ("CFO"), not evidence ("CFO confirmed on 14th that the risk
budget covers this"). → Require a name, a date, and a quote for any score of 3.

**Deferring paper** — "we will deal with legal once they decide." Tell: you have
never spoken to anyone in security or procurement. → Deals that are technically
won die here for a quarter. Parallelize from the proposal stage.

**Deal aging by politeness** — dead opportunities stay in the pipeline because
killing them is uncomfortable and makes coverage look thin. Tell: no
customer-initiated contact in 45 days. → Set an explicit kill rule. Capacity
returned to fresh pipeline outperforms hope.

**Qualifying instead of selling** — the framework becomes the work. Tell: long,
detailed scorecards on deals nobody has advanced in a month. → Qualification is
a ten-minute diagnostic that produces one action. If it takes an hour, you are
avoiding the customer.

## Outputs

- An eight-dimension score with a stated weakest link and one next action, owner,
  and date
- A one-paragraph business case in the customer's own words, with money in it
- A champion assessment (champion / mobilizer / coach) plus an enablement pack:
  numbers, recap, pre-answered objections
- A mutual action plan: steps to signature with owners, dates, and done-criteria
- A competitive map that names doing nothing and building internally
- A pipeline audit: percentage of pipeline above the qualification gate, and what
  should be killed this week

## Pairs with

- [`revenue/value-messaging`](../../revenue/value-messaging/SKILL.md) — qualification tells you where the gap
  is; value messaging gives you the language to close it
- [`revenue/enterprise-negotiation`](../../revenue/enterprise-negotiation/SKILL.md) — for the internal politics that
  determine the real decision process
- [`revenue/challenger-selling`](../../revenue/challenger-selling/SKILL.md) — the posture that creates the
  urgency qualification keeps measuring
- [`gtm/gtm-measurement`](../../gtm/gtm-measurement/SKILL.md) — for turning deal scores into forecast
  accuracy and cycle-time instrumentation

## Lineage

The underlying discipline was built by Jack Napoli, Dick Dunkel, and John McMahon
at PTC in the 1990s as MEDDIC, and formalized for a modern audience by Andy Whyte
in *MEDDICC*, which added the distinction between champion, coach, and mobilizer
and pushed the field from identifying pain to implicating it. Later practice
added the paper process as its own dimension once enterprise procurement grew
teeth. Where this articulation departs: the original tradition treats the
elements as a checklist to complete, and most teams implement it as CRM fields.
I treat the total score as nearly irrelevant and the weakest link as the entire
point — a qualification pass that does not end in one named action with a date
has produced documentation, not progress.
