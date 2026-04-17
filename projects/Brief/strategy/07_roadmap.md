# 07 — Product Roadmap

## Philosophy

Every phase has a **decision gate** — a specific metric or signal that must be hit before proceeding to the next phase. If the gate isn't met, we iterate or pivot, not push forward.

## Phase 0: Concierge MVP (April 2026, ~4 weeks)

**Goal:** Validate that users want this enough to pay for it, and that delivering it produces usable output.

**Scope:**
- Landing page (Framer or simple Next.js) with hero demo, two-tier pricing, email capture
- No product. The "product" is a Notion doc template + Adrian + Claude
- Manual delivery: user fills a form → Adrian runs a 60–90 min Zoom interview → Claude drafts the brief → Adrian reviews and sends via email within 48 hours
- First 5 users: free, in exchange for feedback
- Next 5 users: $49 (founding price), to validate willingness to pay

**What we measure:**
- Landing page signup rate (target: >5% visitor → signup)
- % of signups who actually complete the interview (target: >50%)
- % of free users who say "I would have paid $79 for this" (target: >30%)
- % of paid users who actually pay without friction (target: >80% of invoiced)
- Number of users who ask about Second Team services unprompted (target: >1 out of 10)

**Decision gate to Phase 1:**
- ✅ At least 5 of 10 users finished the interview
- ✅ At least 3 of 10 said the output changed how their AI tools performed
- ✅ At least 3 of 5 paid users paid without friction
- ✅ At least 1 user asked about Second Team services

If these hit → build V1. If not → iterate the interview script and rerun for 5 more users.

## Phase 1: V1 Launch (May–July 2026, ~8–10 weeks)

**Goal:** Ship the first automated version of Brief with free and paid tiers. Begin generating leads for Second Team.

**Scope:**
- Core product (Next.js + Supabase + Stripe + Firecrawl + Anthropic API)
- Free tier: scrape + 10-question interview + basic exports
- Paid tier ($79 one-time): full interview + doc upload + all export formats + Second Team CTA
- Landing page with hero demo (the split-screen ChatGPT comparison)
- Email delivery of briefs
- Stripe Checkout integration
- Basic analytics (PostHog)

**Out of scope for V1:**
- MCP server integration
- Team features
- Multi-brand accounts
- API access
- White-label
- Industry templates

**What we measure (first 90 days after launch):**
- Monthly signups (target: 500 in month 3)
- Free → paid conversion (target: 5–10%)
- Paid → Second Team consultation (target: 3–5%)
- Consultation → services sale (target: 15–25%)
- 14-day refund rate (target: <10%)
- Net Promoter Score from paid users (target: >40)

**Decision gate to Phase 2:**
- ✅ At least 100 paid users within 90 days of launch
- ✅ At least 3 Second Team services engagements sourced from Brief
- ✅ 40%+ of paid users report using 3+ AI tools (required for V2 viability)

If these hit → build V2 Brief Wiki. If not → keep optimizing V1, or wind down Brief as a failed experiment (with lessons captured).

## Phase 2: V2 — Brief Wiki (Q4 2026, only if gate is met)

**Goal:** Turn Brief from a one-time compilation into a living, compounding company knowledge base — following Karpathy's LLM Wiki pattern (April 2026).

### The core insight driving V2

V1 produces the initial compilation. But businesses change — new offers, updated pricing, fresh testimonials, evolved positioning. A static brief goes stale within 3–6 months, and stale context is worse than no context because it makes LLMs confidently wrong.

V2 adds the three LLM Wiki maintenance operations that keep the brief alive:

**1. Ingest (ongoing):** User adds new sources — a case study, a new product page, a testimonial, a competitor update, an updated pitch deck. Brief's LLM reads the source, updates the relevant wiki pages, adds cross-references, and logs the change. One source typically touches 5–10 wiki pages.

**2. Query:** "What's our current positioning against Competitor X?" or "Generate a summary of our last 3 case studies." Brief answers from the compiled wiki, not from raw dumps. Valuable query results can be filed back as permanent wiki pages.

**3. Lint:** Monthly automated health-check that flags contradictions ("your pricing page says $99/mo but your offers.md says $79"), stale claims ("your priorities.md hasn't been updated in 4 months"), orphan pages, missing cross-references, and data gaps. Surfaces a "context health score" to the user.

### Why this justifies a subscription (when V1 doesn't)

V1 is a one-time compilation — the value is delivered once. V2 is ongoing maintenance — the value genuinely compounds month over month. The user isn't paying for the same thing they already have; they're paying for the LLM bookkeeping that keeps their wiki current, cross-referenced, and lint-clean. This is the honest subscription test: "would the user notice if we stopped providing this next month?" For V2, the answer is yes — their brief would start drifting.

### Scope

- Brief Wiki as a separate product ($19–$29/mo)
- Ingest operation: upload new sources → LLM updates wiki pages, cross-references, index, log
- Query operation: ask questions against the compiled wiki → synthesized answers
- Lint operation: monthly automated health-check → "context health score" + suggested fixes
- MCP server per account — Brief becomes an MCP-compatible context source for any connected tool
- Cross-platform sync: when the wiki updates, changes propagate to connected Claude/ChatGPT/Cursor
- Diff view: every update shows what changed, when, from what source
- **Obsidian plugin** (stretch): ingest, lint, and query operations running inside the user's Obsidian vault — no web app needed for power users
- V1 paid users get Brief Wiki free for 12 months

### What V2 deliberately does NOT do

- ❌ **Self-learning from AI tool interactions.** Claude's automemory and ChatGPT's saved memories already handle within-tool learning. We don't compete with that. Brief Wiki is about *user-directed* updates, not passive surveillance.
- ❌ **Bidirectional sync from AI tools back to Brief.** Privacy and noise concerns. The user controls what goes into the wiki; the wiki distributes outward. One-way.
- ❌ **Fully automatic context updates without user confirmation.** Trust problem. Bad auto-updates poison the brand voice across every connected tool. Every update is proposed, then confirmed.
- ❌ **Team management.** Defer to V3.

### The Obsidian angle

For users already in Obsidian, V2 has a dramatically simpler UX path: install the Brief Obsidian plugin. The plugin connects to their Brief account and runs ingest/lint/query directly inside their vault. No separate web app, no context switching — the wiki lives where they already work.

This also opens a distribution channel: the Obsidian community (~4M+ users, heavy overlap with Brief's ICP) is the ideal organic audience for a "living company wiki" product. Plugin marketplace listing + community posts = free distribution.

For users NOT in Obsidian, the web app handles all the same operations. Obsidian is a power-user fast lane, not a requirement.

### What we measure

- % of V1 paid users who activate Brief Wiki during free year (target: >20%)
- Average ingests per user per month (target: >2 — signal of genuine ongoing use)
- Lint health score distribution (target: >60% of users above "healthy" threshold)
- MCP connections per user (target: >2 tools — validates cross-platform thesis)
- % who continue paying after free year (target: >50%)
- MRR from subscribers (target: $5K/mo after 6 months)
- Service deals sourced from Brief Wiki users (target: continuous, higher per-user than V1)

### Decision gate to Phase 3

- Real MRR ($10K+) from Brief Wiki
- Demonstrated retention past first year
- Average user ingesting new sources at least monthly (wiki is actually compounding, not abandoned)

## Phase 3: V3 — Team and Agency (2027, only if Phase 2 works)

**Goal:** Open a higher-revenue tier for small agencies and teams managing multiple briefs.

**Possible scope:**
- Team accounts with seat-based pricing
- Multiple briefs per account (one per client)
- Agency white-label
- API access
- Obsidian marketplace listing for Brief Wiki plugin (if V2 validates the Obsidian channel)
- Industry-specific context templates marketplace
- Public Brief directory (opt-in, like "context packs" other users can borrow from)

**Why this is "only if":** V3 doubles the product complexity. It should only happen if V1 and V2 produce meaningful revenue, and if agency owners are specifically asking for it with their wallets.

## What we explicitly will NOT build (across all phases)

- Content generation features (Jasper's category)
- Brand asset management (Frontify's category)
- CMS integrations (Contentful's category)
- Chat interface (ChatGPT's category)
- Compliance / governance suite (Writer's category)
- Full agent orchestration (LangChain's category)
- AI training / fine-tuning
- Marketplace for prompts or system prompts

Every one of these has been a graveyard for "AI brand kit" startups. We stay small, stay upstream, stay a funnel.

## Summary timeline

| Phase | Timing | Milestone |
|---|---|---|
| Phase 0: Concierge | April 2026 | 10 manual briefs, $245 paid revenue, go/no-go decision |
| Phase 1: V1 Launch | May–July 2026 | Public launch, first 100 paid users, first 3 Second Team leads |
| Phase 2: V2 Brief Wiki | Q4 2026 (if gate met) | Subscription product: ingest/lint/query, MCP-native, Obsidian plugin |
| Phase 3: V3 Team/Agency | 2027 (if gate met) | Multi-brand, team features, possible API |

## The biggest risk to the roadmap

**Shipping Phase 1 late.** Every month of delay past July 2026 is a month Anthropic Cowork, OpenAI Projects, or a well-funded competitor gets closer to eating the cold-start problem. The single most important thing for Phase 1 is **shipping on time**, even if feature-incomplete.

A 60% version of Brief in July is worth more than a 95% version in October.
