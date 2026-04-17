# 01 — The Problem

## The cold-start problem

Every entrepreneur who opens Claude, ChatGPT, Cursor, or any AI tool for the first time hits the same wall: **the AI doesn't know who they are.** It doesn't know their business, their customers, their offers, their voice, or their non-negotiables. So they either:

1. Give up after generic outputs,
2. Paste their website URL and hope,
3. Type three generic sentences and settle for mediocre results, or
4. Spend hours crafting a "system prompt" they never refine.

The result is that the most powerful productivity tools in the world underperform for the people who would benefit most — solo founders and small teams — because the *context layer* is missing.

## Why this is actually a hard problem

It looks trivial ("just write a system prompt"), but it isn't. Getting the context right requires the user to have clear answers to questions most entrepreneurs have never explicitly articulated:

- Who is my ideal customer, specifically (not just "small businesses")?
- What job are they hiring my product to do?
- What's my brand voice — and what do I *never* want to sound like?
- What are the 3–5 things that differentiate me from my competitors?
- What are my current priorities this quarter vs. my long-term vision?
- What are my red lines — things I refuse to say or do?

These are positioning and strategy questions. Most founders don't have answers to them until they've been forced to. And without answers, no amount of "better prompting" produces good AI output.

## Why this is urgent in 2026

Three things have changed in the last 18 months that make this problem acute:

**1. Context engineering is now the recognized discipline.** Karpathy, Tobi Lütke, and Gartner have all declared that "context engineering is in, prompt engineering is out." Users are being told they need a context layer but nobody's handing them one.

**2. Context Rot research (Chroma, 2025) proved that bigger context windows aren't a substitute for better context.** Claude Opus 4.6 has a 1M-token window but performance still degrades past ~30K tokens on complex tasks. Users need *the right* context, not *all* of it.

**3. The average SMB using AI seriously now uses 3–5+ AI tools.** Each one has its own context surface (ChatGPT Projects, Claude Projects, Cursor rules, Windsurf rules, custom GPTs, etc.). Users are writing the same company info into 5 different places and watching them drift out of sync.

Source: web search verification, April 2026.

## Who feels this pain the most

- **Solo founders and solopreneurs** building their first AI-assisted workflows
- **Fractional CMOs and solo marketers** managing AI content for multiple clients
- **Small agencies** trying to standardize AI output across teammates
- **Early-stage teams (2–10 people)** onboarding to Claude/ChatGPT for the first time

Note that this is **not** the enterprise pain point. Writer.com and Notch already serve regulated enterprises with compliance-heavy context management. Our target is explicitly the under-resourced entrepreneur who has no ops team, no brand strategist, and no time to write a 30-page brand book.

## What users try today (and why it fails)

| Workaround | Why it fails |
|---|---|
| Paste website URL into ChatGPT | Pulls surface-level marketing copy, misses JTBD, voice, red lines |
| Write a "system prompt" from scratch | Requires positioning clarity the user doesn't have |
| Copy-paste blog posts about "good prompts" | Generic templates, not company-specific |
| Use ChatGPT Projects with a Company Context Doc | Right idea, but user still stares at a blank page; also locked to one tool |
| Hire a positioning consultant | $5K–$50K, weeks of delay, produces a PDF not a portable artifact |
| Use Jasper Brand IQ / Writer Infobase | Only works inside Jasper/Writer; doesn't export to Claude/ChatGPT/Cursor |

The closest substitute is "ChatGPT Projects + a Company Context Doc you write yourself." That's the real competitor. Brief needs to beat it on **time-to-first-value** and **quality of structured output**, because that's what the beginner actually cares about.

## The emotional problem underneath the functional one

Users don't just want better AI output. They want to feel like **they're not wasting the potential** of these tools. Most entrepreneurs have a nagging sense that AI could be transforming their business and they're only scratching the surface. That frustration — "I know this could be 10x more useful, I just don't know how" — is the real motivator. Brief needs to convert that frustration into a concrete, completable action.

## The problem Brief is NOT solving

To keep the scope honest, here's what we are deliberately leaving out:

- ❌ We are not solving "AI content generation" — that's Jasper, Copy.ai, Writer.
- ❌ We are not solving "enterprise compliance and governance" — that's Writer, Notch.
- ❌ We are not solving "cross-tool data sync" in V1 — that's V2, maybe.
- ❌ We are not solving "sales enablement data enrichment" — that's Clay, Persana.
- ❌ We are not solving "AI agent orchestration" — that's LangChain, CrewAI, n8n.

Brief solves **one thing**: help an entrepreneur produce a usable Company Context document in under 30 minutes without needing a positioning strategist. Everything else is out of scope.
