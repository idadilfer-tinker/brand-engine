# Research

Grounding for the Brand Engine model: what one studio actually built for Stripe and Cursor, and where the market for this kind of service sits in 2026.

## Case study 1 -- Stripe Brand Refresh (Estudi-Image, 2026)

Stripe's in-house Brand Studio brought in Estudi-Image for an R&D phase on two existing visual motifs: the Wave and the Parallelogram. The brief wasn't "invent a new identity" -- it was "unify what already exists into something that scales."

What they actually built, based on the published case study:

Two primitives, one shared material language. The Wave and Parallelogram are visually distinct shapes, but both live in the same z-space, use the same color palette, and share the same surface/depth quality (light piercing through depth of field, ambient and cinematic). Because the material DNA is shared, the two motifs can be deployed independently or combined without looking like they came from different systems.

Meaning was preserved, not reinvented. The Parallelogram already carried "forward-moving, optimistic, directional" meaning inside Stripe's brand. The studio's job was to give that existing meaning more depth and materiality -- evolution, not replacement.

Guidelines as the actual deliverable. Alongside the hero assets (billboards, cards, phone UI, subway ads, stickers), Estudi-Image produced brand guidelines specifically so Stripe's own team could keep using the Wave and Parallelogram "consistently and intentionally going forward" -- i.e., without the studio in the room.

This is the core insight for the Brand Engine model: the studio's real deliverable wasn't the assets, it was the system that let Stripe's internal team keep producing new assets correctly, indefinitely, without commissioning new work every time.

Source: Stripe Brand Refresh -- Estudi-Image (https://estudi-image.com/projects/stripe-brand-refresh/)

## Case study 2 -- Cursor OOH (Estudi-Image, 2026)

Different problem, same underlying discipline. Cursor (AI coding tool) wanted an out-of-home campaign that didn't market AI as "a shortcut" -- the standard category cliche -- but as a craftsmanship amplifier.

One conceptual rule generated the whole campaign. "Developers paired with parallel disciplines" (conductors, architects, machinists) is a single diptych format that scales across any number of executions without needing a new creative idea per placement.

Positioning against category convention. Most AI tooling brands lead with automation/speed. Cursor's system deliberately did the opposite -- human hands, craft, control -- which is a positioning choice as much as a visual one.

Source: Cursor OOH -- Estudi-Image (https://estudi-image.com/projects/cursor-ooh/)

### What both case studies have in common

A small number of primitives (2 visual motifs; 1 pairing format) governed by an explicit, reusable rule (shared material DNA; diptych logic), documented well enough that the rule -- not just the output -- is transferable. That's the pattern the Brand Engine productizes.

## Market landscape (2026)

The "design system as a service" category is real and active, which validates demand but means positioning matters.

Design tokens as the scaling mechanism. Industry practice in 2026 treats design tokens as the semantic backbone of cross-platform brand automation -- a single core system pushing different "brand skins" to different surfaces. This is the same logic as Stripe's shared material language, generalized into an explicit technical artifact. (Superside: Scaling Design Systems for Brands, https://www.superside.com/blog/scale-design-systems-for-brands)

"Design system is a product, not a project." The framing that's taken hold across agencies serving funded tech companies: a design system isn't a one-time deliverable, it's an ongoing internal product with its own maintenance and versioning. (Superside: Design System Examples 2026, https://www.superside.com/blog/design-systems-examples)

Existing players in this exact niche. Ramotion positions itself explicitly around connecting product design systems to brand systems -- tokens, components, motion, and typography aligned to brand identity, for funded tech companies. Heartbeat and The Branx both target venture-backed startups (seed through Series B/C) across AI, fintech, and SaaS with "scalable identity systems designed to grow with the product." MetaLab is known for translating brand principles into tokens/components/documentation that let internal teams ship without design bottlenecks. (Design System Agencies for Enterprise, 925Studios, https://www.925studios.co/blog/best-design-system-agencies-enterprise-2026; Best Branding Agencies for Startups, Designity, https://www.designity.com/blog/best-branding-agencies-for-startups)

AI as delivery infrastructure, not just subject matter. Generative AI in design was a ~$1.11B market in 2025, projected to reach ~$4.54B by 2030 (31.4% CAGR). The stated precondition for using AI well inside a brand system: the AI has to be trained on the brand's tokens, motion rules, and documentation -- i.e., the system has to already be systematized before AI can extend it reliably. (Evalueserve: AI-Powered Brand Design, https://www.evalueserve.com/blog/ai-powered-brand-design-building-the-future-of-visual-identity-at-scale/)

### The gap this fills

Competitors are converging on "design system as a service" from the product-design side (tokens, components, dev handoff). Almost none of them are wiring the system into an operable AI skill that a founder or growth marketer can invoke directly -- most still route every new asset request back through a designer, even a system-literate one. Given that Claude/Cowork-style AI agents can now execute structured design instructions directly, a brand engine that ships as (a) a documented system and (b) a loadable skill that encodes that system's rules closes the loop Estudi-Image left open for Stripe: guidelines a human reads vs. rules a machine can execute.

## Implication for the offering

Every engine has to ship three layers, not two: the primitives + shared DNA (what Estudi-Image built), the documentation (what Estudi-Image also built, for humans), and a machine-executable rule set (the new layer -- a skill or agent config the client's own team runs to generate compliant assets on demand, without waiting on a designer or the agency).
