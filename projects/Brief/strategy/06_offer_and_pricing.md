# 06 — Offer and Pricing

## The pricing philosophy

Brief does not deliver monthly value. It delivers a one-time artifact — a company brief — that a user creates, downloads, and uses. Charging a subscription for this would be dishonest by design, and users would churn as soon as they noticed.

Therefore V1 is **one-time pricing.** Subscription pricing only appears in V2, and only if V2 delivers genuine recurring value (see V2 rationale below).

## V1 offer structure

### Free

| | |
|---|---|
| **Price** | $0 |
| **What they get** | Website scrape + 10-question interview + basic Markdown/ChatGPT/Claude exports |
| **Limits** | 1 brand, 1 brief, no document upload, no advanced schema |
| **Why it exists** | Top-of-funnel. Users should get real value for free so they trust us with paid. |
| **What we get** | Email address, basic profile, AI tool usage data, lead scoring signal |

### Brief Pro — one-time purchase

| | |
|---|---|
| **Price** | **$79 one-time** (recommended; test $49 and $99 in landing page A/B) |
| **What they get** | Everything in free, plus document upload, 25-question deep interview, golden samples, full export suite, case studies, lifetime access to V1 updates |
| **Limits** | 1 brand (additional brands at $39 each or bundled in Team tier later) |
| **Why it exists** | Infrastructure funding + serious-buyer qualification + lead-gen for Second Team |
| **What we get** | $79 revenue + highly qualified lead (see conversion math below) |

### Why $79 and not $29

**$29 feels like an impulse buy.** People pay it, don't complete onboarding, and forget about the product. The checkout conversion rate is slightly higher but the product completion rate is much lower, which means fewer qualified leads for Second Team.

**$79 feels like a real purchase.** People who pay it have committed enough to actually finish the interview. Sunk-cost effect works in our favor: they're more likely to complete, more likely to apply the brief, and more likely to book a Second Team call.

**$79 also respects the category.** Positioning consultants charge $5K+. Compared to that, $79 for an AI-native version of the same artifact is obviously cheap. At $29, users start comparing us to Canva templates.

**$79 also filters for buyer quality.** We want users who take their business seriously enough to invest $79 in getting AI right. Those are the people who later become Second Team clients. Tire-kickers at $29 never convert to $10K engagements.

### Alternative price points to test

- **$49** — lower friction, higher volume; good if landing page test shows strong demand at $79
- **$99** — higher perceived value; test if $79 converts "too easily" (unlikely but possible)
- **Founding customer pricing at $39** — for the first 100 buyers, positioning as "early supporter"; creates urgency and a natural community seed

**A/B test all three on the landing page during the concierge MVP phase.**

## The hidden offer: Second Team services

This is the real monetization. Everything above is surface.

**Inside every delivered brief (free and paid):**

> "Ready to build the AI ops stack that uses this brief?
> Second Team helps founders like you automate their business operations with AI.
> Book a free 30-minute consultation — no pitch, just a conversation about what's possible."
> [Book a call] button

This is the lead capture mechanism. Every brief is a warm introduction to Second Team services.

**Services pricing (not part of Brief, but the thing Brief funnels into):**
- **AI Ops Starter:** $5K–$10K one-time — install Second Team's base AI stack for a founder
- **AI Ops Build:** $15K–$35K — custom automations and workflows
- **AI Ops Retainer:** $2K–$8K/mo — ongoing optimization and expansion

These aren't on the Brief landing page. They're revealed in the consultation call after the user has already engaged with the product.

## Conversion math (unit economics)

Let's run the numbers on a realistic scenario.

**Assume:**
- 1,000 free signups per month (after landing page + organic + light paid)
- 10% convert to Brief Pro at $79 = 100 paid users = **$7,900/mo MRR equivalent**
- 5% of paid users (5/mo) book a Second Team consultation
- 20% of consultations convert to a services engagement (1/mo)
- Average services deal: $15,000

**Monthly outputs:**
- Brief paid revenue: $7,900
- Second Team services from Brief: $15,000
- **Total monthly contribution: ~$22,900**

**Annualized:**
- Brief: ~$95K
- Second Team services from Brief: ~$180K
- **Total: ~$275K/year from Brief funnel alone**

This is not a venture outcome. It is a strong, self-sustaining side-stream that materially adds to Second Team's revenue without distracting from the core business.

**Stress test the math:**
- If free-to-paid converts at 5% instead of 10% → Brief revenue halves, services still roughly similar (most services leads come from paid users, which are more qualified but fewer)
- If services conversion is 10% of paid instead of 5% → services revenue doubles
- If we only hit 500 signups/month → halve everything

Even in pessimistic scenarios (500 signups/mo, 5% free→paid, 10% paid→consultation, 15% consultation→sale), you get ~$40K/yr Brief + ~$60K/yr services = $100K/year. Still meaningfully positive.

## The rationale for NOT charging a subscription

I considered a subscription tier and rejected it. Here's the reasoning preserved for future reference.

**What a subscription tier would have looked like:**
- Brief Pro: $29/mo — full interview + exports + versioning + "keeps your brief updated"

**Why I rejected it:**

1. **Honest pricing builds trust.** A user who pays $29 in month 2 for nothing new will churn and review us badly. Churn on a trust-based lead-gen product is catastrophic.

2. **One-time purchases convert better for this use case.** Cold traffic to a $79 one-time sale converts ~2–4x better than cold traffic to a $29/mo subscription for low-touch digital products (AppSumo data, Product Hunt case studies).

3. **Subscription tier cannibalizes the Second Team funnel.** If users think "I'm already paying $29/mo for Brief," they're less likely to book a $15K services call. One-time pricing keeps the mental budget clear for the real sale.

4. **Subscription SaaS requires ongoing product investment we shouldn't commit to.** A $29/mo customer expects regular updates. Brief's whole point is that it ships one great interview and then funnels. We don't want to be on a feature treadmill.

5. **Claude and ChatGPT now have in-platform memory and projects.** Any "monthly subscription for ongoing context management" is competing with free features inside tools the user already pays for. We lose that fight on price and integration depth.

## V2 subscription rationale (when it makes sense)

A subscription *becomes* honest if — and only if — Brief solves an ongoing, recurring pain that the platforms can't solve for themselves.

**The recurring pain that could justify V2 subscription:**
> "I use 4 AI tools (Claude, ChatGPT, Cursor, Gemini). When I update my positioning, offers, or team, I have to manually update all 4. They drift out of sync and start giving me conflicting advice."

**V2 product: Brief Wiki** (following Karpathy's LLM Wiki pattern)
- Separate product from Brief V1
- $19–$29/mo
- Three compounding operations that justify recurring payment:
  - **Ingest:** Add new sources (case studies, updated pricing, new testimonials) → LLM updates wiki pages, cross-references, and index automatically
  - **Query:** Ask questions against the compiled wiki → synthesized, cited answers; valuable results filed back as new pages
  - **Lint:** Monthly health-check for contradictions, stale claims, orphan pages, data gaps → "context health score"
- MCP-native: when the wiki updates, changes propagate to every connected AI tool
- Obsidian plugin: power users run ingest/lint/query inside their Obsidian vault
- Not "self-learning memory" — Claude and ChatGPT already do that per-tool
- Cross-platform coherence + compounding knowledge are the distinct, defensible jobs

**V1 buyers get Brief Wiki free for 12 months as a goodwill gesture.**

V2 only ships if V1 data shows multi-tool pain. Specifically: if less than 40% of V1 paid users report using 3+ AI tools, V2 is deferred indefinitely or cancelled.

## What to put on the landing page

| Label | Price | Tagline |
|---|---|---|
| Free | $0 | Get unstuck in 20 minutes |
| **Brief Pro** | **$79 one-time** | The full brief, every AI tool, lifetime access |

That's it. Two tiers. No "team," no "enterprise," no "custom." Simplicity converts.

The CTA on the free tier is "Start free." The CTA on paid is "Get Brief Pro — $79." Both point to the same onboarding flow; the upgrade prompt happens after the user finishes the free interview and sees what they're missing.

## Refund policy

**14-day unconditional refund.** No questions. This is non-negotiable for trust on a cold-traffic one-time sale. At $79 and a digital product, refund rates for products like this are typically under 5%. Worth it for trust signal.
