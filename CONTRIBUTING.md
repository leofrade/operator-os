# Contributing to Operator OS

The bar here is not "is this useful information." It is **could a competent operator do
something differently tomorrow because of this file.** Almost everything that gets
rejected is rejected for being true but inert.

## What gets merged

**Failure modes discovered in the field.** The highest-value contribution. If you ran a
skill at a real company and it broke in a way the file did not anticipate, open an issue
describing what happened. One real trap is worth more than a new skill.

**Corrections.** Wrong threshold, misattributed lineage, a framework whose evidence base
has since been undermined. Say so.

**New skills** that meet the standard below.

**Translations**, provided they translate the procedure rather than flattening it.

## What gets rejected

- Book summaries. Any model produces those on request; they are worth nothing here.
- Prompt templates ("act as a world-class CMO").
- Frameworks with no threshold, no exit criterion, and no failure mode.
- Skills that overlap an existing one without arguing why the split is real.
- Vendor content or thinly disguised marketing for a product.

## The authoring standard

Every file in this repository was written against these rules. New ones must be too.

### File shape

Skills live at `skills/<domain>/<skill-name>/SKILL.md`. Domains are `discovery`,
`strategy`, `gtm`, `revenue`, `operations`, `brand`. The directory name must equal the
frontmatter `name`.

### Frontmatter

```yaml
---
name: skill-name-in-kebab-case
description: >-
  One dense sentence on what the skill does, then the activation triggers as a
  natural-language list. Written so an agent can route to it reliably. 40-80 words.
domain: revenue | gtm | strategy | discovery | operations | brand
stage: pre-pmf | gtm | scale | any
lineage: "Author Name — *Work Title*; Second Author — *Work*"
author: Your Name
version: 1.0
license: CC-BY-4.0
---
```

The `description` is the routing surface. If an agent cannot tell from it when to fire the
skill, the skill will not fire. Write the triggers in the language a user would actually
use, not in the framework's jargon.

### Body sections, in this order

| Section | Requirement |
|---|---|
| `# Title` + `> thesis` | One line. The sharpest true sentence about why this matters. No hedging. |
| `## The question this answers` | 2-4 bullets. Real questions asked out loud, not topics. |
| `## When to run it` | Entry conditions. **Must include an explicit "Do not run this when…" clause.** |
| `## The method` | 3-7 numbered moves. Each needs a decision rule or threshold and an exit criterion. |
| `## Failure modes` | Minimum 4, named. Format: **Name** — the tell. → the correction. |
| `## Outputs` | Concrete artifacts a run should produce. |
| `## Pairs with` | Minimum 2 cross-links, relative paths, each with a reason. |
| `## Lineage` | Credit the originators, and state where this departs from them. |

### Length

**1,200-1,900 words of body, targeting around 1,500.** Density is the point. If your draft is 3,000 words, most of
the excess is recap. Cut it.

### Voice

- English, plain and declarative. Short sentences.
- Second person for instructions.
- Numbers over adjectives. "Below 6/10, kill the deal" beats "carefully evaluate."
- No emoji. No exclamation marks. American spelling.
- Banned: "In today's fast-paced…", "It's important to note", "Let's dive in", "unlock",
  "leverage" as a verb.
- Assume a competent founder or operator, not a student.

## Intellectual property

**Do not reproduce sources.** Do not paste a book's full enumerated framework, its
complete step list, or its case-study roster. If a passage could be diffed against the
original and match, rewrite it.

**Do credit sources.** Every file names its lineage. Attribution is not a license to
reproduce — the rewrite is what makes publication legitimate — but the credit is
intellectually correct and non-negotiable.

**Do not include confidential material.** No client names, no revenue or churn figures, no
contract terms, no internal data from any company you work for or advise. Replace real
examples with neutral archetypes: "a vertical SaaS in a regulated market", "a multi-site
distributor". This applies to your employer as much as to anyone else's.

## Submitting

1. Fork, branch, write the file.
2. Verify: valid YAML frontmatter, all seven sections present, ≥4 failure modes,
   ≥2 working relative cross-links, body inside 1,200-1,900 words.
3. Open a PR. In the description, state the one decision this skill changes and the
   situation where you have actually run it.

Contributions are licensed CC BY 4.0, consistent with the rest of the repository.
