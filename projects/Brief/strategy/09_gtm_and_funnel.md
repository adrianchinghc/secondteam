# 09 — Go-to-Market and Funnel

## The funnel in one diagram

```
Cold traffic (content + organic + light paid)
         ↓
Landing page with hero demo (split-screen ChatGPT before/after)
         ↓
Free signup → 20-minute interview + scrape
         ↓
Free brief delivered (Markdown + ChatGPT + Claude exports)
         ↓
Upgrade prompt → $79 Brief Pro
         ↓
Paid brief delivered with "Book a call with Second Team" CTA
         ↓
Second Team consultation (free, 30 min, no pitch)
         ↓
Services engagement ($5K–$50K)
```

Each step has a specific conversion target (see [11_metrics_and_success.md](./11_metrics_and_success.md)).

## The hero demo (most important marketing asset)

Before anything else works, the landing page hero demo must produce a visible, undeniable difference in output quality between "ChatGPT without Brief" and "ChatGPT with Brief."

**The demo:**
- Split screen, side by side
- Same prompt to ChatGPT on both sides: "Write a sales email to a new lead introducing our business."
- Left side: no context. Generic, wrong tone, wrong audience framing.
- Right side: Brief pasted into custom instructions. Specific, on-voice, audience-aware.
- A "see another example" toggle cycles through different content types: email, landing page hero, social post, cold DM.

**If the demo isn't instantly compelling, nothing else in marketing matters.** We test this before writing any other marketing copy. Run it past 10 people and ask "does the right side look noticeably better?" If fewer than 8 say yes, iterate the demo until they do.

## Acquisition channels (ranked by likely ROI)

### 1. Content-led SEO (primary, long-term)

**What:** Long-form content about the cold-start problem, context engineering, and the "system prompt trap."

**Target keywords:**
- "how to write a system prompt for ChatGPT"
- "best brand voice prompt for Claude"
- "company context ChatGPT"
- "ChatGPT Projects brand voice setup"
- "Cursor rules for solo founders"
- "how to make ChatGPT sound like my brand"

**Why this works:** Every one of these queries is made by Brief's ICP, and most of the top results today are thin blog posts. A well-written, actually-useful article with a "download your brief with Brief" CTA should convert well.

**Cadence:** 1 article per week for first 3 months, then 2 per month. Each article takes 2–4 hours.

### 2. Product Hunt launch (one-shot)

**When:** Week 1 of V1 launch (July 2026 target).

**Prep:**
- The hero demo as a video (under 90 seconds)
- 3 "making of" posts in the week before launch to warm the community
- A specific founder testimonial from the concierge MVP phase

**Why:** PH isn't the volume channel it used to be, but for developer- and indie-hacker-adjacent products it still drives ~1,000–5,000 visitors in a day. Worth doing once.

### 3. Twitter/X native (high effort, high variance)

**What:** Adrian and Jayson posting Brief's point of view — the "context engineering is real, here's how to do it" narrative — with occasional product demos.

**Why:** The AI indie hacker crowd lives on X. A single viral thread can produce 500+ signups.

**Cadence:** 3–5 posts per week, 1 thread every 2 weeks. Budget 30 min/day.

### 4. Newsletter partnerships

**Targets:** The Neuron, Ben's Bites, Lenny's Newsletter, The Rundown AI, Superhuman's newsletter, smaller indie hacker lists.

**Pitch:** "Free tool that solves the cold-start problem for your readers — will you feature it?"

**Why:** These newsletters are always looking for concrete, useful tools to share. Brief is giveable content.

### 5. Light paid ads (for validation only)

**What:** $500–$1,500 on LinkedIn ads targeting fractional CMOs, solopreneurs, and agency owners. Not a scaling channel — a validation channel.

**Purpose:** Confirm landing page conversion rates before investing in organic content. If paid converts at <3%, the landing page needs work before organic efforts scale.

### 6. Reddit and community seeding (organic only)

**Targets:** r/ChatGPT, r/ClaudeAI, r/entrepreneur, r/SaaS, r/indiehackers.

**Rule:** No promotional posts. Only comment in threads where someone is specifically asking for help with AI context / custom instructions / brand voice, and the answer genuinely includes Brief.

**Why:** Reddit is rabidly anti-promotion but rewards genuine help. 1–2 good comments per week is enough.

### 7. Second Team existing network (warm)

**What:** Post to Adrian's and Jayson's existing LinkedIn networks, Second Team client base, and any founder communities they're in.

**Why:** Warm traffic converts 5–10x better than cold. First 100 users should come from here.

## The handoff from Brief to Second Team (the critical path)

This is the single most important part of the GTM and the thing most likely to be executed sloppily. Nail this.

### Inside the delivered brief

At the bottom of every paid brief, a section titled:

> **"What's next?"
> You've built the foundation. Here's what to do with it:
> 1. Paste the Claude Project block into your Claude projects
> 2. Paste the ChatGPT custom instructions into Settings → Personalization
> 3. Paste the Cursor rules file into your project repos
>
> If you want help installing this into a complete AI ops stack — workflows, automations, agent setups — Second Team does this for a living. Book a free 30-minute call, no pitch, just a conversation about what's possible for your business.
>
> [Book a call]"

### The consultation flow

1. User books a 30-minute call via Calendly or Cal.com
2. Call is with Adrian, Jayson, or a qualified Second Team team member
3. Agenda: 5 min intro, 15 min listening to user's business, 10 min walking through "here's what Second Team could build for you" — specific, concrete, quoted
4. No hard sell. The goal is to leave the user feeling that Second Team understood their business and could obviously help.
5. Follow-up email within 24 hours with a proposal outline (not a full scope doc — just "here's what we'd build and what it would cost")

### Lead scoring

Not every Brief user should be pushed toward Second Team. Score leads based on their interview answers:

- **Hot lead (push toward Second Team aggressively):** Company revenue $500K+, already uses 3+ AI tools, has specific use cases in mind, current priority mentions AI or automation
- **Warm lead (mention Second Team but don't push):** Company revenue $100K–$500K, uses 1–2 AI tools, open to help but not clearly ready
- **Cold lead (let them self-serve):** Pre-revenue, tinkerer, just exploring — don't waste consultation time here; stay friendly and nurture via email

**Score the lead automatically based on the interview answers.** Surface the call-to-action differently for each tier. Hot leads see "Book a call" prominently; cold leads see a softer "Join our newsletter."

## Launch sequence (first 30 days after V1 is live)

| Day | Action |
|---|---|
| Day 1 | Product Hunt launch, X announcement thread, Second Team network post |
| Day 2–7 | Daily X updates, 1 long-form article, email to concierge MVP users for testimonials |
| Day 8 | First newsletter feature pitches sent |
| Day 10 | LinkedIn Ad test: $500 budget, one creative, target fractional CMOs |
| Day 14 | Second article published, Reddit soft presence begins |
| Day 21 | First retrospective: measure conversions, iterate landing page |
| Day 28 | Decide on content cadence for month 2 based on actual data |

## GTM sanity check

If by end of month 3 post-launch we don't have:
- 500+ email signups
- 30+ paid users
- 1+ Second Team consultation booked

…then the GTM isn't working and we need to stop and reassess rather than push more traffic through a leaky funnel.

## What we won't do

- ❌ Cold outbound sales (wrong price point, wrong motion)
- ❌ Paid Google Ads (too expensive per click, wrong intent)
- ❌ Affiliate programs (too early; no product-market fit to amplify)
- ❌ Conferences / events (too expensive, wrong scale)
- ❌ Press releases (dead channel)
- ❌ Influencer partnerships (fake for a cold-start product)
