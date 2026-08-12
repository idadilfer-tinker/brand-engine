# Methodology -- The Brand Engine

## The idea in one sentence

Instead of selling a startup a finished brand, sell them the rules that generate the brand -- a small set of primitives sharing one DNA, documented and encoded well enough that the startup's own team (or their AI tools) can keep producing new, correct work without commissioning it each time.

## Why this, why now

Traditional branding is a bottleneck by design: one studio produces a static kit (logo, colors, type, a few templates), hands it over, and every new use case -- a new landing page, a new pitch deck, a new OOH campaign, a new in-product surface -- either gets stretched awkwardly out of that kit or triggers a new billable engagement. That model made sense when design output was expensive and slow.

It doesn't make sense anymore. Startup teams now routinely use AI tools to generate their own components, copy, and layouts. The constraint has moved from "can we produce this asset" to "does what we produce actually look like it belongs to us." A brand kit built for a pre-AI production pace doesn't survive that shift -- it wasn't built to be extended by fifty people generating variations a day, it was built to be extended by one designer producing a few assets a month.

The Brand Engine is the response: build the brand as a system with explicit combination rules, not a fixed set of outputs, so it can absorb high-velocity, distributed production -- including AI-generated production -- without drifting off-brand.

## The three layers every engine needs

### 1. Primitives + shared DNA

A small number (2-4) of core visual or conceptual elements, each distinct enough to be recognizable alone, all sharing one underlying material language: the same color logic, the same surface/depth treatment, the same motion physics, the same geometric grammar. Shared DNA is what lets primitives combine or stand alone without looking like they came from different systems -- this is what Stripe's Wave and Parallelogram demonstrate (see research.md).

Primitives are chosen, not invented from nothing, whenever prior equity exists. If the startup already has a shape, a gesture, a color that people associate with them, the job is usually to give it more depth and rigor, not replace it.

### 2. The rule set (documentation layer)

The traditional brand guideline, but written as executable logic rather than mood-board prose: what can combine with what, what can never happen, how the system flexes across format (billboard vs. mobile UI vs. a slide) without breaking. This is the layer most agencies stop at. It's necessary but not sufficient -- a PDF of rules still requires a human who has read and internalized it to produce correct output.

### 3. The operable skill (machine layer)

The rule set re-encoded as something an AI agent can execute directly -- tokens, constraints, and generation logic packaged as a skill/agent config the client's own team loads into their tools (Claude, Cowork, or equivalent) to generate on-brand assets on demand. This is the layer that makes the engine actually self-sustaining after the engagement ends, and it's the layer most competitors in this space (Ramotion, Heartbeat, MetaLab, The Branx -- see research.md) aren't yet shipping as a first-class deliverable. See skills/brand-engine-generator/SKILL.md for a working example of this layer.

## Design principles for building an engine

Evolve equity, don't erase it. If a shape, color, or gesture already carries meaning for the client, deepen it before considering replacement. Discarding recognizable equity to "start fresh" is usually a cost, not a gain.

Fewer primitives, tighter rules. Two elements with an airtight shared-DNA rule outscale ten elements with a loose one. The constraint is what makes distributed, high-velocity production stay on-brand -- not the primitive count.

Design for the format you haven't thought of yet. A system that only works for the deliverables in the original engagement (say, a landing page and a deck) will visibly crack the first time the startup needs a subway ad or an in-product empty state. Test primitives against at least one format outside the original brief before shipping.

Write rules a machine can check, not just a human can read. "Use optimistic color" is not a rule. "Primary gradient stops must be within X-Y hue range, applied only along the primary motion axis" is. If a rule can't be stated precisely enough to encode into the skill layer, it isn't finished.

Ship the engine, not just its output. The deliverable set for every engagement includes the primitives, the token/rule documentation, and the operable skill -- never just hero assets. Hero assets prove the system works; they aren't the system.

## What "done" looks like

A founder or in-house marketer, twelve months after the engagement ends and with zero contact with the agency, can generate a genuinely new asset -- a format that didn't exist at handoff -- that a brand-literate observer would still recognize as unmistakably theirs. If that's not true, the engagement produced a brand kit, not a brand engine.
