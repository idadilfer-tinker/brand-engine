# Brand Engine

A brand you don't have to keep commissioning.

## What this is

A service model for venture-backed, AI-led startups and scale-ups: instead of delivering a static brand kit, we build a **brand engine** -- a small set of primitives sharing one visual DNA, documented as executable rules, and packaged as an operable AI skill so the client's own team can generate correct, on-brand work indefinitely, without routing every new asset back through a designer.

The model is grounded in how Estudi-Image actually built Stripe's brand refresh and Cursor's OOH campaign (see docs/research.md) -- a small number of primitives, one shared material language, documented well enough to be reusable -- pushed one layer further: the rules are also machine-executable, not just human-readable.

## Repo map

brand-engine/
- docs/
-   - research.md            case study analysis (Stripe, Cursor) + 2026 market landscape, cited
    -   - methodology.md         the engine framework: primitives, DNA, rule set, skill layer
        -   - service-offering.md    tiers, process, ideal client profile, pricing logic
            - - engine/
              -   - tokens.json            example token set: color, material, motion, geometry
                  -   - index.html             live interactive demo -- two primitives, one shared DNA
                      - - skills/
                        -   - brand-engine-generator/
                            -     - SKILL.md           example Claude Skill that encodes an engine's rules so a client team can generate on-brand assets on demand
                         
                            - ## Start here
                         
                            - 1. docs/research.md -- why this model, and what it's competing against.
                              2. 2. docs/methodology.md -- the three layers every engine needs: primitives + DNA, documented rules, operable skill.
                                 3. 3. docs/service-offering.md -- how this becomes a service business: tiers, process, positioning.
                                    4. 4. index.html -- open in a browser (or via GitHub Pages) for a live example of the primitive + shared-DNA concept.
                                       5. 5. skills/brand-engine-generator/SKILL.md -- a template for the machine-executable layer; swap in a real client's tokens and rules to make it live.
                                         
                                          6. ## The core bet
                                         
                                          7. Design output used to be scarce, so brand systems were built to be extended by one designer at a time. That's no longer the bottleneck -- startup teams now generate their own components and copy with AI tools faster than any studio can review it. A brand engine is built for that reality: fewer, tighter primitives with rules precise enough that both humans and AI agents can extend the system correctly, at whatever velocity the startup is actually producing at.
