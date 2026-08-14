---
name: platform-thinking
description: >-
  Decides whether to open a product into a platform, what control that costs, and which
  half of the business you keep. Use when customers are already extending your product
  without permission, when your roadmap cannot absorb the long tail of requests, when a
  partner asks for API access, when growth from your own build is decelerating, or when
  someone proposes "becoming a platform" without naming what changes.
domain: strategy
stage: scale
lineage: "Geoffrey Parker, Marshall Van Alstyne & Sangeet Paul Choudary — *Platform Revolution*; Andrew Chen — *The Cold Start Problem*; Thomas Eisenmann, Geoffrey Parker & Marshall Van Alstyne — platform strategy research (HBR); Jeff Jarvis — *What Would Google Do?*"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Platform Thinking

> Becoming a platform means giving up control of the part you are proudest of. It only pays if other people's work makes your product more valuable than your own work would have.

## The question this answers

- Should we open this up, or is "platform" the word we are using to avoid funding the roadmap?
- What exactly are we giving up control of, and what do we get for it?
- Which margin are we defending that the market has already stopped paying for?
- Where are customers already assembling a solution we could be the foundation of?

## When to run it

Run it when customers are visibly working around you — exporting data weekly, paying consultants to bolt things on, running unofficial integrations you did not sanction. Run it when the backlog is full of requests that are individually reasonable and collectively unfundable. Run it when a serious partner asks for API access and you do not have a policy.

**Do not run this when** nobody is extending your product yet. Platform ambition ahead of platform demand produces an SDK with a launch blog post and no builders. Do not run it when your differentiation is the last mile itself: if the value is in the integrated experience, opening it turns you into a component with component margins. And do not run it as a substitute for distribution — a platform without users is a hobby with documentation.

## The method

**Move 1 — Prove the demand before you build the surface.**

Rank the evidence, strongest first:

1. Customers paying third parties to extend your product. This is money already leaving for a job you could do.
2. Unofficial integrations that exist without your help or approval.
3. Export behavior: what share of accounts pull data out monthly, and what they do with it downstream.
4. Feature requests you have declined repeatedly as too niche. Count them, group them, and look at how many are the same shape.

Threshold: if you cannot name ten organizations that built something on top of you without permission, you do not have platform demand. You have a roadmap you do not want to fund, and opening an API will not change that.

**Move 2 — Price the control you are giving up.**

List it explicitly: the last-mile experience, the direct customer relationship, pricing power over the extended surface, freedom to change the data model, and support load from other people's defects.

Then answer the extraction question: what is the least you can take per transaction, install, or builder while still covering the cost of running the platform? Take less than the market would bear. The objective is participant volume, not margin per participant. If the business case requires a heavy take rate in year one, you are building a toll booth, and participants will route around toll booths as soon as an alternative exists.

Test it: model the platform at ten times the participants and one third of the take rate. If that scenario is not clearly better than today, do not open.

**Move 3 — Split core from edge, and be honest about which side compounds.**

Keep what improves with aggregate usage: matching, settlement, identity, trust, cross-customer data with a feedback loop. Give away what is specific to one customer's context: workflow configuration, reporting, vertical logic, last-mile interface.

The failure test: if the thing you kept does not get measurably better as participants grow, you are not running a platform. You are running an outsourcing arrangement in which other people capture the increasing returns.

**Move 4 — Solve the cold start in one bounded market.**

For a two-sided model, name the hard side and subsidize it deliberately, with a budget and an end date rather than an open-ended discount. Then define critical mass locally instead of globally: the smallest bounded market — one vertical, one region, one large customer's ecosystem — where both sides are dense enough to transact.

Set the density metric before launch. Something like: for the median active customer, at least three available extensions covering their top workflows. Below that threshold, do not market the platform. An empty marketplace is worse than no marketplace, because it is public evidence that nobody showed up.

**Move 5 — Ship in visible increments, and publish the rules that protect builders.**

Release early and label it as such, but pair that with the thing builders actually price in: a written breaking-change and deprecation policy, published before the first external integration exists. A platform's reputation is set by how fast and how honestly it responds when it breaks someone, not by whether it ever breaks them.

Track one number as the health metric: time from a builder signing up to their first working call in production. Measure it in hours. When it moves to weeks, something in your approval process is adding ceremony rather than quality.

**Move 6 — Decide in writing when you will compete with your own ecosystem.**

Every platform eventually builds something a participant already sells. Write the boundary before you need it: which categories you will build, which you will buy, which you will leave alone. Ambiguity here is what makes ecosystems quietly stop investing — long before anyone complains publicly.

## Failure modes

**Platform as a synonym for API** — the plan has SDK milestones and no line for partner economics. The tell: no builder can explain how they make money. → A platform is a business model. If the builder's P&L does not close, you shipped an integration.

**Opening the wrong half** — giving away the aggregating asset and keeping the interface. The tell: competitors now use your data to serve your customers better than you do. → Keep what compounds with usage; give away what is context-specific.

**Extracting too early** — a take rate reverse-engineered from this year's plan. → Run the ten-times-participants, one-third-rate model. A low rate you never raise beats a high rate participants design around.

**The empty marketplace launch** — announced with a handful of logos and no density inside any single customer's use case. → Reach the density threshold in one bounded market first, then announce.

**Competing quietly with participants** — building the top three partner applications yourself while telling partners you will not. The tell: partners stop shipping new features against your API and nobody has said why. → Publish the boundary and hold it. If you must cross it, acquire rather than clone.

**Breaking changes by announcement** — versioning without a deprecation window, and support tickets arriving from other people's customers. → Write the policy before the first external build, then honor it even when it is expensive.

**Control theater** — a certification and review process that adds weeks and no measurable quality. The tell: signup-to-first-call measured in weeks. → Track that number as a core metric and cut the steps that do not change defect rates.

**Openness as a values exercise** — publishing data, roadmaps, and blog posts without changing who captures value. → Openness is a means. If it does not change the economics or the growth loop, it is marketing, and should be budgeted as marketing.

## Outputs

- A demand dossier: named organizations already extending you, export behavior, and grouped declined requests
- An explicit list of the control being traded away, with the support and roadmap cost of each item
- The extraction model at ten times participants and one third of the take rate, with a go or no-go
- A core/edge split naming the asset that compounds with participant growth
- A bounded first market with a density threshold and a subsidy budget with an end date
- A published deprecation policy and a written competition boundary with the ecosystem

## Pairs with

- [`strategy/business-model-design`](../../strategy/business-model-design/SKILL.md) — the two-sided shift, its preconditions, and where the revenue mechanism has to change
- [`gtm/pricing-power`](../../gtm/pricing-power/SKILL.md) — sets the take rate against what participants will actually tolerate
- [`strategy/value-innovation`](../../strategy/value-innovation/SKILL.md) — what you keep at the core has to be worth keeping on its own curve
- [`strategy/scaling-playbook`](../../strategy/scaling-playbook/SKILL.md) — the operating load of supporting builders alongside customers

## Lineage

The economics here are Geoffrey Parker, Marshall Van Alstyne and Sangeet Paul Choudary's, in *Platform Revolution*: the core interaction, the pipe-to-platform inversion, the argument that a platform's job is to keep the cost of participation low enough that volume arrives, and the governance question of when the platform competes with what it hosts. Thomas Eisenmann, with Parker and Van Alstyne, supplied the earlier strategy research in HBR on two-sided network pricing — which side to subsidize and which to charge, and why subsidizing the wrong one is unrecoverable. The vocabulary of the hard side and the cold start is Andrew Chen's, from *The Cold Start Problem*, as is the insight that critical mass is local rather than global: density inside one bounded market beats thin coverage everywhere. Jeff Jarvis's *What Would Google Do?* popularized the surrounding instincts early — link rather than build, extract the minimum, treat customers as collaborators — but it argues a worldview, not an economics.

Where this articulation departs: the platform literature is written from the winners, so it explains how successful platforms work and understates how many products should never open at all. This version gates on evidence before design — ten named organizations already building on you, or you do not have platform demand — prices the control being traded away as a line item, forces an explicit core-versus-edge decision with a compounding test, and requires the competition boundary with your own ecosystem to be written down before it is needed rather than litigated after.
