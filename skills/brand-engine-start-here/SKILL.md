---
name: brand-engine-start-here
description: >
  Use when someone wants to start a Brand Engine engagement but doesn't
  know which stage skill applies, or has a single specific question and
  isn't sure where it fits in the seven-stage process. Asks a small number
  of triage questions and routes to the correct stage skill instead of
  defaulting to stage one. Don't use this for a full system overview (that's
  brand-engine-hub) or for a question that already clearly names its stage.
---

# Brand Engine -- start here

Read `../_shared/protocol.md` first.

## What this is for

Most people arrive with one real question, not a request to run the whole
process from scratch. This skill's only job is to find out what that
question actually is and route to the stage skill that owns it -- including,
often, a stage other than Discovery.

## Triage questions

Ask at most one to two questions per turn, not a list. Useful ones, pick
whichever is most relevant to what they've already said:

- Is there an existing brand here already, or is this from zero? (If from
  zero and no engagement has started, Discovery is likely right. If there's
  an existing brand and the question is "should we even touch this,"
  `brand-engine-audit` may be a better fit than Discovery.)
- Do they already have primitives chosen, or is the question about what the
  primitives should be?
- Is the question about the visual/material system (color, depth, motion,
  geometry) or about the rules that govern how primitives combine?
- Are they trying to produce actual assets, or trying to get their own team
  generating assets going forward?
- Is this a brand-new relationship, or do they already have Briefs from a
  prior session?

## Routing table

- No engagement started, question is about equity, competitors, or which
  formats matter -- `brand-engine-01-discovery`
- Existing brand, question is "is this worth evolving" with no committed
  engagement yet -- `brand-engine-audit`
- Discovery Brief exists, question is about which shapes/motifs to use --
  `brand-engine-02-primitive-selection`
- Primitives chosen, question is about color/material/motion/geometry
  tokens -- `brand-engine-03-dna-definition`
- Tokens exist, question is about what can combine with what --
  `brand-engine-04-rule-authoring`
- Rules exist, question is about producing hero assets to prove the system --
  `brand-engine-05-asset-production`
- Assets exist, question is about packaging the rules as something the
  client's own AI tools can run -- `brand-engine-06-skill-encoding`
- Skill exists, question is about training the client team or closing the
  engagement -- `brand-engine-07-handoff-training`
- Multiple Briefs exist already and something seems inconsistent between
  them -- `brand-engine-hub`, not this skill
- Engagement is fully handed off and the question is "generate me an asset"
  -- `brand-engine-generator`

## Closure conditions

Route as soon as the question clearly maps to one stage. Don't keep
triaging past that point -- over-triaging a clear question is its own
failure mode.

## Formal artifact: Routing Brief

A short version of the shared output shell: current judgment (which stage
this belongs to), key evidence (what they said that indicates it), and the
recommended next skill. This doesn't need the full six-part shell -- it's
a router, not a diagnostic stage -- but it should still be explicit about
what it does *not* know yet, so the destination skill isn't starting blind.
