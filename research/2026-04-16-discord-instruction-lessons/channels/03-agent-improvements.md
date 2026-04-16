# Channel Summary: #agent-improvements

## Date coverage
- 2026-04-05 to 2026-04-12 verified from current Discord session transcripts

## Why this channel mattered
This was the clearest meta-operations channel. It contains direct lessons about instruction design, runtime mistakes, debugging quality, and progress update quality.

## Main lessons learned

### 1. Docs-only fixes are fake fixes
Observed change:
- an initial pass replaced Claude Code references in skills/docs, but runtime exposure was still wrong
- later correction explicitly called out that the real fix required changing runtime/config behavior, not just text

Why it mattered:
- taught the difference between instruction cosmetics and actual behavioral control
- prevented repeated regressions where the written rule changed but the live tool path did not

### 2. Debug from actual logs, not vibes
Observed change:
- later debugging explicitly checked session/run history instead of guessing why a timeout happened
- over-broad searches across all logs were identified as their own failure mode

Why it mattered:
- made debugging faster and more accurate
- reduced narrative explanations built on the wrong evidence set

### 3. Progress updates need to be sparse and meaningful
Observed change:
- the coding-agent guidance emphasized one start message, then updates only on milestone, blocker, error, or finish

Why it mattered:
- users stop trusting updates when they are constant but low-information
- concise milestone-only reporting made status messages worth reading

### 4. Tight working scope beats sprawling context
Observed change:
- coding-agent guidance increasingly favored focused workdirs, smaller context, and less wandering across unrelated workspace files

Why it mattered:
- reduced meandering and irrelevant file reads
- improved completion speed and relevance

## Durable rules from this channel
- Fix runtime behavior, not just docs.
- Debug from exact logs.
- Keep progress updates milestone-based.
- Constrain scope hard.
