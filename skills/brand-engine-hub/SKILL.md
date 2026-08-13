---
name: brand-engine-hub
description: >
  Use when someone wants a full overview of how the Brand Engine skill
  system fits together, wants to know which of the seven stage skills an
  engagement currently sits at, wants to check whether the artifact chain
  (Discovery through Handoff Briefs) is intact or has a broken link, or
  wants a system-level retrospective on a stalled or resumed engagement.
  Not for answering a specific stage's question directly -- this skill
  routes, it doesn't diagnose primitives, tokens, or rules itself.
---

# Brand Engine -- method hub

Read `../_shared/protocol.md` first. This skill follows that protocol; it
does not restate it.

## What this is for

This is not another stage and it doesn't replace `brand-engine-start-here`.
Its job is system-level: show how the seven stage skills, the two standing
tools, and the artifact chain relate, and figure out where a given
engagement actually stands right now.

Good fits: "how does this whole skill system work," "what's the
relationship between the seven stages," "I have some Briefs already, where
should I pick back up," "something feels broken in this engagement, help me
find where."

Not a fit: a specific question that belongs inside one stage (route to that
stage or to `brand-engine-start-here` instead), or a request to actually
produce a primitive, token set, rule, asset, or skill file (those are the
stage skills' jobs, not this one's).

## Modes

**Overview mode** -- the client is asking how the system works in general,
with no specific engagement in mind yet. Explain the shape: two entry
skills, seven sequential stages, two standing tools, one Brief per stage.
Point them at `brand-engine-start-here` if they have an actual question.

**Audit mode** -- the client has an engagement in progress, with some Briefs
already produced. Read every Brief that exists. Check: is the chain
continuous (does each Brief's "key conclusions for the next skill" actually
get used by the Brief after it), or is there a gap -- a stage that was
skipped, or a Brief that contradicts an earlier one? Report the break
plainly; don't paper over it.

**Retrospective mode** -- the engagement stalled or the client is returning
after a gap. Same as audit mode, plus: name what's stale (token values or
market context that may have moved on) and what's still valid.

Don't force a client into overview mode when they clearly need audit mode,
or vice versa -- triage which one applies from their first message before
picking a mode.

## Closure conditions

Only produce the formal `Method Brief` once:

- The client's need is classified as overview, audit, or retrospective.
- Every existing upstream Brief has been read.
- The chain's continuity (or specific break point) is known.
- The next recommended stage skill is known.
- What should *not* be opened yet is known (e.g., don't jump to
  brand-engine-06-skill-encoding if the DNA Brief was never actually closed).

## Formal artifact: Method Brief

Use the shared output shell from `../_shared/protocol.md`, with this
stage-specific content in slot 6 (key conclusions for the next skill):

- Which stage skill to enter next, and why.
- Which Briefs already exist and are trustworthy vs. which are stale or
  incomplete.
- The single most important thing the next skill should read before asking
  the client anything.

## Routing

- No prior Briefs, no clear question yet -- `brand-engine-start-here`.
- Chain intact, client knows their next question -- route directly to that
  stage skill.
- Chain broken -- route back to the stage where it broke, not forward.
- Client wants to check if an existing brand (no active engagement) is
  engine-ready -- `brand-engine-audit`, not this skill.
