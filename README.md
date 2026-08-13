# Brand Engine

A brand you don't have to keep commissioning.

## What this is

A service model for venture-backed, AI-led startups and scale-ups: instead of delivering a static brand kit, we build a brand engine -- a small set of primitives sharing one visual DNA, documented as executable rules, and packaged as an operable AI skill so the client's own team can generate correct, on-brand work indefinitely, without routing every new asset back through a designer.

The model is grounded in how Estudi-Image actually built Stripe's brand refresh and Cursor's OOH campaign (see docs/research.md) -- a small number of primitives, one shared material language, documented well enough to be reusable -- pushed one layer further: the rules are also machine-executable, not just human-readable.

## Repo map

brand-engine/
  docs/
      research.md              case study analysis (Stripe, Cursor) + 2026 market landscape, cited
          methodology.md           the engine framework, plus the skill-chain architecture
              service-offering.md      tiers, process, ideal client profile, pricing logic
                engine/
                    tokens.json               example token set: color, material, motion, geometry
                        index.html                 live interactive demo -- two primitives, one shared DNA
                          skills/
                              _shared/
                                    protocol.md                    the unified triage-diagnose-close discipline every skill follows
                                        brand-engine-hub/                entry -- full system overview, artifact-chain audit
                                            brand-engine-start-here/         entry -- triage a question into the right stage
                                                brand-engine-01-discovery/               stage 1 -- equity, competitors, format inventory
                                                    brand-engine-02-primitive-selection/     stage 2 -- choose 2-4 primitives
                                                        brand-engine-03-dna-definition/          stage 3 -- color/material/motion/geometry tokens
                                                            brand-engine-04-rule-authoring/          stage 4 -- machine-checkable combination rules
                                                                brand-engine-05-asset-production/        stage 5 -- hero assets, prove the system
                                                                    brand-engine-06-skill-encoding/          stage 6 -- package rules as an operable skill
                                                                        brand-engine-07-handoff-training/        stage 7 -- live client test, close the engagement
                                                                            brand-engine-audit/              standing tool -- Tier 1 diagnostic, no engagement required
                                                                                brand-engine-generator/          standing tool -- the client team runs this after handoff

                                                                                ## Start here

                                                                                1. docs/research.md -- why this model, and what it's competing against.
                                                                                2. docs/methodology.md -- the three layers every engine needs, and the skill-chain architecture that delivers them.
                                                                                3. docs/service-offering.md -- how this becomes a service business: tiers, process, positioning.
                                                                                4. engine/index.html -- open in a browser for a live example of the primitive + shared-DNA concept.
                                                                                5. skills/_shared/protocol.md -- the discipline every skill in the chain follows; read this before any individual skill file.
                                                                                6. skills/brand-engine-start-here/SKILL.md -- the actual entry point into the skill chain.

                                                                                ## The core bet

                                                                                Design output used to be scarce, so brand systems were built to be extended by one designer at a time. That's no longer the bottleneck -- startup teams now generate their own components and copy with AI tools faster than any studio can review it. A brand engine is built for that reality: fewer, tighter primitives with rules precise enough that both humans and AI agents can extend the system correctly, at whatever velocity the startup is actually producing at.
