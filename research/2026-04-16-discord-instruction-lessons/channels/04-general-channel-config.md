# Channel Summary: #general and channel wiring lessons

## Date coverage
- 2026-04-06 to 2026-04-14 verified from current Discord session transcripts

## Why this channel mattered
This is where channel-level operating behavior became explicit instead of assumed.

## Main lessons learned

### 1. A new Discord channel is not real until it is wired
What improved:
- new channels were added to config and restarted properly
- response behavior was no longer assumed from mere server membership

Why it mattered:
- prevented silent deafness
- made channel availability deterministic

### 2. Mention behavior must be intentional
What improved:
- some channels were configured to respond without mentions
- others later moved toward requiring mentions

Why it mattered:
- channel norms differ
- explicit mention policy prevents accidental spam or accidental silence

### 3. Channel setup is operational work, not metadata
What improved:
- channel creation plus config patch plus verification became the real checklist

Why it mattered:
- this closed the gap between "channel exists" and "assistant can actually behave correctly there"

## Durable rule from this channel
- Treat channel wiring and mention policy as first-class operating rules.
