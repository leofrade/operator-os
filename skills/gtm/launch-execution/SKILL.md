---
name: launch-execution
description: >-
  Turns a launch date into a sequenced operation with entry gates, a named
  primary surface, a recruited support group, and a go/no-go bug bar. Trigger
  when planning a product, feature, pricing, or vertical launch, when writing a
  press release or media kit, when preparing a marketplace or community launch,
  when deciding whether the product is ready to ship publicly, or when running
  the post-launch retrospective.
domain: gtm
stage: gtm
lineage: "Colin Bryar & Bill Carr — *Working Backwards* (Amazon's PR/FAQ method); Jakob Nielsen — *Why You Only Need to Test with 5 Users*; Maja Voje — *GTM Strategist*"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Launch Execution

> A launch is not an announcement. It is a scheduled, public test of your distribution assumptions, and most teams run it without stating the assumption.

## The question this answers

- We ship in three weeks. What actually has to be true on the day, and who owns each piece?
- Is this a launch, or a deploy with a blog post attached?
- Which surface do we launch on, given that our buyer may not be on the one everybody talks about?
- The launch underperformed. Was that the product, the offer, or the distribution?

## When to run it

Run this when there is a dated, publicly irreversible moment: a new product, a new segment, a new pricing tier, a marketplace listing, a category claim. Run it when at least ten people outside the company have used the thing and can describe it without a script. Run it when one person owns the single number the launch is supposed to move.

**Do not run this when** activation is broken. A launch amplifies whatever exists — if new users cannot reach value on their own, the launch converts strangers into churned users and spends a list you can only spend once. Fix time-to-value first. **Do not run this when** the release is a feature for existing customers; that needs an in-app note and a changelog, not an operation. **Do not run this when** nobody can name the metric. "Awareness" is not a metric. If the honest answer is "we want to feel like we shipped," ship quietly and keep the powder dry.

## The method

### Move 1 — Write the announcement before you commit the date

Write the external press release first, one page, in customer language. Headline, the change in the buyer's life, how it works, availability, price. No feature list.

Then write the hostile FAQ: fifteen questions from a skeptical buyer, including the ones you would rather skip — what did you deliberately not build, when is this the wrong tool, why should anyone trust a new company with this data, what happens on cancellation, who else in my industry uses it.

Decision rule: hand the page to three people outside the team. If two can restate who it is for and what changes, pass. If more than three FAQ questions have no answer, the date moves — you have a positioning problem, and no launch tactic fixes positioning.

### Move 2 — Choose one primary surface, one supporting

| Surface | What it actually buys | When it is the wrong choice |
|---|---|---|
| Community/marketplace launch | Awareness with early adopters, a reusable badge, a burst of unfiltered feedback | Your buyer is a director in a regulated industry who has never visited the site |
| Lifetime-deal marketplace | Cash in 30-60 days and hundreds of paying critics | Cost to serve is high, or you sell annual contracts the deal cannibalizes |
| Press and analyst outreach | Third-party credibility you cannot self-assert | You have no genuinely new fact — a launch alone is not news |
| Owned list plus direct outreach | Conversion, not reach | Never wrong; it is the floor, not the strategy |
| Founder-led content | Compounding inbound over quarters | Treated as a launch-day lever; it is a 90-day instrument |

Rule: one primary, one supporting, everything else is a repost. Teams that pick four surfaces execute none at the depth that produces a result, then conclude the market was not ready.

### Move 3 — Recruit the alliance, ask each person for exactly one action

Thirty to eighty people, invited individually, never in a batch. Core team, then beta customers and advisors, then the wider network of ex-colleagues, community contacts, and partners.

The ask is one action at one named hour: open the link, look for five minutes, leave an honest comment. Ask for honesty, not praise — a thread of superlatives reads as staged to exactly the audience you want to convince.

Threshold: if fewer than 60% confirm in writing seven days out, you do not have enough concentrated attention to clear the noise floor. Shrink the ambition, move the date, or accept a quiet launch on purpose.

### Move 4 — Break it before strangers do

Two sessions, both before the date.

Five usability tests with people who match the buyer profile and have never seen the product. Nielsen's finding holds in practice: five sessions surface most usability defects, and returns fall off sharply after that. Give tasks, not instructions. Say nothing when they stall — a sixty-second stall is data, and helping destroys it.

One two-hour exploratory bug hunt on staging with three to eight people, including two non-engineers, who find the paths engineers never take.

| Severity | Example | Decision |
|---|---|---|
| Critical | Data loss, payment failure, signup or login blocked | Blocks the launch |
| High | Core path broken, unreadable on mobile, wrong pricing shown | Fix before |
| Medium | Secondary feature inconsistent | Fix in week one |
| Low | Cosmetic, rare edge case | Backlog |

Only Critical and High move the date. Everything else ships alongside a published known-issues list, which is cheaper and more credible than a slipped date.

### Move 5 — Run the day on a clock

Written run-of-show with owners and timestamps: who publishes, who posts first, who triggers the alliance, who answers comments, who watches the funnel, who can roll back. Every comment answered within six hours — response rate in the opening window is the strongest lever you control on the day.

### Move 6 — Retrospective within 72 hours, numbers before opinions

Twenty minutes on data with no interpretation: target versus actual per metric, which surface converted, the largest drop-off point, the most repeated comment. Then what worked and what did not, facts only, blame out of scope. Close with four decisions: what changes this week, what becomes next sprint's experiment, what is abandoned, and the one metric that owns the next 30 days. Written and dated, or it did not happen.

## Failure modes

**The silent launch** — you go live and nothing happens, because the alliance was never asked and the list was never warmed. The tell is a launch plan whose distribution section is a list of channels rather than a list of named people with confirmed times. → Distribution on launch day is people, not platforms. Book the humans first.

**Vanity surface** — the team launches on the platform founders read about rather than where the buyer lives, then reads a badge as market validation while pipeline stays flat. The tell: strong upvotes, no qualified conversations. → Choose the surface by where the economic buyer already spends attention, and accept that it may be an industry association mailing list rather than a tech community.

**Feature-list press release** — the announcement enumerates capabilities because the team could not agree on a single claim. The tell: the headline contains "and". → Cut to one claim. If two claims cannot be dropped, you are launching two products.

**Deadline laundering** — the launch date is used to force scope decisions nobody wants to make, so the day is spent shipping rather than selling. The tell: engineering merges on launch morning. → Feature freeze at seven days, code freeze at 48 hours, and the launch team spends the day on distribution.

**Testing with friends** — usability testers are people who like you, so every stall is politely explained away and the sessions produce no defects. The tell: a test session with zero moments of confusion. → Recruit from leads that never converted; they know the problem and owe you nothing.

**Retro theater** — the meeting happens, feelings are shared, and no decision is written down, so the same mistakes appear at the next launch. The tell: no owner and no date next to any line. → No line leaves the room without a name and a date.

## Outputs

- One-page external press release plus a fifteen-question hostile FAQ with answers
- Surface decision with a one-paragraph rationale, primary and supporting
- Launch alliance roster with the specific ask and confirmation status per person
- Announcement asset pack: headline variants, short description, screenshots, demo outline, first comment
- Usability findings with severity-ranked defects and the go/no-go call
- Run-of-show for launch day with owners and timestamps
- Retrospective document: target versus actual, three keeps, three fixes, dated decisions, next 30-day metric

## Pairs with

- [`gtm/gtm-measurement`](../../gtm/gtm-measurement/SKILL.md) — instrument before the launch, not after; a launch with no tracking plan generates a story instead of data
- [`revenue/value-messaging`](../../revenue/value-messaging/SKILL.md) — the claim in the press release must be the claim in the sales call
- [`brand/positioning`](../../brand/positioning/SKILL.md) — if move 1 fails, the problem is upstream of the launch
- [`discovery/experiment-design`](../../discovery/experiment-design/SKILL.md) — for the post-launch fixes that should be run as tests rather than opinions

## Lineage

The press-release-first discipline is Amazon's, documented by Colin Bryar and Bill Carr in *Working Backwards*; the five-user rule for usability testing is Jakob Nielsen's, from the Nielsen Norman Group's research on defect discovery curves; the launch-checklist tradition owes much to Maja Voje's *GTM Strategist*. Where this articulation departs: those sources treat the artifacts as deliverables, and this treats them as gates — the press release is a kill switch on the date, and the bug bar is a contract that only two severity classes are allowed to move a launch. The surface-selection table and the 60%-confirmation threshold on the alliance are operating rules from running launches where the buyer was nowhere near the channel the team wanted to use.
