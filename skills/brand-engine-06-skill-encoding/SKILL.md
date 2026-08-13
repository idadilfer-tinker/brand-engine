---
name: brand-engine-06-skill-encoding
description: >
  Use once the rule set is production-tested to package it as an operable
  skill/agent config -- filling in the brand-engine-generator template with
  this specific client's tokens, rules, and real examples. Produces the
  Skill Brief and the client's actual SKILL.md. Not for training the client
  team on it (that's brand-engine-07) and not for producing more hero
  assets (that's brand-engine-05).
---

# Stage 6 -- Skill encoding

Read `../_shared/protocol.md` first. See
`skills/brand-engine-generator/SKILL.md` for the template this stage fills
in.

## What this is for

This is the layer most competitors don't ship (see `docs/research.md`).
The rule set becomes something the client's own AI tools can execute, not
just something a human reads before making an asset by hand.

## Triage

If no Asset Brief exists, route back to `brand-engine-05-asset-production`
first -- encoding an unproven rule set just moves the failure downstream to
the client's own team, which is worse.

## Diagnosis

- Does the template's Generation rules section reference this client's
  actual token names and values, or is it still using placeholder
  language?
- Does the template's Check rules section cover every rule from the Rule
  Brief, including the ones only surfaced during asset production?
- Are there real, client-specific examples in the Example invocation
  section -- not the generic template example -- using formats the client
  actually produced in stage 5?
- Is there any format-specific constraint (legal lockup, clear-space,
  localization) that belongs in the CLIENT section and hasn't been added
  yet?

## Closure conditions

Only produce the Skill Brief once:

- Every `CLIENT:` placeholder in the template has been replaced with real
  content.
- At least two real examples, drawn from stage 5's actual assets, replace
  the generic template example.
- The skill file has been sanity-checked against the Rule Brief line by
  line -- every rule is represented.

## Formal artifact: Skill Brief

Use the shared output shell. Stage-specific content:

- **Current judgment**: the finished, client-specific SKILL.md is ready for
  handoff.
- **Key evidence**: which rules and examples came from where.
- **Primary thread**: anything the skill can't fully cover yet -- a rule
  that's still more judgment than checkable logic.
- **What not to do yet**: don't hand off to the client team until the
  Handoff stage confirms they can actually run it live; don't treat this
  stage's output as final without a live test run.
- **Recommended next step**: `brand-engine-07-handoff-training`.
- **Key conclusions for next skill**: the finished skill file, and any
  known weak spot to specifically test during the live training session.
