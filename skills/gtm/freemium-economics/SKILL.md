---
name: freemium-economics
description: >-
  Decides whether to give something away, who pays for it, and where the line
  between free and paid should sit, using marginal cost to serve and a named
  cross-subsidy rather than optimism. Trigger when considering a free tier,
  trial, or free pilot, when a competitor launches something free, when free
  users are not converting, or when support costs from non-paying users climb.
domain: gtm
stage: gtm
lineage: "Chris Anderson — *Free: The Future of a Radical Price*"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Freemium Economics

> Free is not a hundred percent discount. It is a different market with different buyers, entered deliberately or not at all.

## The question this answers

- Should we have a free tier, and what exactly goes in it?
- A competitor made our core feature free. Do we match, or hold?
- Free users never upgrade. Is the tier too generous, or too useless?
- Free pilots keep stalling. Should we charge for them instead?

## When to run it

Run when serving one more non-paying user costs almost nothing, when the product improves as more people use it, or when a competitor's free offering is compressing conversion.

**Do not run this when** each additional user carries real marginal cost — onboarding, support hours, compute, per-account regulatory obligations. Free plus real cost to serve is a slow bleed disguised as growth. Do not run it with nothing else to sell; free without a named payer is charity with a roadmap. And never use free to compensate for weak distribution: giving away a product nobody has heard of produces the same silence as selling one, minus the revenue.

## The method

### Move 1 — Price the free user before you design the free tier

Compute the fully loaded annual cost of one non-paying user: infrastructure, support contacts, team attention, compliance obligations, sales time on people who will never buy. Founders count the first and ignore the rest, which is why free tiers surprise their owners in year two. Set it against gross profit per paying customer; the ratio sets the conversion rate you need to survive.

**Threshold:** if a hundred free users cost more than one paying customer's gross profit, you need better than one percent conversion to break even — roughly what an undesigned free tier delivers. Fix the cost side first.

### Move 2 — Name the payer before you name the tier

Every sustainable free offering has a payer. Name them in one sentence before designing anything.

| Route | Who pays | Fits when | Fails when |
|---|---|---|---|
| Paid upgrade | A minority of users | Cost to serve is near zero, value grows with use | The free tier ends the buyer's search |
| Third party | An advertiser or data buyer | Audience is large, attention monetizable | Users are few, or the data is regulated |
| Complement | Another product you sell | Free creates demand for the paid thing | The complement is easily substituted |
| Contribution | Users, in labor or content | Product improves as people use it | Participation stalls below critical mass |

If none of the four applies, do not launch. Write down the route and what must stay true for it to hold at ten times your current scale.

### Move 3 — Draw the line where it creates a reason, not a wall

The free tier delivers a complete win on a narrow slice of the problem and stops where the buyer's ambition begins. Four ways to draw it:

| Limit | Conversion behavior | Watch for |
|---|---|---|
| Time-boxed | Fast decisions, low cannibalization | Most never activate inside the window |
| Feature-boxed | Best conversion quality and reach | You maintain two products |
| Volume or seat | Simple; converts as the account grows | Users ration usage to stay under the line |
| Customer-type | Charges by ability to pay | Verification burden and gaming |

Feature limits work best when the free capability is genuinely useful and the paid one is what a serious user inevitably wants. Volume limits work when your value metric is already volume. Time limits are weakest for complex products: the clock runs during the exact period the user is too busy to evaluate.

**Threshold:** design toward roughly ten percent conversion from activated free users. Well below, the tier is too complete or attracting the wrong population; well above, you are withholding too much and losing reach.

Measure activated free users, not signups. A signup that never reached first value is a row in a table, and counting it corrupts every ratio downstream.

### Move 4 — Respect the gap between free and cheap

The distance between zero and the smallest non-zero price is the largest single step in your pricing. At zero the buyer evaluates nothing, risks nothing, needs no approval; at any positive price they do all three. A trivially priced tier therefore performs worse than either a free one or a properly priced one.

So never use a token price as a compromise. Either remove the price and accept the population it brings, or set one that funds service and screens for intent.

The counterweight: paying changes customer behavior. People use and complete what they pay for. Where results depend on the customer doing work, price is a commitment device, and free can be why your outcomes look worse than your product is.

### Move 5 — Decide in advance how you respond to free competition

Someone in your category will eventually give away what you charge for. Decide the response before it happens, because a response chosen in panic is always a discount.

Three legitimate moves. Match and monetize an adjacent layer, which requires already owning something adjacent. Hold price and make the quality gap larger than a hundred percent discount, which works only where the buyer bears real cost for failure. Or get there first: where the cost curve is falling, whoever makes it free captures the attention and the switching. The illegitimate move is quietly cutting price without changing the product — that concedes the comparison and funds nothing.

**B2B translation.** Consumer freemium logic transfers poorly above small-business price points. The free user is usually not the buyer, so the tier is a distribution mechanism aimed at practitioners who will later need budget — it must produce evidence a champion can carry upward, not just personal utility. Security review, procurement, and data residency arrive the moment usage goes departmental, so expect a wall only sales can pass, and staff that handoff. Free pilots are not freemium: an unpaid pilot has no sponsor with anything at stake, and completion rates show it. Charge for pilots, even nominally, with a written success criterion and a pre-agreed conversion price. And cost to serve here is human time, not infrastructure — a free tier that generates tickets costs far more than its consumer equivalent, so make it self-serve or do not offer it.

## Failure modes

**Free tier that ends the search** — it solves enough that upgrading has no trigger. The tell is high activation, long retention, near-zero conversion. → Move one capability the serious user needs behind the line. Retention on a free tier is not a success metric.

**Free tier that proves nothing** — so limited nobody reaches value, so no signal appears. The tell is high signups with almost no activation. → Widen until the free user gets a complete win on a narrow problem; that win makes the paid tier credible.

**Cost creep by a thousand tickets** — the free population grows and support becomes the largest line item. The tell is support headcount tracking free users, not paying ones. → Restrict support to paid tiers, move free users to community and docs, re-run Move 1 quarterly.

**The unpaid pilot** — enterprise trials that run long, stall, and end without a decision. The tell is a pilot extending past its end date with no executive sponsor. → Replace it with a paid pilot carrying a success criterion and an agreed conversion price.

**Signup vanity** — registrations get reported as growth while activated users stay flat. The tell is a headline number nobody can tie to revenue. → Report activated free users and conversion from activated; drop signups from the board deck.

**Panic matching** — a competitor goes free and price is cut within a week, with no change to product or model. The tell is a discount decided without naming who pays for it. → Use Move 5 instead.

## Outputs

- Fully loaded annual cost per free user, itemized, against gross profit per paying customer.
- A named cross-subsidy route in one sentence, with the condition that breaks it.
- The free/paid line: limit type, what sits on each side, why.
- The activation definition and the conversion target from activated users.
- A written response plan for a competitor going free.
- For B2B: paid-pilot structure, success criterion, conversion price.

## Pairs with

- [`gtm/pricing-power`](../../gtm/pricing-power/SKILL.md) — the paid tiers this feeds, and the value metric the limit should follow.
- [`strategy/business-model-design`](../../strategy/business-model-design/SKILL.md) — when the cross-subsidy question is really a model question.
- [`gtm/growth-loops`](../../gtm/growth-loops/SKILL.md) — how free users generate more users; without it, free is only cost.
- [`gtm/monetization-model`](../../gtm/monetization-model/SKILL.md) — what gets sold after the free user converts.

## Lineage

The framing comes from Chris Anderson's *Free: The Future of a Radical Price*: zero is a business model rather than a promotion, every instance of free is a cross-subsidy with an identifiable payer, and the psychological distance between zero and one cent is far larger than the arithmetic suggests. The behavioral evidence for that last point traces to Dan Ariely's work on zero as a decision anomaly.

This articulation departs in temperament. Anderson wrote while marginal costs were collapsing and free looked inevitable; practice since has shown cost to serve reappearing as support, compliance, and human attention, and that in business software the free user and the buyer are usually different people. So the method starts from the cost of a free user rather than the opportunity, and treats the enterprise free pilot as a failure mode rather than an entry point.
