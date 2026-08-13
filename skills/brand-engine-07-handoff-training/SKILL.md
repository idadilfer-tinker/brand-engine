---
name: brand-engine-07-handoff-training
description: >
  Use to close a Brand Engine engagement: walk the client team through
  generating a genuinely new asset live, using brand-engine-generator,
  before the engagement ends. Produces the Handoff Brief, the last artifact
  in the chain, and the go/no-go decision on whether the engine actually
  meets the "done" bar from docs/methodology.md. Not for producing the
  skill file itself (that's brand-engine-06).
---

# Stage 7 -- Handoff and training

Read `../_shared/protocol.md` first. See "What 'done' looks like" in
`docs/methodology.md` for the bar this stage tests against.

## What this is for

An engine isn't done when the skill file is written -- it's done when the
client's own team can use it, unsupervised, on a request the engine has
never seen before. This stage is the live test of that, not a formality.

## Triage

If no Skill Brief exists, route back to `brand-engine-06-skill-encoding`
first.

## Diagnosis

- Pick a format that genuinely didn't exist at handoff -- not one already
  proven in stage 5. This is the actual test; reusing a proven format
  doesn't test anything new.
- Have a member of the client's own team (not the studio) run
  `brand-engine-generator` on that request, live, with minimal prompting
  from the studio.
- Did the output comply with the rule set without a studio judgment call
  fixing it after the fact?
- Would a brand-literate outside observer recognize the output as
  unmistakably this brand's, per the "done" bar in `docs/methodology.md`?

If the live test fails, that's real signal, not a formality to route
around -- diagnose whether the failure is in the skill encoding (route back
to stage 6) or in the rule set itself (route back to stage 4).

## Closure conditions

Only produce the Handoff Brief once:

- A live, client-run test has actually happened -- not a hypothetical
  walkthrough.
- The test used a genuinely novel format or request.
- The result meets or explicitly falls short of the "done" bar, with the
  gap named if it falls short.
- The client knows how to invoke `brand-engine-generator` themselves going
  forward, including how to update the token file if it changes.

## Formal artifact: Handoff Brief

Use the shared output shell. Stage-specific content:

- **Current judgment**: pass or explicit gap against the "done" bar.
- **Key evidence**: what was tested, who ran it, what the output was.
- **Primary thread**: if there's a gap, whether it's a skill-encoding issue
  or a rule-set issue.
- **What not to do yet**: don't close the engagement on a hypothetical
  walkthrough; don't paper over a failed live test as "close enough."
- **Recommended next step**: engagement closes, or route back to stage 6
  or 4 depending on where the gap traces to. If closing, offer Tier 4
  Retainer per `docs/service-offering.md`.
- **Key conclusions for the client**: this Brief is the engagement's own
  closing record -- keep it, since it's the reference point for any future
  `brand-engine-hub` audit of this same brand.
