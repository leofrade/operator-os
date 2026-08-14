---
name: chasm-crossing
description: >-
  Selects and defends the single beachhead segment that converts early-adopter
  traction into repeatable mainstream revenue, using a funding test and an
  adjacency test rather than intuition. Trigger when early sales have stalled
  despite enthusiastic first customers, when every deal still requires custom
  scope, when choosing which vertical to concentrate on, when pragmatic buyers
  keep asking who else in their industry uses this, or when the team is
  spreading across too many segments at once.
domain: gtm
stage: gtm
lineage: "Geoffrey A. Moore — *Crossing the Chasm*"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Chasm Crossing

> Choosing a beachhead is a capital allocation decision, not a focus exercise: you are betting that dominating one small market produces enough money and enough proof to buy the next one.

## The question this answers

- Ten happy customers, flat growth. Sales problem or segment problem?
- Which of the segments we could serve do we commit to for eighteen months?
- How small is too small, and how do I know before burning a year finding out?
- We won the segment. Why did the win not travel to the adjacent one?

## When to run it

Run this when early revenue arrived through relationships, enthusiasm, and custom scope, and the next tier of buyers is asking what the first tier never did: who else like me is using this. Run it when the pipeline looks full and conversion has collapsed, or when the team keeps resolving "which vertical" to "both."

**Do not run this when** you have fewer than five customers who paid real money and still use the product; selection with no reference data is guessing with extra steps. **Do not run this when** the product spreads on its own mechanics rather than on peer reference — use [`gtm/growth-loops`](../../gtm/growth-loops/SKILL.md) instead. **Do not run this when** runway is under six months; this pays out over four to six quarters.

## The method

### Move 1 — Establish which side of the gap you are actually on

Count, do not intuit. Of the deals closed in the last two quarters, how many closed on the same three reasons, with the same buyer title, no bespoke scope, and no founder in the close?

| Count | Reading | Implication |
|---|---|---|
| 0-2 | Pre-chasm regardless of revenue size | Selection is the priority; scaling headcount now burns cash |
| 3-5 | You have a candidate beachhead, possibly by accident | Formalize it; do not go looking for a better one |
| 6+ | You have crossed within that segment | Move to expansion sequencing, not selection |

Revenue is not the signal. Substantial revenue from a handful of bespoke deals is further from crossing than a dozen identical small ones.

### Move 2 — Define candidates as buyer × trigger × cost of inaction

An industry is not a segment. "Logistics" is a directory category. A beachhead is a specific buyer title, hitting a specific trigger, already paying a quantifiable cost for the failure you remove.

```
CANDIDATE
Buyer title:        [who signs and who feels the pain — both]
Trigger event:      [what just happened that makes this urgent now]
Current cost:       [money, headcount, penalty, or risk absorbed today]
Today's workaround: [manual process, incumbent, consultant, or nothing]
Whole product gap:  [what they need beyond your core]
Reachable accounts: [how many you can name]
Peer network:       [where these buyers talk]
```

If you cannot name the peer network, disqualify the candidate. Mainstream buyers adopt on each other's evidence, not yours. A segment with no association, conference, shared channel, or gossip has no transmission medium, and references die where they are made.

### Move 3 — Apply the funding test

Most teams skip this move, and skipping it produces the method's most expensive failure: winning a segment that cannot pay for the next campaign.

```
Capture value = reachable accounts × realistic annual contract value × attainable share

Attainable share: 0.3 to 0.5 is aggressive but real for a focused team
in a segment of 20 to 200 named accounts over 18 months.
```

Two thresholds, both hard:

- **Floor.** Capture value must exceed roughly twice the fully loaded annual cost of the team required to win it. Below that you bought a job, not a beachhead. The segment's purpose is to fund the next invasion.
- **Ceiling on smallness.** Under about twenty reachable accounts, word of mouth has nowhere to travel. You exhaust the pipeline before the whole product is finished, and that gap is where teams panic and abandon the strategy.

If a candidate fails the floor, widen the trigger, not the industry. The same buyer title with a broader triggering condition keeps the peer network intact; a second industry destroys it.

### Move 4 — Apply the adjacency test

Score where the beachhead leads before committing.

| Test | Pass condition | Failure meaning |
|---|---|---|
| Whole-product carryover | The next segment reuses 70%+ of what you build for this one | Below 50%, the second segment is a second company |
| Buyer-network separation | The next segment has a different peer network but a recognizable adjacent one | Same network means it was never a second segment, just more of the first |
| Defensibility of the win | You win structurally — regulatory depth, workflow lock, data accumulation, integration position | Winning on being first or faster means an incumbent closes the gap in two quarters and keeps the account |

Defensibility is where beachheads fail quietly. Teams pick the segment their network reaches most easily, which is often one an incumbent already holds and is merely inattentive to: you win the pilot on speed and lose the renewal on bundled price. Choose where the incumbent's own economics stop them from following — too small for their sales model, too regulated for their roadmap, too specific for their platform.

### Move 5 — Close the whole-product gap for exactly one segment

List everything the buyer needs beyond your core to succeed, then give each gap an owner: you, a contracted partner, or the customer. A partner named in a slide and not in a contract is an unowned gap.

Rule: if the gaps cannot close in three to six months, you picked the wrong segment. Revisit move 3 rather than extending the timeline — a mainstream buyer who evaluates you before the whole product exists is a reference permanently lost.

### Move 6 — Manufacture three to five peer references, then expand on a trigger

Success is not revenue; it is named, callable, same-industry references. Instrument it: what share of new deals cite a peer you can name. Below 30%, keep concentrating. Above 50%, the segment sells itself and you may open the adjacent one — one, on a date, with the same discipline.

## Failure modes

**The beachhead that cannot fund the next one** — you dominate a segment whose capture value is smaller than the team that captured it, and the strategy stalls with nothing to reinvest. The tell: capture value under two times go-to-market cost, or a board conversation about how to grow after "winning." → Re-run move 3 before committing; widen the trigger while holding the buyer title constant.

**The adjacent beachhead you cannot defend** — you pick the segment nearest your network, which sits inside a large incumbent's installed base. Pilots close fast; renewals do not. The tell: every deal has an incumbent in the account and your win reason is speed or price. → Select where the incumbent's economics prevent a response, not where your relationships are warmest.

**Segment as industry** — the beachhead is a sector name, so messaging stays generic, the whole product is never finished for anyone, and references do not compound. The tell: no buyer title and no trigger in the definition. → Rewrite as buyer × trigger × cost of inaction and verify the peer network exists.

**Pilot purgatory** — pragmatic buyers use unfunded pilots to defer commitment, and the team reads the pilot roster as pipeline. The tell: no success criteria, no budget line, no dated decision. → Refuse them. A pilot that costs the buyer nothing teaches you nothing.

**Abandoning at month nine** — concentrated work shows little for two or three quarters, patience fails, the team switches, and the reference clock resets to zero. The tell: a segment change proposed with no new data, only fatigue. → Gate the review on reference share, not elapsed time. Under 30% peer citation after four quarters is evidence; impatience is not.

**Two beachheads to make the market look bigger** — a conversation about total addressable market converts one committed segment into two hedged ones, both under-resourced. The tell: two segments in the plan, each with less than a full team. → Commit to one in execution and put the sequence in the narrative. Sequencing is the expansion story; hedging is not.

## Outputs

- Position diagnosis: repeatable-close count with the evidence behind it
- Three to five candidates in buyer × trigger × cost format, each with a named peer network
- Funding test per candidate: reachable accounts, ACV, attainable share, capture value against go-to-market cost
- Adjacency map of the second and third segments with carryover estimates
- Whole-product gap table with a contracted owner and date per gap
- Positioning statement for the pragmatic buyer, anchored on today's workaround
- Reference plan: first five target accounts and the peer-citation metric with its review gate

## Pairs with

- [`brand/positioning`](../../brand/positioning/SKILL.md) — the beachhead determines the positioning statement, not the reverse
- [`revenue/deal-qualification`](../../revenue/deal-qualification/SKILL.md) — the pilot discipline that keeps segment focus honest
- [`gtm/lead-engine`](../../gtm/lead-engine/SKILL.md) — concentrated demand generation inside one peer network
- [`strategy/value-innovation`](../../strategy/value-innovation/SKILL.md) — when no candidate passes the defensibility test, the offer is the problem

## Lineage

The chasm, the adoption psychographics, the beachhead metaphor, and the whole-product concept are Geoffrey A. Moore's, from *Crossing the Chasm*. His durable insight is that early adopters and pragmatic buyers do not serve as references for each other, which makes the gap structural rather than a matter of sales effort. Where this departs: Moore's selection criteria are qualitative and scenario-based, and this replaces them with two quantitative gates — a funding test requiring the beachhead to pay for the next campaign, and an adjacency test requiring the win to be structurally defensible rather than merely first. The failure I see most is not weak focus, but focus applied to a segment too small to fund the sequel or too close to an incumbent to hold.
