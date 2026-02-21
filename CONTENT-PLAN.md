# Content Operations Plan

## Chris Salvato — Building in Public

*Generated: 2026-02-20*

---

## Table of Contents

1. [Content Pillars](#content-pillars)
2. [Content Calendar — 50+ Pieces](#content-calendar)
3. [Pipeline Operations Design](#pipeline-operations-design)
4. [Posting Cadence](#posting-cadence)
5. [Ambient Content Agent Design](#ambient-content-agent-design)
6. [First Week — Ready to Draft](#first-week)

---

## Content Pillars

### Pillar 1: Building Remarq in Public
The story of building an open-source browser extension for web annotations — from fork to product. Architecture decisions, browser extension quirks, shipping in public with AI assistance.

**Key themes:**
- Product decisions (why fork Hypothesis? why AGPL + dual license?)
- Technical deep dives (content scripts, sidebar injection, toast systems, dark mode)
- The marketing page rewrite journey
- Open source strategy and community building
- Browser extension ecosystem (Manifest V3, Chrome Web Store, cross-browser)

### Pillar 2: AI-Assisted Development (The Meta-Story)
The autonomous dev pipeline — an ambient agent that triages GitHub issues, plans implementations, ships PRs via Claude Code, with a review agent that enforces staff-level code review. The messy, honest reality.

**Key themes:**
- How the pipeline actually works (cron → issue triage → branch → implement → PR → review agent → merge)
- Claude Code in production: what it's good at, where it fails
- The review agent pattern (spawning a fresh agent for adversarial code review)
- Permission systems, git workflow enforcement, automation debugging
- Honest metrics: what percentage of PRs actually merge cleanly?
- The content pipeline itself (meta-meta: AI writing about AI writing)

### Pillar 3: Engineering Leadership & Career
From the book — the hidden curriculum of staff+ engineering. Frameworks, stories, contrarian takes.

**Key themes:**
- The LEAD framework (Locate → Envision → Architect → Deliver)
- Hidden curriculum vs. visible curriculum
- Why switching companies beats chasing promotions
- Tuckman's model applied to engineering teams (storming → performing)
- Staff vs. Senior Staff vs. Principal: living in different "spaces"
- Agency over intelligence — mindset over skillset
- Managing up, managing down, managing sideways
- Why shipping slow can beat shipping fast

### Pillar 4: Hot Takes & Commentary
Timely observations on the AI/dev tooling landscape, browser extensions, engineering culture.

**Key themes:**
- AI coding tools: hype vs. reality
- Browser extension ecosystem problems
- Engineering hiring, culture, team dynamics
- The "more people = more velocity" fallacy
- Open source business models

---

## Content Calendar — 50+ Pieces

### Pillar 1: Building Remarq in Public

| # | Title / Hook | Platform | Format | Priority | Dependencies |
|---|---|---|---|---|---|
| 1 | "I forked Hypothesis and rebuilt it as Remarq. Here's why." | X | Thread (8-10 posts) | 🔴 HIGH | Screenshot of old vs new |
| 2 | "We shipped 20 PRs in 48 hours. None of them were written by a human." | X | Thread (6-8 posts) | 🔴 HIGH | PR count data from repo |
| 3 | "The first thing I did was delete TODO.md" | X | Tweet | 🟡 MED | Link to PR #52 |
| 4 | "Why I chose AGPL + dual licensing for an open source dev tool" | Substack | Long-form (1500w) | 🟡 MED | None |
| 5 | "Browser extension bundle size: 174KB and climbing. Here's my plan." | X | Thread (4-5 posts) | 🟡 MED | Bundle analysis screenshot |
| 6 | "Content scripts are a nightmare. Here's what I learned injecting a sidebar into every webpage." | Substack | Long-form (2000w) | 🟡 MED | Code snippets |
| 7 | "Dark mode for browser extensions is harder than you think" | X | Thread (5-6 posts) | 🟢 LOW | PR #105 merged |
| 8 | "I wrapped my entire extension init in try/catch. Here's the bug that made me do it." | X | Tweet + screenshot | 🔴 HIGH | PR #114 |
| 9 | "Replacing alert() dialogs with a toast system in a browser extension" | X | Thread (4 posts) | 🟡 MED | PR #111 |
| 10 | "Mobile web annotations don't work. Here's why and what I'm trying." | X | Thread (5 posts) | 🟡 MED | Issue #115 |
| 11 | "Thread-aware status filtering: a small API change that unlocked huge UX improvements" | X | Tweet | 🟢 LOW | PR #29 |
| 12 | "Why I killed the 'Author Mode' and replaced it with an inline AI button" | X | Thread (4 posts) | 🔴 HIGH | PR #24 |
| 13 | "Lazy loading a sidebar that injects into every page on the internet" | X | Thread (5 posts) | 🟡 MED | PR #118 |
| 14 | "The Remarq marketing page rewrite — from developer docs to actual product page" | Substack | Long-form (1500w) | 🟡 MED | Before/after screenshots |
| 15 | "Open Graph tags: the thing your side project is missing" | X | Tweet | 🟢 LOW | Issue #112 |
| 16 | "Building a browser extension in 2026: the state of the ecosystem" | Substack | Long-form (2500w) | 🔴 HIGH | Research |
| 17 | "E2E testing browser extensions — here's what actually works" | X | Thread (6 posts) | 🟡 MED | PR #119 progress |
| 18 | "Why I'm building annotation tools when Hypothesis already exists" | LinkedIn | Post (300w) | 🔴 HIGH | None |

### Pillar 2: AI-Assisted Development

| # | Title / Hook | Platform | Format | Priority | Dependencies |
|---|---|---|---|---|---|
| 19 | "I built an autonomous dev pipeline. It checks a project board, picks issues, writes code, opens PRs, and reviews its own work." | X | Thread (10-12 posts) | 🔴 HIGH | Architecture diagram |
| 20 | "The review agent pattern: why I spawn a fresh AI to adversarially review every PR" | X | Thread (6-8 posts) | 🔴 HIGH | CLAUDE.md excerpt |
| 21 | "My AI agent shipped 20+ PRs. Here's what the diffs actually look like." | Substack | Long-form (2000w) | 🔴 HIGH | PR screenshots |
| 22 | "Claude Code doesn't know when to stop. Here's how I constrain it." | X | Thread (5-6 posts) | 🔴 HIGH | Examples |
| 23 | "The messy reality of AI-assisted development: a 48-hour log" | Substack | Long-form (3000w) | 🔴 HIGH | Detailed log |
| 24 | "'Just use AI' — my honest breakdown of what works and what doesn't after shipping a real product with it" | X | Thread (8-10 posts) | 🔴 HIGH | None |
| 25 | "Fail-fast patterns: why I made my AI agent remove default passwords instead of using them" | X | Tweet | 🟡 MED | PR #51 |
| 26 | "The git workflow I enforce on my AI: branch → implement → PR → review → merge. No exceptions." | X | Thread (5 posts) | 🟡 MED | CLAUDE.md |
| 27 | "AI code review > human code review. Fight me." | X | Tweet (hot take) | 🔴 HIGH | None |
| 28 | "I use AI to write content about using AI to write code. The meta-pipeline." | X | Thread (4 posts) | 🟡 MED | Content repo link |
| 29 | "Why I target 80-90% test coverage, not 100% — and why my AI agent agrees" | X | Tweet | 🟡 MED | CLAUDE.md excerpt |
| 30 | "The cron-based ambient agent: how I built a system that works on my project while I sleep" | Substack | Long-form (2000w) | 🔴 HIGH | Architecture diagram |
| 31 | "Permission systems for AI agents: what happens when your bot has push access" | X | Thread (6 posts) | 🟡 MED | None |
| 32 | "Error handling patterns I learned from watching an AI write code all night" | X | Thread (5 posts) | 🟡 MED | PR #113, #114 examples |
| 33 | "The AI didn't write a single test until I told it to. Lessons on AI agency." | X | Tweet | 🟡 MED | None |
| 34 | "OpenClaw: the ambient AI infrastructure I'm building on" | LinkedIn | Post (400w) | 🟡 MED | None |

### Pillar 3: Engineering Leadership & Career

| # | Title / Hook | Platform | Format | Priority | Dependencies |
|---|---|---|---|---|---|
| 35 | "There's a hidden curriculum in software engineering. Nobody talks about it." | X | Thread (10 posts) | 🔴 HIGH | Book intro |
| 36 | "LEAD: the 4-phase framework that separates Staff engineers from Senior engineers" | X | Thread (8-10 posts) | 🔴 HIGH | Book Ch. 1 |
| 37 | "Most engineers are trapped in the Deliver phase. Here's why that's a ceiling." | X | Thread (6 posts) | 🔴 HIGH | LEAD framework |
| 38 | "Why switching companies is almost always better than chasing promotions" | X | Thread (8 posts) | 🔴 HIGH | Book content |
| 39 | "The Stardew Valley model of software engineering" | Substack | Long-form (2000w) | 🔴 HIGH | Book Ch. 1 |
| 40 | "My guidance counselor said I wasn't smart enough to be an engineer. 17 years later..." | X | Thread (6-8 posts) | 🔴 HIGH | Book intro, personal story |
| 41 | "Staff Engineer ≠ Senior Engineer who ships more code" | X | Tweet | 🔴 HIGH | None |
| 42 | "The Tuckman model is the most underrated framework in engineering leadership" | X | Thread (8 posts) | 🟡 MED | Book chapter on teams |
| 43 | "Stop saying 'more engineers = more velocity'. Here's the math." | X | Thread (6 posts) | 🔴 HIGH | Book content |
| 44 | "Why I'm writing a book on staff+ engineering" | Substack | Long-form (1500w) | 🔴 HIGH | Book draft |
| 45 | "Agency over intelligence: the #1 trait I look for in engineers" | X | Thread (5 posts) | 🔴 HIGH | Karpathy tweet ref |
| 46 | "Principal Engineers live in Problem Space. Staff lives in Solution Space. Senior lives in Execution Space." | X | Tweet (with visual) | 🔴 HIGH | Diagram |
| 47 | "How I went from near-failing to Summa Cum Laude — and what it taught me about engineering" | LinkedIn | Post (500w) | 🟡 MED | Book intro |
| 48 | "The competence trigger: why engineers who understand team dynamics get promoted faster" | X | Thread (6 posts) | 🟡 MED | Book chapter |
| 49 | "Shipping slow is sometimes better than shipping fast. Here's when." | X | Tweet | 🟡 MED | None |
| 50 | "I shattered a sales record in 6 months by reading every sales book I could find. Here's what that taught me about engineering." | X | Thread (5 posts) | 🟡 MED | Book intro |
| 51 | "Protect your performing teams. Don't 'spread the talent.'" | X | Tweet | 🟡 MED | Book content |
| 52 | "Managing up as a Staff IC: how to tell your EM they're wrong (without getting fired)" | Substack | Long-form (1500w) | 🟡 MED | Book content |
| 53 | "The PSHE framework for navigating engineering orgs" | X | Thread (6 posts) | 🟡 MED | Book outline |

### Pillar 4: Hot Takes & Commentary

| # | Title / Hook | Platform | Format | Priority | Dependencies |
|---|---|---|---|---|---|
| 54 | "The browser extension ecosystem is broken. Here's what needs to change." | X | Thread (6 posts) | 🔴 HIGH | Remarq experience |
| 55 | "Manifest V3 was supposed to make extensions better. It made them worse." | X | Tweet | 🟡 MED | None |
| 56 | "AI coding tools in 2026: what's real and what's vaporware" | Substack | Long-form (2000w) | 🔴 HIGH | Research |
| 57 | "Hot take: most 'AI-powered' dev tools are just GPT wrappers with a $20/mo subscription" | X | Tweet | 🟡 MED | None |
| 58 | "The web annotation space is wide open. Here's why nobody's won it yet." | X | Thread (5 posts) | 🟡 MED | Market research |
| 59 | "Open source licenses nobody understands: AGPL edition" | X | Thread (4 posts) | 🟢 LOW | None |
| 60 | "Engineering culture red flags I've seen at companies from startups to Shopify" | X | Thread (8 posts) | 🟡 MED | Experience |

---

## Pipeline Operations Design

### GitHub Project Board Structure

**Board:** `Content Pipeline` (GitHub Projects v2 on cass-clearly/content)

**Columns (Status field):**

| Column | Description |
|---|---|
| **Backlog** | Ideas captured, not yet prioritized |
| **Ready to Draft** | Researched, outlined, source material identified — agent can pick this up |
| **Drafting** | Agent or Chris is actively writing |
| **In Review** | Draft complete, waiting for Chris to review |
| **Approved** | Chris approved, ready to publish |
| **Published** | Live on platform |

**Labels:**

| Label | Color | Description |
|---|---|---|
| `tweet` | blue | Single tweet |
| `thread` | blue | X thread (multi-post) |
| `linkedin` | blue | LinkedIn post |
| `substack` | blue | Substack article |
| `pillar:remarq` | green | Building Remarq in Public |
| `pillar:ai-dev` | purple | AI-Assisted Development |
| `pillar:leadership` | orange | Engineering Leadership |
| `pillar:hot-take` | red | Hot Takes & Commentary |
| `priority:high` | red | Ship this week |
| `priority:medium` | yellow | Ship within 2 weeks |
| `priority:low` | gray | Whenever |
| `needs-screenshot` | pink | Requires visual asset |
| `needs-data` | pink | Requires metrics/data |
| `ready-to-write` | green | All dependencies met, can be drafted |

### Workflow Rules

1. **New issue → Backlog** by default
2. **Move to Ready to Draft** when: all dependencies are met (screenshots taken, data gathered, source material linked)
3. **Ambient agent picks up** issues in "Ready to Draft" column (oldest first, highest priority first)
4. **Agent drafts** → creates a markdown file in the repo under `short-form/` or `long-form/`, opens a PR, moves issue to "In Review"
5. **Chris reviews** → approves, requests changes, or rejects
6. **Approved** → Chris publishes manually (or via Typefully API in future)
7. **Published** → issue closed, PR merged

---

## Posting Cadence

### Weekly Target

| Platform | Frequency | Type |
|---|---|---|
| X (tweets) | 5-7/week | Mix of standalone tweets and thread components |
| X (threads) | 2-3/week | Deep dives, frameworks, stories |
| LinkedIn | 1-2/week | Leadership content, career insights |
| Substack | 1/week | Long-form deep dive |

### Weekly Rhythm

| Day | Primary Content | Secondary |
|---|---|---|
| Monday | Substack article publishes | Tweet promoting it |
| Tuesday | X thread (AI dev or Remarq) | LinkedIn post |
| Wednesday | Standalone tweets (2-3) | — |
| Thursday | X thread (leadership/career) | — |
| Friday | Building in public update (week recap) | LinkedIn cross-post |
| Saturday | Hot take or commentary tweet | — |
| Sunday | Buffer / catch-up | — |

---

## Ambient Content Agent Design

### How It Mirrors the Dev Pipeline

The Remarq dev pipeline works like this:
1. **Cron schedule** checks the GitHub project board for issues in "Ready" column
2. **Agent picks an issue**, reads the spec, creates a branch
3. **Agent implements**, commits, opens a PR
4. **Review agent** is spawned to adversarially review
5. **Merge on approval**

The content pipeline mirrors this exactly:

1. **Cron schedule** (daily at 6 AM MT) checks the content project board for issues labeled `ready-to-write` in "Ready to Draft" column
2. **Agent picks the highest-priority issue**, reads the issue body for: platform, format, key points, source material
3. **Agent drafts content** as a markdown file with proper frontmatter:
   - Reads STYLE.md for voice/tone guidelines
   - Pulls source material (book excerpts, PR descriptions, commit logs)
   - Writes draft in the specified format and word count
   - Creates branch `content/YYYY-MM-DD-slug`
4. **Agent opens a PR** with the draft, links the issue, moves issue to "In Review"
5. **Notification** sent to Discord channel for Chris to review
6. **Chris reviews** → approves/requests changes via PR comments
7. **On merge** → issue auto-closes, content moves to "Published"

### Trigger Sources

| Trigger | What It Creates | Example |
|---|---|---|
| PR merged in Remarq | "Building in public" tweet or thread | PR #117 merged → tweet about toast notifications |
| Issue closed in Remarq | Technical deep dive opportunity | Issue #73 (bundle size) closed → thread about optimization |
| Weekly cadence | Substack article, recap thread | Every Monday |
| Book chapter completed | Leadership thread + Substack excerpt | Chapter on Tuckman → thread |
| News/event | Hot take tweet | New AI tool launch → commentary |
| Manual | Chris adds an issue directly | Any format |

### Agent Prompt Template

```
You are a content writer for Chris Salvato's personal brand.

Read STYLE.md for voice and tone guidelines.
Read the linked issue for: platform, format, key points, source material.

Write a draft that:
- Matches the specified platform format exactly
- Uses Chris's voice (direct, contrarian, experience-backed)
- Includes a strong hook in the first line
- Is the specified word count ± 10%
- References real examples from his work (PRs, code, experiences)

Output as a markdown file with proper frontmatter.
```

### Integration Points

| System | Integration | Status |
|---|---|---|
| GitHub Issues | Source of truth for content pipeline | ✅ Ready |
| GitHub Projects | Kanban board for status tracking | 🔲 To set up |
| Discord (#content channel) | Notifications when drafts are ready for review | 🔲 To set up |
| Typefully API | Future: auto-schedule approved tweets/threads | 🔲 Future |
| Remarq repo webhooks | Auto-create content issues when PRs merge | 🔲 Future |
| Logseq | Mine for ideas and source material | ✅ Available via qmd |

---

## First Week — Ready to Draft

These 7 pieces are fully specified and ready for the ambient agent to pick up on day one:

### Day 1 (Monday) — Substack Launch
**"I Built an Autonomous Dev Pipeline. Here's What Actually Happened."**
- Platform: Substack
- Format: Long-form (2500w)
- Key points: Architecture overview, the cron → issue → PR → review flow, honest metrics, what surprised you
- Source: CLAUDE.md from Remarq, PR history, pipeline architecture

### Day 2 (Tuesday) — X Thread
**"I forked Hypothesis and rebuilt it as Remarq. Here's why."**
- Platform: X thread (8-10 posts)
- Key points: Why Hypothesis wasn't enough, what changed, AGPL licensing decision, the vision
- Source: Remarq README, PR #38 (removing Hypothesis refs), PR #30 (marketing rewrite)

### Day 3 (Wednesday) — Standalone Tweets
**Tweet 1:** "The first thing I did on my new project was delete TODO.md and migrate everything to GitHub Issues. If your task tracker isn't where your code lives, you're doing it wrong."
**Tweet 2:** "I wrapped my entire browser extension init in try/catch. The bug that made me do it was breaking every page on the internet."

### Day 4 (Thursday) — X Thread
**"There's a hidden curriculum in software engineering. Nobody talks about it."**
- Platform: X thread (10 posts)
- Key points: Visible vs hidden curriculum, LEAD framework intro, why grinding tickets is a ceiling
- Source: Book intro + Chapter 1

### Day 5 (Friday) — Building in Public Recap
**"Week 1 building Remarq in public. Here's what shipped:"**
- Platform: X thread (5-6 posts)
- Key points: PR count, features shipped, what the AI did vs what Chris did, next week's goals
- Source: This week's merged PRs

### Day 6 (Saturday) — Hot Take
**"Hot take: AI code review is already better than most human code review. The AI actually reads every line."**
- Platform: X tweet
- Key points: Provocative but backed by real experience with the review agent pattern

### Day 7 (Sunday) — LinkedIn
**"Why I'm building annotation tools when Hypothesis already exists"**
- Platform: LinkedIn (400w)
- Key points: Market gap, open source strategy, the intersection of AI + annotations
- Source: Remarq vision, product decisions

---

## Appendix: Source Material Index

| Source | Location | Content Type |
|---|---|---|
| Engineering Book | `/tmp/engineering-book.pdf` | Leadership frameworks, career stories, contrarian takes |
| Remarq CLAUDE.md | `cass-clearly/remarq/CLAUDE.md` | Pipeline spec, git workflow, review agent pattern |
| Remarq PRs | `gh pr list -R cass-clearly/remarq` | Technical decisions, code changes, implementation details |
| Remarq Issues | `gh issue list -R cass-clearly/remarq` | Product roadmap, technical debt, feature ideas |
| Logseq Graph | `qmd query -c logseq` | Personal ideas, "Become Renowned" theme, AI agent ideas |
| Content STYLE.md | `cass-clearly/content/STYLE.md` | Voice, tone, formatting guidelines (TO BE CREATED) |
