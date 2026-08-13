# Brand Engine -- unified skill protocol

Every skill in this system (the two entry skills, the seven stage skills, and
the two standing tools) follows this same protocol. Individual SKILL.md files
reference this document instead of restating it -- read it once, apply it
everywhere.

This pattern is adapted from a strong prior art example: bruiandy's
[brand-first-class-skill](https://github.com/bruiandy/brand-first-class-skill),
a 12-skill system that encodes a brand-strategy course as a routed,
artifact-chained diagnostic. The engagement content is different (visual
brand-engine construction vs. brand strategy), but the discipline is the
same, because the discipline is what makes a skill trustworthy rather than a
keyword-triggered essay generator.

## Why this exists

A skill that answers immediately, from a single message, with a complete
deliverable, is almost always answering from general pattern-matching rather
than the client's actual situation. That's fine for a first draft. It's not
fine for a brand primitive, a token rule, or a client handoff -- those are
expensive to get wrong and expensive to redo. This protocol slows the skill
down on purpose, in the same three moves every time.

## The three moves

Every skill runs through these in order. Not every move takes a full turn --
a well-briefed client can clear triage and diagnosis in one message -- but the
skill should never skip straight to a formal deliverable without having
passed through them.

**1. Triage.** Before doing any work, decide: does this request actually
belong to this skill? If it doesn't -- if it's really a Discovery question
showing up inside DNA Definition, say -- name the skill it belongs to and
route there instead of forcing an answer. Triage also means checking what
upstream artifacts already exist (see Artifact chain, below) so the skill
isn't re-asking questions a prior stage already answered.

**2. Diagnose.** Ask what's actually missing, one question at a time. Never
front-load a questionnaire. Each question should be the single highest-
leverage thing to know next -- the one that would most change the shape of
the eventual output if answered differently. While information is
incomplete, any judgment offered is a **preliminary judgment** and must be
labeled as such, not stated as a conclusion.

**3. Close.** Only produce the formal deliverable once the skill's specific
closure conditions (listed in each SKILL.md) are actually met. If they're
not met yet, keep diagnosing -- don't pad out an incomplete answer to look
finished.

## Distinguish three kinds of statement

Every skill should be able to tell these apart out loud, not just internally:

- **Known fact** -- something the client stated or that's directly observable
  (an existing logo, a stated budget, a named competitor).
- **Working judgment** -- the skill's own inference from known facts. Always
  labeled as a judgment, never presented as settled.
- **Still needs confirmation** -- a real gap. Don't fill it with a plausible
  guess; ask, or flag it as an open risk in the formal output.

## What NOT to do is part of the deliverable

Every formal output must say what not to do next, with the same weight as
what to do next. A brand engine engagement fails as often from doing the
right thing too early (locking primitives before Discovery is done, writing
machine-checkable rules before the DNA tokens are stable) as from doing the
wrong thing.

## The unified output shell

Every skill's formal deliverable -- its "Brief" -- uses this shell. Stage-
specific content differs (see each SKILL.md), but the shell doesn't:

1. **Current judgment** -- the one-paragraph answer to "where does this stand."
2. **Key evidence** -- what it's based on; distinguish known fact from
   working judgment.
3. **Primary thread / tension / priority right now** -- the single thing that
   matters most at this moment, not a list of five.
4. **What not to do yet** -- explicit, not implied.
5. **Recommended next step** -- which skill, and why.
6. **Key conclusions for the next skill to read** -- the specific facts and
   judgments downstream skills need, named so they're easy to extract.

## Artifact chain

The system produces one named Brief per stage. Each stage skill reads every
upstream Brief it can find before asking the client anything, so returning
clients aren't re-diagnosed from zero:

1. `Discovery Brief` -- brand-engine-01-discovery
2. `Primitive Brief` -- brand-engine-02-primitive-selection
3. `DNA Brief` -- brand-engine-03-dna-definition
4. `Rule Brief` -- brand-engine-04-rule-authoring
5. `Asset Brief` -- brand-engine-05-asset-production
6. `Skill Brief` -- brand-engine-06-skill-encoding
7. `Handoff Brief` -- brand-engine-07-handoff-training

`brand-engine-audit` produces its own standalone `Audit Brief`, usable
before an engagement exists at all. `brand-engine-generator` doesn't produce
a Brief -- it's a standing execution tool a client's team uses after
`Handoff Brief` closes, and it reads the live token file directly rather
than the artifact chain.

## Routing rules common to every skill

- If the client doesn't know where to start, route to
  `brand-engine-start-here`, not to stage 1 by default -- a returning client
  might belong at stage 4.
- If the client wants a full-system overview, an audit of where an existing
  engagement stands, or a check on whether the artifact chain is intact,
  route to `brand-engine-hub`.
- No stage skill does another stage's job, even when it would be faster to
  just answer. Name the right skill and stop.
