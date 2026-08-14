---
name: design-systems
description: >-
  Decides whether a design system is justified yet, then builds one as three
  token tiers, a small set of components with deliberate APIs, and a governance
  contract covering contribution and deprecation. Trigger when UI drifts across
  surfaces, when a rebrand or theming requirement lands, when designers and
  engineers argue about spacing and color, when a second product or platform
  ships, or when someone proposes standing up a design system team.
domain: brand
stage: scale
lineage: "Brad Frost — *Atomic Design*; Alla Kholmatova — *Design Systems*; Josef Müller-Brockmann — *Grid Systems*; Alina Wheeler — *Designing Brand Identity*"
author: Leonardo Frade
version: 1.0
license: CC-BY-4.0
---

# Design Systems

> A design system is a governance contract that happens to ship components. Teams that build the components and skip the contract get a second inconsistent UI plus a maintenance burden.

## The question this answers

- Is it too early, or are we already paying for not having one?
- How do tokens get structured so a rebrand or a dark mode is a config change, not a rewrite?
- Who is allowed to add a component, and how does anything ever get removed?
- Why does the library exist while product teams keep building their own buttons?

## When to run it

Run this when the same interface element exists in four or more visually distinct versions, when more than one squad ships UI, when a second platform or white-label requirement appears, or when a rebrand is scheduled and nobody can price it.

**Do not run this when** one team ships one surface and the product still changes shape weekly. Before product-market fit a system freezes decisions you have not earned the right to freeze: the abstraction cost is paid daily, the benefit arrives in a year. The substitute at that stage is one tokens file and a shared component folder, with a rule that anything used three times gets extracted. Also do not staff a dedicated systems team before three consuming teams exist — a platform with two customers is a hobby.

## The method

### Move 1 — Prove the cost before building the cure

Count, do not argue. Inventory the live product: distinct button styles, greys, type sizes, spacing values, modal implementations. Screenshot each. That number is both the business case and the baseline. Then size the recurring cost — hours per quarter rebuilding existing UI, plus the cost of the next rebrand.

**Threshold:** under three consuming teams and under roughly twenty duplicated components, the answer is a shared folder, not a system. Above both, proceed.

### Move 2 — Build the token layer in three tiers

The highest-leverage architectural decision here, and the one most often botched. Three tiers, and product code may only touch the third.

| Tier | Contains | Named for | Who edits it |
|---|---|---|---|
| Primitive | Raw values: `blue-600`, `space-4`, `size-14` | What it is | Systems owner only, rarely |
| Semantic | Intent: `color-surface-danger`, `space-inline-tight` | What it means | Systems owner, with review |
| Component | Bindings: `button-bg-destructive` | Where it applies | Component author |

Product code referencing `blue-600` directly is the defect that makes theming impossible later. Enforce the rule with a linter on day one, not a guideline — guidelines lose to deadlines.

Derive the spacing and type scales from one typographic decision — a base size and a line height — and make everything else a multiple. Müller-Brockmann's point about grids holds for tokens: constraint is what makes variation legible rather than accidental. A scale of arbitrary values is a list, not a scale.

**Exit criterion:** a theme swap is a change to the semantic tier alone, verified by actually shipping a second theme.

### Move 3 — Extract components from evidence, not imagination

Frost's atomic vocabulary is a useful ordering heuristic: small elements compose into groups, groups into sections, sections into templates. Treat it as a naming convention, not a taxonomy to enforce — teams arguing whether a search bar is a molecule or an organism have found a way to avoid shipping.

Extract only what already exists three times in production; speculative components are the main source of dead library weight. Then design the API deliberately. Two rules carry most of the value:

- **No boolean explosion.** Three booleans mean eight states, most untested. Use one variant enum instead. If a component needs `isPrimary`, `isDanger`, and `isGhost`, it needs `variant`.
- **One documented escape hatch.** Every component gets a sanctioned way to deviate — a slot, a style override, a composition path. Without one, teams fork silently and you lose sight of the drift you were trying to prevent.

**Exit criterion:** each component ships with a variant matrix, an escape hatch, accessibility states, and a real page using it with production content. Hold Kholmatova's distinction while you do it: the functional pattern is what the thing does, the perceptual pattern is what it feels like, and they change on different schedules. Separate layers mean a visual refresh does not touch behavior.

### Move 4 — Write the governance contract

Governance is what makes it a system rather than a library. One page, before the first release.

```
Contribution
  Anyone may propose. Proposal states: 3 production uses, the variant matrix,
  the a11y states. Systems owner reviews within 5 working days.
  No review inside 5 days → the proposing team ships it locally and it is
  reconsidered next cycle. Silence must not be a veto.

Deprecation
  Deprecated components emit a build warning, ship with a codemod or a written
  migration path, and are removed on a named date at least 2 minor versions out.
  Removal without a migration path is prohibited.

Breaking changes
  Semver. Majors batched to a maximum of two per year, announced 30 days ahead.
```

The five-day clause decides adoption. A system whose maintainers are a bottleneck gets routed around within a quarter, and shadow components cost far more than a slightly imperfect contribution.

### Move 5 — Measure coverage, not inventory

Component count and library size measure effort, not effect. Track two numbers monthly.

- **Adoption rate** — share of rendered UI nodes coming from system components. Target above 70 percent before adding scope.
- **Hardcoded value count** — raw hex, px, and font values in product code. Should trend near zero; if it does not, the escape hatch is wrong or missing.

A third signal: time-to-first-screen for a new engineer. If it has not fallen after two quarters, the system is documentation, not infrastructure.

## Failure modes

**Library mistaken for system** — components ship, nothing is written about contribution or deprecation, and within two quarters there are two systems. The tell is a second internal component folder. → Run Move 4 retroactively and absorb the shadow set.

**Semantic tier skipped** — product code binds straight to primitives because it was faster, and the first theming request costs a quarter. The tell is `blue-600` in a feature branch. → Add the tier and the lint rule, migrate by codemod. This gets more expensive weekly.

**Boolean explosion** — a component accumulates flags until its combinations are untestable. The tell is a prop list longer than the component's documentation. → Collapse into variant enums; delete combinations nobody uses in production.

**Deprecation by announcement** — old components are declared dead in a channel message, no codemod ships, and they live for years. The tell is a component deprecated two releases ago with active usage. → No deprecation without a migration path and a removal date.

**Coverage theater** — the system is reported by component count while product teams keep building their own. The tell is a growing library and a flat adoption rate. → Report adoption rate and hardcoded-value count instead.

**Design-code divergence** — the design file and the shipped component drift, and each side calls the other wrong. The tell is a spec citing a spacing value that does not exist in code. → Name one source of truth per layer: tokens generated from code, behavior owned by code, visual intent owned by design. Parity is a pipeline, not a promise.

**Premature platform team** — a dedicated team is staffed with two consumers, so it invents work and ships abstractions nobody asked for. The tell is a roadmap of components with no requesting team. → Staff part-time from consuming teams until three real consumers exist.

**Governance by taste** — no intake path exists, so contributing depends on catching the right person and everyone else forks. The tell is a component built twice in one month by different squads. → Publish the intake path and the five-day rule.

## Outputs

- A duplication inventory with counts and screenshots, plus the quarterly cost estimate.
- A three-tier token file with the semantic layer named by intent, and the lint rule enforcing it.
- A component extraction list ordered by production frequency, speculative items deferred.
- A per-component spec: variant matrix, escape hatch, accessibility states, production example.
- A one-page governance contract covering contribution, deprecation, and breaking changes.
- A monthly dashboard with adoption rate and hardcoded-value count.

## Pairs with

- [`brand/positioning`](../../brand/positioning/SKILL.md) — decides what the product should feel like before tokens encode it; visual language without a position is decoration.
- [`brand/presentation-craft`](../../brand/presentation-craft/SKILL.md) — applies the same token and hierarchy discipline to decks, where consistency usually breaks first.
- [`brand/purpose-narrative`](../../brand/purpose-narrative/SKILL.md) — supplies the principles that settle taste arguments component review cannot.

## Lineage

Brad Frost's *Atomic Design* supplies the composition vocabulary and the argument that interfaces should be scoped as systems of parts rather than pages. Alla Kholmatova's *Design Systems* supplies the functional-versus-perceptual distinction, and the more important observation that shared language and shared practice are what make a pattern library work at all. Josef Müller-Brockmann's grid work underpins deriving every spatial value from a single typographic decision. Alina Wheeler's *Designing Brand Identity* supplies the touchpoint discipline that keeps a digital system coherent with everything else a customer sees.

This articulation departs from all four in emphasis. It treats atomic vocabulary as a naming convention rather than a hierarchy worth defending, because classification arguments cost more time than they save. It puts governance and token architecture ahead of component craft, since those decide whether a system survives its second year. And it adds an explicit do-not-build threshold: the most common failure in practice is not a badly built design system but a correctly built one shipped two years early.
