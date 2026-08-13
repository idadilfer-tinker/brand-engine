---
name: brand-engine-04-rule-authoring
description: >
  Use once tokens are defined to write the combination logic precisely
  enough to be machine-checkable, not just human-readable -- what can
  combine with what, dominance ratios, primitive count limits. Produces the
  Rule Brief and the combination_rules block of tokens.json. Not for
  producing actual hero assets from the rules (that's brand-engine-05) and
  not for defining the token values themselves (that's brand-engine-03).
---

# Stage 4 -- Rule authoring

Read `../_shared/protocol.md` first. See `combination_rules` in
`engine/tokens.json` for the target format.

## What this is for

This is the stage most traditional brand kits skip or leave as prose
("use the mark thoughtfully"). The test for a real rule: could
`brand-engine-generator` check compliance against it without a human
judgment call? If not, it's not finished yet.

## Triage

If no DNA Brief exists, route back to `brand-engine-03-dna-definition`
first -- rules without stable tokens will need rewriting the moment the
tokens change.

## Diagnosis

- When two or more primitives share a composition, is there a dominance
  rule (e.g., a minimum split ratio) so they don't compete at equal weight?
- Is there a hard cap on how many primitives can appear together?
- Does the signal color rule specify not just "one accent" but where it can
  and can't apply within a shared composition?
- Are there absolute never-rules -- combinations that should never occur
  regardless of format -- distinct from soft defaults that a format
  exception could override?
- For each rule candidate, could it be phrased as a checkable condition
  rather than a value judgment? If the best phrasing is still "use good
  taste here," it's not a rule yet -- say so rather than forcing it into
  rule form.

## Closure conditions

Only produce the Rule Brief once:

- Every primitive-combination scenario from the Primitive Brief has an
  explicit rule, not a gap.
- At least one rule has been tested against a real hypothetical asset to
  confirm it's actually checkable.
- Absolute rules and soft defaults are distinguished from each other.

## Formal artifact: Rule Brief

Use the shared output shell. Stage-specific content:

- **Current judgment**: the finalized `combination_rules` list.
- **Key evidence**: the hypothetical asset each rule was tested against.
- **Primary thread**: the rule most likely to need a format-specific
  exception once real assets get produced.
- **What not to do yet**: don't finalize hero assets on an untested rule
  set; don't leave any rule in prose form if it can be made checkable.
- **Recommended next step**: `brand-engine-05-asset-production`.
- **Key conclusions for next skill**: the finalized rule set, and which
  rule is least proven so asset production can stress-test it first.
