---
name: brand-engine-generator
description: >
  Generate new on-brand assets (social graphics, slide backgrounds, ad
  variants, UI empty-states, OOH concepts, etc.) that comply with this
  client's Brand Engine -- its primitives, shared token DNA, and combination
  rules. Use whenever the client's team needs a new asset in a format the
  original engagement didn't already produce, and wants it to look like it
  came from the same system without commissioning new design work. Trigger
  on requests like "make a version of this for Instagram," "I need a banner
  for the launch," "generate a new hero image in our brand," or "does this
  asset someone made follow our brand system."
---

# Brand Engine Generator -- template

This is a standing execution tool, not a stage in the seven-skill chain. A
client starts using it after `brand-engine-07-handoff-training` closes the
Handoff Brief -- it reads the live token file directly rather than the
artifact chain, and it doesn't produce a Brief of its own. See
`../_shared/protocol.md` for the "distinguish fact / judgment / needs
confirmation" and "read live, never from memory" discipline this skill
still follows, even outside the staged chain.

This is a template skill. It ships empty (using the example tokens from
`../../engine/tokens.json`) so it can be filled in with a real client's
system at the end of `brand-engine-06-skill-encoding`. Replace every
section marked `<!-- CLIENT: ... -->` before handing this off.

## What this skill does

Two jobs, both grounded in the client's actual token file -- never invented
from general design taste:

1. **Generate** -- produce a new asset (image spec, HTML/CSS mockup, or
   direct file when the requesting tool supports it) that uses only the
   client's defined primitives, reads color/depth/motion from their tokens,
   and obeys every listed combination rule.
2. **Check** -- given an existing asset (an image, a Figma link description,
   an HTML snippet), evaluate it against the same rules and report specific,
   fixable violations -- not vague "doesn't feel on-brand" feedback.

## Before generating anything

1. Read the client's token file (`tokens.json` or equivalent) in full. Do
   not proceed from memory of a past conversation -- token values are the
   single source of truth and may have been updated.
2. Identify which primitive(s) the request calls for. If the request
   doesn't map cleanly to an existing primitive, say so explicitly and ask
   whether this is a new use case that needs a new primitive (which is a
   design decision, not something this skill should invent on its own).
3. Identify the target format (social post, deck slide, banner, print,
   in-product UI, etc.) and check whether the engine's documented rules
   already cover that format. If the engine has never been validated
   against this format, flag that as a risk before producing the asset.

## Generation rules (read from tokens, not hardcoded)

- Use `color.signal.primary` as the only saturated accent; never introduce
  a new hue. Respect the stated max surface-coverage rule.
- Apply `material.depth` and `material.grain` values identically across
  every primitive in the composition -- depth and grain are shared-DNA
  tokens, not per-shape choices.
- Apply `motion.easing` to any animated or implied-motion element.
- Resolve all directional elements to `geometry.axis`.
- Follow every rule listed under `combination_rules` exactly, including
  primitive count limits and dominance ratios (e.g. 60/40 minimum split
  when two primitives share a composition).
- <!-- CLIENT: add any format-specific constraints here, e.g. minimum
  logo clear-space, required legal lockup, localization rules. -->

## Check rules (when reviewing an existing asset)

Report violations against the same list above, each as: what rule was
broken, where in the asset, and the specific fix (not "adjust the color" --
"the accent hue is applied to two shapes at once; combination_rules
requires it be limited to one dominant primitive per composition").

## What this skill will not do

- Invent a new primitive or change a token value on its own. Both are
  brand decisions; this skill executes the existing system, it doesn't
  redesign it. If a request genuinely can't be satisfied within the
  current engine, say that plainly and suggest it as a candidate for the
  next engine review (see the Tier 4 retainer in `docs/service-offering.md`).
- Produce an asset without first reading the live token file -- cached or
  remembered values are not acceptable, since tokens may have been updated
  since the engine was last touched.
- Fabricate brand rationale. If a rule's reasoning isn't documented, note
  that it's undocumented rather than guessing at intent.

## Example invocation

> "Make a LinkedIn announcement graphic for our new pricing page using the
> Arc primitive, warm variant."

Expected behavior: pull `color`, `material`, and `motion` tokens from the
live file, confirm LinkedIn's 1200x627 format isn't already covered by an
existing rule (flag if untested), generate the asset using only the Arc
primitive per `combination_rules`, and state which token values were used
so the output is auditable against the system.

<!-- CLIENT: replace this template's example with 2-3 real examples from
the actual engagement, using the client's real primitive names and at
least one asset type produced during the live test run in
brand-engine-07-handoff-training (see that skill's Handoff Brief for the
specific format that was tested). -->
