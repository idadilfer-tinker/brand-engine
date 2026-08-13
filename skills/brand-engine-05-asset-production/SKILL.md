---
name: brand-engine-05-asset-production
description: >
  Use once rules are authored to produce hero assets across priority
  formats and prove the system actually holds together in practice, the
  way Estudi-Image proved the Stripe system across billboard, card, phone
  UI, OOH, and stickers. Produces the Asset Brief. Not for packaging the
  system as an operable skill (that's brand-engine-06) and not for writing
  the rules themselves (that's brand-engine-04).
---

# Stage 5 -- Asset production

Read `../_shared/protocol.md` first.

## What this is for

Rules on paper and rules that survive contact with a real layout are
different things. This stage produces actual hero assets -- not a full
campaign, a proving set -- and treats every asset as a test of the rule set,
not just a deliverable.

## Triage

If no Rule Brief exists, route back to `brand-engine-04-rule-authoring`
first.

## Diagnosis

- Which formats from the Discovery Brief's inventory are highest priority
  to prove first -- usually the format most different from the others (a
  billboard and a mobile UI stress a system in different ways; producing
  two similar formats proves less than producing two different ones).
- Does each asset comply with every rule from the Rule Brief, or did
  producing a real asset surface a rule that doesn't actually hold up under
  a real layout?
- If a rule broke: is the fix a rule revision (route back to stage 4) or a
  one-off exception that should be logged, not quietly absorbed?

## Closure conditions

Only produce the Asset Brief once:

- At least two structurally different formats have been produced.
- Every asset has been checked against the rule set explicitly, not just
  eyeballed.
- Any rule that broke under real production has been either revised
  upstream or logged as a deliberate, documented exception.

## Formal artifact: Asset Brief

Use the shared output shell. Stage-specific content:

- **Current judgment**: which formats were proven and how they performed
  against the rule set.
- **Key evidence**: the specific compliance check for each asset.
- **Primary thread**: any rule that needs revision based on what production
  actually surfaced.
- **What not to do yet**: don't move to skill encoding while a rule is
  known to be broken; don't treat a one-off exception as a new default
  without updating the Rule Brief.
- **Recommended next step**: `brand-engine-06-skill-encoding`, or back to
  `brand-engine-04-rule-authoring` if a rule needs real revision first.
- **Key conclusions for next skill**: the proven asset set, and the final,
  production-tested version of the rule set for the skill to encode.
