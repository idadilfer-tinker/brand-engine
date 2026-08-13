---
name: brand-engine-03-dna-definition
description: >
  Use once primitives are chosen to establish the shared token layer --
  color, material/surface, motion, geometry -- that lets the primitives
  combine or stand alone without looking like separate systems. Produces
  the DNA Brief and a draft tokens.json. Not for writing the combination
  rules that govern how primitives interact (that's brand-engine-04) and
  not for choosing the primitives themselves (that's brand-engine-02).
---

# Stage 3 -- DNA definition

Read `../_shared/protocol.md` first. See `engine/tokens.json` in this repo
for the token structure this stage produces.

## What this is for

Primitives are shapes; DNA is what makes them read as one brand rather than
a shape collection. This stage defines the actual token values -- not
principles, values. "Warm, confident color" is not a token. `#FF5B1F` with
a stated max-coverage rule is.

## Triage

If no Primitive Brief exists, route back to
`brand-engine-02-primitive-selection` first.

## Diagnosis

Work through each token category as its own question, not all at once:

- **Color**: what's the one signal hue, and what's its stated maximum
  surface coverage? (Never more than one saturated accent -- see
  `docs/methodology.md`.)
- **Material**: what depth/shadow treatment and what surface texture
  (grain, gloss, matte, print) does every primitive share, regardless of
  its individual shape?
- **Motion**: what easing curve and what kind of movement (parallax,
  transform, none) applies uniformly?
- **Geometry**: is there a consistent axis or corner logic that every
  directional element resolves to?

For each, ask whether the value came from the client's stated preference,
the skill's own judgment based on positioning, or is still open -- and label
accordingly.

## Closure conditions

Only produce the DNA Brief once:

- Color, material, motion, and geometry each have an actual value, not a
  description.
- Every primitive from the Primitive Brief has been checked against every
  token -- no primitive gets a token exception.
- A draft `tokens.json` exists in the same shape as `engine/tokens.json` in
  this repo.

## Formal artifact: DNA Brief

Use the shared output shell. Stage-specific content:

- **Current judgment**: the finalized token values, in the four categories.
- **Key evidence**: what positioning or equity signal each token value
  traces back to (don't let a token be arbitrary -- if it can't be
  justified, it's not ready).
- **Primary thread**: which token is the shakiest or most likely to get
  revisited once real assets are produced.
- **What not to do yet**: don't write combination rules yet if any token is
  still a placeholder; don't let the client pick a second accent color
  "just for one use case."
- **Recommended next step**: `brand-engine-04-rule-authoring`.
- **Key conclusions for next skill**: the finalized token set (attach or
  reference the draft tokens.json).
