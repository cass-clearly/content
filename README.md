# Content Pipeline

Automated content drafts generated from dev activity across repositories.

## Structure

- `short-form/` — Tweet-length posts, X threads, quick updates
- `long-form/` — Substack articles, deep dives, tutorials
- `drafts/` — Work-in-progress content not yet categorized

## Workflow

1. Cass generates drafts based on pipeline activity (PRs shipped, bugs fixed, architecture decisions)
2. Drafts land here as markdown files with frontmatter (status, platform, topic)
3. Chris reviews, edits, approves
4. Approved content gets published to X / Substack

## Naming Convention

- `short-form/YYYY-MM-DD-slug.md`
- `long-form/YYYY-MM-DD-slug.md`

## Frontmatter

```yaml
---
title: "Post title"
status: draft | review | approved | published
platform: x | substack | both
tags: [remarq, ai-dev, building-in-public]
date: YYYY-MM-DD
---
```
