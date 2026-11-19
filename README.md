<div align="center">

# Operator OS

**The business half of an AI-native founder's toolkit.**

45 executable skills for Claude Code, Claude, Cursor, and any agent that reads Markdown —
covering discovery, strategy, go-to-market, enterprise sales, operations, and brand.

[![Skills](https://img.shields.io/badge/skills-45-0d1117?style=flat-square)](#the-library)
[![Domains](https://img.shields.io/badge/domains-6-0d1117?style=flat-square)](#the-library)
[![License](https://img.shields.io/badge/docs-CC--BY--4.0-0d1117?style=flat-square)](LICENSE)
[![Format](https://img.shields.io/badge/format-SKILL.md-0d1117?style=flat-square)](#anatomy-of-a-skill)

</div>

---

## Why this exists

Coding agents got good fast because engineering knowledge is written down, structured, and
close to the model. Business knowledge is not. It sits in books nobody rereads, in decks,
and in the heads of people who have run the play.

So the agent writes your migration script correctly and then tells you to "leverage your
unique value proposition."

This repository is the missing half. Every file is a **decision procedure** — the sequence
an operator actually runs, with the thresholds that say whether a move worked and the
failure modes that say when to stop. Not summaries. Not prompts. Procedures.

I am partner at two startup studios — one focused on blockchain, one on AI — plus two
board seats. Somewhere around a dozen ventures at different stages, most with founders who
are not me. These are the files I use to hold that surface area without a chief of staff.

## What this is not

- **Not book summaries.** A condensed business book is worth nothing now — any model does
  that on request. What is scarce is the judgment layer: what to skip, what threshold means
  stop, what the framework's author was wrong about. That is what these files contain.
- **Not neutral.** Several skills argue with their own source. `strategy/enduring-company`
  opens by discounting the evidence base of the book it descends from.
  `brand/purpose-narrative` states plainly that the Golden Circle is unfalsifiable.
  `strategy/blitzscaling` leads with the precondition test that makes blitzscaling
  something other than arson.
- **Not a prompt collection.** No "act as a world-class CMO." These are structured
  procedures with entry conditions, exit criteria, and named anti-patterns.

## Install

### Claude Code

```bash
git clone https://github.com/leofrade/operator-os.git
mkdir -p ~/.claude/skills
cp -R operator-os/skills/*/* ~/.claude/skills/
```

Skills load by description. Ask a normal question — "our win rate collapsed in enterprise
deals this quarter" — and the matching skill activates.

Project-scoped instead of global:

```bash
mkdir -p .claude/skills
cp -R operator-os/skills/*/* .claude/skills/
```

Both commands flatten the six domain folders into 45 skill folders, which is the layout
agents expect. One consequence worth knowing: the relative paths in each file's
**Pairs with** section stop resolving as links once flattened. The names still do their
job — every entry is written as `domain/skill-name`, so the agent can find the sibling —
and the links resolve normally when you browse the repo here.

To keep the domain structure for reading or for tools that recurse:

```bash
cp -R operator-os/skills ~/operator-os-skills
```

### Claude (web and desktop)

Zip any skill folder and upload it in **Settings → Capabilities → Skills**.

```bash
cd operator-os/skills/revenue/deal-qualification && zip -r ../deal-qualification.zip .
```

### Cursor, Windsurf, and other agents

`SKILL.md` files are plain Markdown with YAML frontmatter. Point your rules or context
config at the folder, or paste a single file into the conversation. Nothing here depends
on a runtime.

### Just reading them

Every file is legible on its own. Start with
[`brand/positioning`](skills/brand/positioning/SKILL.md) or
[`revenue/deal-qualification`](skills/revenue/deal-qualification/SKILL.md).

## Anatomy of a skill

Every file follows the same seven-part shape, which is what makes them composable and
what makes an agent able to route to the right one.

```
The question this answers   Real questions an operator asks out loud — not topics.
When to run it              Entry conditions, plus an explicit "do not run this when."
The method                  3-7 numbered moves. Each has a decision rule or threshold.
Failure modes               Named traps, the tell, and the correction.
Outputs                     The concrete artifacts a run should produce.
Pairs with                  Cross-links, because no decision is made in isolation.
Lineage                     Credit to the originators, and where this departs from them.
```

The two sections that carry the weight are **the thresholds** and **the failure modes**.
A framework without a number that says "stop" is a diagram. A framework without failure
modes is somebody else's success story.

Example, from [`brand/positioning`](skills/brand/positioning/SKILL.md):

```
1. A rep says it unprompted in the first five minutes of discovery.
2. It caused at least one deliberate disqualification this quarter.
3. It changed a roadmap, pricing, or hiring decision within 90 days.
4. A customer restated it accurately to a peer without your materials.
5. It names something you intend to lose to.

5/5  load-bearing — leave it alone for four quarters
3-4  partially adopted — fix rollout and enablement, not the statement
0-2  slogan — return to Move 1; it was written to be approved, not used
```

## The library

45 skills across six domains. Stage tags: `pre-pmf`, `gtm`, `scale`, `any`.

### Discovery — before you have product/market fit

| Skill | What it decides | Lineage |
|---|---|---|
| [`build-measure-learn`](skills/discovery/build-measure-learn/SKILL.md) | Runs the learning loop at company level: how long a full cycle takes, what an MVP is and is not, how to account for progress before revenue exists, and when to pivot the venture | Eric Ries — The Lean Startup; Steve Blank — customer development |
| [`customer-development`](skills/discovery/customer-development/SKILL.md) | Sequences a company through four gated stages — discovery, validation, demand creation, and organizational build — so nobody scales a sales motion that has not been proven | Steve Blank — The Four Steps to the Epiphany |
| [`customer-interviews`](skills/discovery/customer-interviews/SKILL.md) | Runs discovery conversations that produce evidence instead of encouragement, by forcing past-tense specifics, neutralizing praise, and closing for a real commitment | Rob Fitzpatrick — The Mom Test |
| [`engagement-ethics`](skills/discovery/engagement-ethics/SKILL.md) | A design-review instrument for auditing your own product's retention mechanics: where engagement stops creating value and starts extracting it, and what to do when the growth metric and the user's interest point in opposite directions | Natasha Dow Schüll — Addiction by Design; Nir Eyal — Hooked (as counterpoint) |
| [`experiment-design`](skills/discovery/experiment-design/SKILL.md) | Turns a business assumption into a test that can actually fail, with the kill number written down before the test runs | David Bland & Alexander Osterwalder — Testing Business Ideas |
| [`founder-patterns`](skills/discovery/founder-patterns/SKILL.md) | Runs a founder's actual situation against the structural patterns that recur in early-stage company histories — pivot signals, cofounder failure correlation, where distribution really came from, timing | Jessica Livingston — Founders at Work |
| [`jobs-to-be-done`](skills/discovery/jobs-to-be-done/SKILL.md) | Converts messy customer conversations into a stable job statement and a ranked set of outcome metrics, using the cheap subset of outcome-driven innovation that a team without a research budget can actually run | Anthony Ulwick — Jobs to Be Done: Theory to Practice; Clayton Christensen — Competing Against Luck |
| [`venture-design`](skills/discovery/venture-design/SKILL.md) | Reduces a new venture to the five decisions that actually gate progress — beachhead, quantified value, buying process, unit economics, and a paid minimum product — and names which classroom steps a bootstrapped team should skip | Bill Aulet — Disciplined Entrepreneurship |

### Strategy — what game you are playing

| Skill | What it decides | Lineage |
|---|---|---|
| [`blitzscaling`](skills/strategy/blitzscaling/SKILL.md) | Decides whether to trade capital efficiency for speed, then runs the campaign if the answer is yes | Reid Hoffman & Chris Yeh — Blitzscaling |
| [`business-model-design`](skills/strategy/business-model-design/SKILL.md) | Turns a business model canvas from a documentation exercise into a diagnostic: which blocks carry weight at your stage, which are invention, and where the joints between them break | Alexander Osterwalder & Yves Pigneur — Business Model Generation |
| [`disruption-radar`](skills/strategy/disruption-radar/SKILL.md) | Separates genuine low-end and new-market disruption from ordinary competition, then picks the organizational container that can respond to it | Clayton Christensen — The Innovator's Dilemma |
| [`enduring-company`](skills/strategy/enduring-company/SKILL.md) | Builds the disciplines that let a company compound for a decade — leadership selection, honest information flow, ruthless focus — while discounting the research that made those disciplines famous | Jim Collins — Good to Great |
| [`monopoly-thesis`](skills/strategy/monopoly-thesis/SKILL.md) | A scored self-assessment that tells a founder whether a venture can own a market or is a better version of something that already exists, and whether it is fundable yet | Peter Thiel & Blake Masters — Zero to One |
| [`platform-thinking`](skills/strategy/platform-thinking/SKILL.md) | Decides whether to open a product into a platform, what control that costs, and which half of the business you keep | Geoffrey Parker, Marshall Van Alstyne & Sangeet Paul Choudary — Platform Revolution; Andrew Chen — The Cold Start Problem; Thomas Eisenmann, Geoffrey Parker & Marshall Van Alstyne — platform strategy research (HBR); Jeff Jarvis — What Would Google Do? |
| [`scaling-playbook`](skills/strategy/scaling-playbook/SKILL.md) | Runs the company through the post-product/market-fit phase, where the constraint stops being the product and becomes the organization | Elad Gil — High Growth Handbook |
| [`value-innovation`](skills/strategy/value-innovation/SKILL.md) | Rebuilds an offer so that differentiation and cost fall together, by charting what the industry competes on and deleting most of it | W. Chan Kim & Renée Mauborgne — Blue Ocean Strategy |
| [`venture-financing`](skills/strategy/venture-financing/SKILL.md) | Turns a venture round from a price negotiation into a governance decision you can actually model | Scott Kupor — Secrets of Sand Hill Road |

### Go-to-market — demand, launch, price

| Skill | What it decides | Lineage |
|---|---|---|
| [`audience-engine`](skills/gtm/audience-engine/SKILL.md) | Builds an owned audience as a compounding distribution asset — a defensible angle, one channel held long enough to matter, attention converted into subscribers you control, and monetization gated on self-propelled growth | Joe Pulizzi — Content Inc.; Mark Schaefer — The Content Code |
| [`chasm-crossing`](skills/gtm/chasm-crossing/SKILL.md) | Selects and defends the single beachhead segment that converts early-adopter traction into repeatable mainstream revenue, using a funding test and an adjacency test rather than intuition | Geoffrey A. Moore — Crossing the Chasm |
| [`freemium-economics`](skills/gtm/freemium-economics/SKILL.md) | Decides whether to give something away, who pays for it, and where the line between free and paid should sit, using marginal cost to serve and a named cross-subsidy rather than optimism | Chris Anderson — Free: The Future of a Radical Price |
| [`growth-loops`](skills/gtm/growth-loops/SKILL.md) | Separates real compounding loops from funnels wearing loop vocabulary, using four tests — reinvestment, compounding, independence, and cycle time — and then sizes what a sub-1 loop is actually worth | Sean Ellis & Morgan Brown — Hacking Growth; Gabriel Weinberg & Justin Mares — Traction; Andrew Chen — the law of shitty clickthroughs; Jonah Berger — Contagious |
| [`gtm-measurement`](skills/gtm/gtm-measurement/SKILL.md) | Builds the go-to-market measurement stack in the order that survives being wrong — money events first, activation second, attribution third — and names the metric that misleads at each stage of growth | Dave McClure — pirate metrics (AARRR); Sean Ellis & Morgan Brown — Hacking Growth; Eric Ries — The Lean Startup (actionable vs. vanity metrics); Chris Goward — PIE prioritization |
| [`headline-craft`](skills/gtm/headline-craft/SKILL.md) | Writes and selects headlines by decision procedure rather than by pulling templates — promise first, reader awareness second, provable substance third, and a forced spread across trigger families before anything gets tested | John Caples — Tested Advertising Methods; David Ogilvy — Ogilvy on Advertising; Eugene Schwartz — Breakthrough Advertising; Joseph Sugarman — The Adweek Copywriting Handbook |
| [`launch-execution`](skills/gtm/launch-execution/SKILL.md) | Turns a launch date into a sequenced operation with entry gates, a named primary surface, a recruited support group, and a go/no-go bug bar | Colin Bryar & Bill Carr — Working Backwards (Amazon's PR/FAQ method); Jakob Nielsen — Why You Only Need to Test with 5 Users; Maja Voje — GTM Strategist |
| [`lead-engine`](skills/gtm/lead-engine/SKILL.md) | Picks the one acquisition channel your stage can actually sustain, sets the volume and efficiency thresholds that prove it works, and defines the bait that attracts buyers instead of spectators | Alex Hormozi — $100M Leads |
| [`monetization-model`](skills/gtm/monetization-model/SKILL.md) | Designs the sequence of offers around a first sale so that cash collected in the first 30 days exceeds the cost of acquiring and serving the customer | Alex Hormozi — $100M Money Models |
| [`offer-design`](skills/gtm/offer-design/SKILL.md) | Rebuilds a commoditized offer into a priced package that cannot be line-item compared, by inventorying the buyer's friction and engineering the gap between perceived value and price | Alex Hormozi — $100M Offers |
| [`partner-engine`](skills/gtm/partner-engine/SKILL.md) | Wins distribution by borrowing an audience someone else already built — mapping the specific people and communities that already hold your buyer's trust, earning entry before asking for anything, and choosing between paying for access and earning it | Chet Holmes — The Ultimate Sales Machine (Dream 100 prospecting) |
| [`pricing-power`](skills/gtm/pricing-power/SKILL.md) | Sets price from evidence of what buyers will pay rather than from competitor averages or cost-plus, by choosing the billing unit first, gathering willingness-to-pay signal at a method appropriate to sample size, and packaging into tiers with a single upgrade gate | Madhavan Ramanujam & Georg Tacke — Monetizing Innovation; Peter van Westendorp — Price Sensitivity Meter; André Gabor & Clive Granger — price-response research |

### Revenue — enterprise sales execution

| Skill | What it decides | Lineage |
|---|---|---|
| [`buyer-psychology`](skills/revenue/buyer-psychology/SKILL.md) | Reads how a specific buyer processes evidence and risk, then changes the format, pace, and proof of your sales motion to match | David Merrill & Roger Reid — Personal Styles and Effective Performance; William Moulton Marston — Emotions of Normal People (the DISC tradition these four-quadrant models descend from) |
| [`challenger-selling`](skills/revenue/challenger-selling/SKILL.md) | Builds and delivers a commercial insight that reframes how a buyer sees their own problem, then holds the tension long enough for it to change their behavior | Matthew Dixon & Brent Adamson — The Challenger Sale |
| [`channel-strategy`](skills/revenue/channel-strategy/SKILL.md) | Decides whether to sell direct, through partners, or both, and builds the rules that make a partner economy work | Pedro Luiz Roccato — O Grande Livro de Canais de Vendas |
| [`deal-qualification`](skills/revenue/deal-qualification/SKILL.md) | Scores an enterprise opportunity on the eight things that actually predict a close, finds the weakest one, and turns it into this week's action | Jack Napoli, Dick Dunkel & John McMahon (MEDDIC at PTC); Andy Whyte — MEDDICC |
| [`enterprise-negotiation`](skills/revenue/enterprise-negotiation/SKILL.md) | Reads the power, incentives, and alternatives inside a corporate buying group, then converts that map into what to say next | Fisher, Ury & Patton — Getting to Yes; Robert Cialdini — Influence; Mahan Khalsa — Let's Get Real or Let's Not Play |
| [`overcoming-indecision`](skills/revenue/overcoming-indecision/SKILL.md) | Diagnoses why a buyer who already wants to change still will not decide, then runs four moves: judge the indecision, recommend personally, limit the research, take risk off the table | Matthew Dixon & Ted McKenna — The JOLT Effect |
| [`value-messaging`](skills/revenue/value-messaging/SKILL.md) | Builds the argument that survives a CFO, a competitor, and six weeks of silence: the customer's problem in their own words, priced in currency, and tied to capabilities only you do well | Force Management — Command of the Message / Value Messaging Framework |

### Operations — running the company

| Skill | What it decides | Lineage |
|---|---|---|
| [`constraint-analysis`](skills/operations/constraint-analysis/SKILL.md) | Finds the one place in a business that actually caps output, then routes every decision through it: identification procedure for systems with no visible queue, exploitation before investment, subordination of everything else, and the inertia check for when the constraint moves | Eliyahu M. Goldratt — The Goal and the Theory of Constraints |
| [`daily-management`](skills/operations/daily-management/SKILL.md) | Separates the work of holding a result from the work of raising it, then installs the routine that holds it: control items with action rules, written standards for the tasks that matter, and an anomaly-treatment loop with named roles | Vicente Falconi Campos — Gerenciamento da Rotina do Trabalho do Dia a Dia, O Verdadeiro Poder; W. Edwards Deming and the Japanese TQC tradition |
| [`management-os`](skills/operations/management-os/SKILL.md) | The operating system for a manager's own week: how to convert your hours into other people's output, how much rope to give each person on each task, how to refuse work that belongs to someone else, and which four meetings earn their place on the calendar | Andy Grove — High Output Management; William Oncken Jr. & Donald Wass — Management Time: Who's Got the Monkey?; Jason Fried & David Heinemeier Hansson — Rework |
| [`okr-system`](skills/operations/okr-system/SKILL.md) | Installs a quarterly goal system that survives contact with a real company: three objectives, key results written as outcomes, a hard firewall between scores and pay, and a weekly check-in that moves confidence rather than percentages | Andy Grove — High Output Management; John Doerr — Measure What Matters |
| [`structured-problem-solving`](skills/operations/structured-problem-solving/SKILL.md) | Turns a vague business problem into an answer someone will act on: a sharp question, a hypothesis formed in the first hour, an issue tree that can falsify it, the two analyses that decide it, and a conclusion delivered answer-first | Ethan M. Rasiel & Paul N. Friga — The McKinsey Mind; Barbara Minto — The Pyramid Principle |

### Brand — positioning and communication

| Skill | What it decides | Lineage |
|---|---|---|
| [`design-systems`](skills/brand/design-systems/SKILL.md) | Decides whether a design system is justified yet, then builds one as three token tiers, a small set of components with deliberate APIs, and a governance contract covering contribution and deprecation | Brad Frost — Atomic Design; Alla Kholmatova — Design Systems; Josef Müller-Brockmann — Grid Systems; Alina Wheeler — Designing Brand Identity |
| [`founder-narrative`](skills/brand/founder-narrative/SKILL.md) | Builds the founder or spokesperson identity a company runs consistently across content, sales, and lifecycle email — a real backstory, a stated position, and an origin story shaped so a stranger reaches your conclusion by living the discovery themselves | Direct-response funnel literature, 2010s; Joseph Campbell — The Hero with a Thousand Faces |
| [`positioning`](skills/brand/positioning/SKILL.md) | Rebuilds the market context a buyer uses to judge your product, by sequencing competitive alternatives, unique attributes, value themes, best-fit segment, and market category — then testing whether the result is load-bearing or a slogan | Al Ries & Jack Trout — Positioning; April Dunford — Obviously Awesome |
| [`presentation-craft`](skills/brand/presentation-craft/SKILL.md) | Builds a presentation by first deciding whether the artifact is a document to be read or slides to be presented, then structuring the argument, enforcing one idea per slide, and rehearsing against objections rather than script | Nancy Duarte — Resonate / slide:ology; Barbara Minto — The Pyramid Principle; Garr Reynolds — Presentation Zen |
| [`purpose-narrative`](skills/brand/purpose-narrative/SKILL.md) | Extracts a company's operating belief from its actual history, tests it for falsifiability, and reorders the story so belief precedes method precedes product — then audits whether incentives contradict the stated purpose | Simon Sinek — Start With Why |

## How to compose them

Skills are written to chain. A few sequences that come up constantly:

**New venture, nothing validated yet**

```
discovery/customer-interviews  →  discovery/jobs-to-be-done  →  strategy/monopoly-thesis
   →  discovery/venture-design  →  gtm/pricing-power
```

**Enterprise deal that has gone quiet**

```
revenue/deal-qualification  →  find the weakest element  →  revenue/value-messaging
   →  revenue/enterprise-negotiation
```

**Win rate is fine but nobody knows what you are**

```
brand/positioning  →  revenue/value-messaging  →  gtm/chasm-crossing
```

**Post product/market fit, execution is the constraint**

```
operations/constraint-analysis  →  operations/okr-system  →  operations/daily-management
   →  strategy/scaling-playbook
```

Each file's **Pairs with** section names its own neighbors and why.

## On sources and originality

These skills stand on published work by people who did the thinking first — Ries and
Trout, April Dunford, Clayton Christensen, Bill Aulet, Rob Fitzpatrick, Anthony Ulwick,
Andy Grove, Vicente Falconi, Eliyahu Goldratt, Steve Blank, and others. Every file names
its lineage explicitly and states where this articulation departs from it.

None of these files reproduce their sources. They are rewrites into an operator's decision
procedure — which means most of the original book is deliberately absent, and what is here
that matters most (the thresholds, the failure modes, the sequencing, the disagreements)
is not in the book at all. If a skill makes you want the underlying work, buy it. Several
are worth far more than a summary of them.

One skill worth calling out: [`operations/daily-management`](skills/operations/daily-management/SKILL.md)
documents the Falconi management system — the PDCA/SDCA discipline that runs a large share
of Brazilian industry and is almost entirely absent from English-language startup writing.
If you have only ever read American management books, start there.

## Contributing

Issues and pull requests are welcome, with one standard: additions must be procedures,
not summaries. See [CONTRIBUTING.md](CONTRIBUTING.md) for the authoring rules — the same
ones every existing file was written against.

If you use these and something breaks in the field, open an issue and say what happened.
A failure mode discovered in a real company is worth more than a new skill.

## Who wrote this

**Leonardo Frade** — partner at [Khiza](https://khizadao.com), a web3 startup studio,
and at [Her0](https://her0.io), an AI startup studio where I also run the portfolio. Board
member at two Brazilian companies. Before that: Director of Expansion at Endeavor Brazil,
one exit as a founder, and 500 Startups in San Francisco.

I am not an engineer. I am an operator who reorganized how he works around agents, and
this repository is the substrate that makes that work. If you are a founder trying to
figure out what AI-native actually means outside of code, this is my answer: put your
judgment in files, keep it versioned, make it composable, and stop re-deriving decisions
you already made.

- LinkedIn — [in/leofrade](https://www.linkedin.com/in/leofrade/)
- Her0 — [her0.io](https://her0.io) · Khiza — [khizadao.com](https://khizadao.com)

## License

Documentation and skill content: [CC BY 4.0](LICENSE) — use it commercially, adapt it,
just keep the attribution.
Any code or tooling added later: MIT.

---

<div align="center">
<sub>If this saved you a bad quarter, a star helps other operators find it.</sub>
</div>
