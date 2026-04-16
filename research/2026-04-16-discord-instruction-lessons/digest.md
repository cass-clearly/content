# Digest: What We Learned from Discord About Better Instructions

## Executive summary
Across Discord, the best improvements came from converting general preferences into hard operating rules.

The system got better when we made these shifts:
- from helpful-sounding to execution-specific
- from progress reporting to artifact shipping
- from guessing to verifying
- from broad delegation to constrained delegation
- from implicit channel behavior to explicit wiring and mention rules

## Most important lessons, compressed

- Replace vague instructions with executable ones.
- Done should mean usable, verified, and linked.
- Debug from logs and live paths, not confidence.
- Smaller context produces better delegated work.
- Wandering is a real failure mode.
- Review-ready should be treated as a separate state.
- Explicit IDs beat implied integrations.
- Channel setup is operational work.
- Voice systems improve content quality.
- The best lessons should be committed into the operating files.

## Best tweet-ready bullets

- "Be helpful" is weak. "Ship it, verify it, link it" is strong.
- Many agent failures are scope failures wearing a reasoning costume.
- Docs-only fixes are fake fixes.
- A status update should happen on start, milestone, blocker, or done. Not every five minutes.
- The hardest part of AI ops is defining done honestly.
- Review-ready and publish-ready are different states.
- If a delegate stalls, read the log before you tell a story about why.
- A new channel is not real until it is wired.
- Voice quality improves when it becomes a tracked system, not a vibe.
- If a lesson matters, commit it.

## Channel-specific takeaways

### `#cass-inbox`
- intake surfaces need routing contracts
- inbox handling needs deterministic workflow
- style guides materially improve content fit

### `#car-shopping`
- separate verified facts from inference
- admit unverified inventory plainly
- synthesis beats link dumping

### `#agent-improvements`
- fix runtime behavior, not just docs
- inspect actual logs
- constrain scope
- keep updates sparse and meaningful

### `#general`
- channel wiring and mention policy are first-class rules

### `#knowledge-graphs`
- stalls are often wandering
- architecture should converge earlier
- delegates need intervention rules

### `#lesson-plans`
- completeness is product quality
- honest status is better than fake finish
- teaching usability matters more than raw output volume

### `#lesson-plans-2`
- include direct links automatically
- keep review-ready separate from publish-ready
- make preview windows meaningful
- use explicit Remarq IDs
- define done as live and reviewable

### `#chris-stories`
- use gap tracking
- avoid repeated prompts
- use voice guides for narrative fidelity

### `#remarq` and repo-backed changes
- codify important lessons in git-backed operating files

## Long-form article count
There are **12 strong long-form article candidates** supported by this review.

Top 5:
1. Operational prompts beat aspirational prompts
2. The real definition of done for AI-assisted work
3. Most agent stalls are scope bugs, not reasoning bugs
4. Docs-only fixes are fake fixes
5. Review-ready vs publish-ready
