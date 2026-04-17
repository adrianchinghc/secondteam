# 05 — Product and Scope

## V1 scope (what we're actually building)

V1 is deliberately minimal. The goal is to ship a usable product within 90 days and start generating leads for Second Team, not to build a feature-complete SaaS.

### Free tier

**Purpose:** Top of funnel. Get the user to the "aha moment" (visibly better AI output) in under 20 minutes. Collect email and basic profile data.

**Features:**
- Enter domain → automated 60-second scrape of homepage, about, pricing, and up to 3 other public pages
- Auto-fill ~30–40% of the schema from scraped content
- **10-question guided interview** covering: mission, core values, primary ICP basics, JTBD, voice dimensions, top 3 differentiators, top 3 competitors, current priorities, elevator pitch, red lines
- **Export formats:** one wiki folder (interlinked Markdown pages — Obsidian-compatible), one consolidated ChatGPT custom instruction block, one Claude Project system prompt
- **1 brand / 1 context document** per account
- Brief branding preserved on exports ("Created with Brief by Second Team")
- Email capture required

**Intentional limits:**
- No document upload
- No golden writing samples
- No case study structured capture
- No deep interview (JTBD functional/emotional/social split, anti-ICP, messaging hierarchy)
- No versioning
- No re-scraping

### Paid tier — "Brief Pro" — $79 one-time (recommended)

**Purpose:** Convert users who finished the free brief and want more depth. Generate the $79 revenue that pays for infrastructure. Qualify for Second Team services.

**Features:** everything in free, plus:
- **Document upload** (up to 10 files): PDFs, decks, Notion exports, Google Docs, brand guides
- **25-question deep interview** including: JTBD functional/emotional/social split, anti-ICP, full messaging hierarchy, Business Model Canvas basics, detailed voice calibration, red lines deep dive
- **Golden writing sample capture** (upload 5–10 pieces of "our best" content for few-shot steering)
- **Structured case study and testimonial capture**
- **All export formats:** Wiki folder (Obsidian vault), JSON, ChatGPT custom instructions, Claude Project prompt, Cursor rules (.cursorrules), Windsurf rules, Custom GPT config file, raw schema
- **Brief branding removable** on exports
- **Lifetime access** to all V1 updates
- **"Book a free 30-min AI ops consultation with Second Team"** prominent CTA in the delivered brief (this is the critical lead-gen mechanism)

### Explicitly out of scope for V1

- ❌ MCP server integration / live sync → V2
- ❌ Team collaboration features → V2
- ❌ Multiple brands per account → V2
- ❌ API access → V3 or never
- ❌ Agency white-label → V3 or never
- ❌ Industry-specific templates → only if V1 data shows it's needed
- ❌ In-app chat / AI assistant → not our category
- ❌ Content generation features → actively refuse; not our category

## The schema in full (what Brief captures)

### Wiki-native folder structure (Karpathy LLM Wiki pattern)

Instead of exporting a single flat Markdown file, Brief V1 exports a **wiki folder** — a set of interlinked Markdown pages with YAML frontmatter, an index, and a log. This structure is Obsidian-compatible out of the box, git-versionable, and designed to compound over time (V2 adds maintenance operations).

The engineering cost of wiki-vs-flat is minimal (~2–3 hours extra). The strategic payoff is significant: users who open their Brief in Obsidian get an instant visual knowledge graph of their company context, and the V2 upgrade path (ingest, lint, query) is seamless because the structure is already in place.

```
brief/
├── index.md                        # Catalog of all pages, organized by layer
├── log.md                          # Chronological record: created, sources used, updates
├── identity/
│   ├── mission-and-vision.md       # Mission, vision, origin story (paid)
│   ├── values.md                   # Core values with behavioral examples
│   └── red-lines.md                # Never-say, never-do, topics to avoid
├── positioning/
│   ├── icp.md                      # Primary ICP: firmographic, psychographic, JTBD
│   ├── anti-icp.md                 # (paid only) Who we don't serve
│   ├── category.md                 # Category, POV, frame of reference
│   ├── differentiators.md          # 3–5 value wedges with proof points
│   ├── competitors.md              # 3–5 competitors, our counter-positioning
│   ├── voice.md                    # 4-axis dimensions, vocabulary, sample sentences
│   └── messaging.md                # (paid only) Primary message, pillars, proof
├── operational/
│   ├── offers.md                   # Products, pricing, guarantees
│   ├── business-model.md           # (paid only) BMC basics
│   └── priorities.md               # Current quarter focus / Rocks
└── evidence/                       # (paid only — entire folder)
    ├── case-studies.md             # Structured: problem/solution/outcome
    ├── testimonials.md             # With attribution and context tags
    ├── golden-samples.md           # 5–10 labeled "our best" pieces
    ├── faqs.md                     # Objection handling pairs
    └── glossary.md                 # Terms of art, product names, definitions
```

**Every page includes:**
- YAML frontmatter: `title`, `layer`, `last_updated`, `sources`, `confidence` (high/medium/low)
- `[[wikilinks]]` to related pages (e.g., `icp.md` links to `offers.md` via "audience_fit")
- A "Why this matters for AI" one-liner at the top explaining what LLMs use this page for

**The `index.md` page** is the entry point for both humans and LLMs. It catalogs all pages by layer and serves as the "paste this into Claude/ChatGPT" consolidated view when the user wants a single-file export. The index is auto-generated from the wiki contents — the user never writes it manually.

**The `log.md` page** tracks when the brief was created, from which sources (scrape, interview, uploaded docs), and any future updates. This follows Karpathy's pattern for auditability and is the foundation for V2's lint operation ("your brief was last updated 3 months ago; here's what's changed on your website since then").

### How the wiki maps to different export targets

| Export target | What gets exported |
|---|---|
| **Obsidian vault** | The full wiki folder, drag-and-drop ready |
| **ChatGPT custom instructions** | Consolidated `index.md` (all layers in one block, optimized for token count) |
| **Claude Project prompt** | Same as ChatGPT but formatted for Claude's system prompt conventions |
| **Cursor / Windsurf rules** | `positioning/voice.md` + `positioning/icp.md` + `operational/priorities.md` (code-context-relevant subset) |
| **Custom GPT config** | Full schema as JSON + instruction block |
| **Raw JSON** | Structured data for developers building on top of Brief |
| **Single Markdown** | `index.md` flattened to one file for users who just want to paste |

This means the wiki is the **source of truth** and every other export format is a *view* compiled from it. One schema, many outputs. Users who don't want a wiki never see it — they just get the ChatGPT/Claude export. Users who want depth get the full vault.

### Schema field detail

The contents of each page follow the same schema as the original design:

**Identity layer** (immutable, rarely changes):
- Mission, Vision, Origin Story (paid), Values (3–7 with behavioral examples), Red Lines (never-say, never-do, topics-to-avoid)

**Positioning layer** (changes yearly):
- ICP Primary: firmographic + psychographic + JTBD (functional/emotional/social — full split paid only) + triggers
- Anti-ICP (paid only)
- Category + POV
- Differentiators (3–5) with proof points
- Competitors (3–5) with counter-positioning
- Voice: 4-axis dimensions (formal↔casual, serious↔funny, respectful↔irreverent, matter-of-fact↔enthusiastic) + vocabulary (prefer/avoid) + sample sentences (paid)
- Messaging Hierarchy (paid only): primary message + 3 pillars + proof points

**Operational layer** (changes quarterly):
- Offers / products / pricing
- Business Model Canvas basics (paid only)
- Current priorities (this quarter)

**Evidence layer** (paid only, append-only):
- Case studies (structured: problem/solution/outcome)
- Testimonials (with attribution)
- Golden writing samples (5–10 labeled pieces for few-shot steering)
- FAQs / objection handling
- Glossary / terms of art

## The interview design (the real moat)

The interview is where Brief wins or loses. A bad interview produces a mediocre schema even with perfect UX. A great interview produces a usable brief from a user who came in with unclear thinking.

### Principles for the interview

1. **Every question has an example answer.** The user should never stare at a blank field.
2. **Every section has a "why this matters" explainer.** The user should understand the point of each field.
3. **Follow-ups are dynamic.** If a user writes "small businesses" as their ICP, Brief asks "what kind — size, industry, stage?" until the answer is specific enough.
4. **Skip logic is aggressive.** If a user has a one-product business, don't ask about product line strategy. Respect their time.
5. **AI-assisted inference, then confirmation.** Brief should *propose* answers inferred from the scrape and let the user confirm or edit. This is faster than writing from scratch.
6. **Progress is always visible.** Users need to feel the brief getting more complete as they go. Use a progress bar and a live preview of the current brief state.
7. **Save on every step.** Users will abandon and return. Auto-save is non-negotiable.

### The 10-question free interview (draft)

1. In one sentence, what does your business do?
2. Who is your primary customer? (With example answers showing specificity levels)
3. What problem are you solving for them that nobody else does well?
4. Who are your top 3 competitors, and how are you different from each?
5. Pick 3–5 words that describe how your brand should sound.
6. Pick 3–5 words that describe how your brand should NEVER sound.
7. What are 3 words or phrases you refuse to use in your marketing? (Red lines — this one is surprisingly powerful.)
8. What are your top 1–3 offers, with pricing?
9. What's your elevator pitch?
10. What are you focused on this quarter?

Each question has a "show me an example" button that reveals 2–3 anonymized example answers from other users. This is the single highest-leverage UX choice — users copy-paste and adapt instead of starting from scratch.

### The 25-question paid interview (outline)

The paid interview expands every free section and adds:
- Full JTBD elicitation with functional/emotional/social split
- Anti-ICP identification
- Origin story interview
- Golden sample capture and voice calibration
- Messaging pyramid (primary → pillars → proof)
- Business Model Canvas walkthrough
- Case study structured capture

Detailed question bank will be drafted in the concierge MVP phase based on what questions actually produce good output when asked.

## V1 architectural decisions

These are lightweight and meant to be shipped in 8–10 weeks max.

- **Frontend:** Next.js + Tailwind + shadcn/ui, deployed on Vercel
- **Backend:** Next.js API routes (no separate service in V1)
- **Auth:** Clerk or Supabase Auth
- **Storage:** Supabase (Postgres + JSONB for the schema)
- **LLM calls:** Direct Anthropic API (Claude) for the interview, structured outputs for schema extraction
- **Crawling:** Firecrawl for V1 (managed service; we can replace later if margins demand)
- **Payments:** Stripe Checkout (one-time payment, no subscription logic needed)
- **Emails:** Resend or Postmark
- **Analytics:** PostHog (free tier covers us for months)
- **Evals:** Braintrust free tier for interview quality testing

Nothing fancy. Anything that requires custom infrastructure is a red flag for V1 scope.

## The concierge MVP (pre-build phase)

Before any code is written, run this in April 2026:

**Week 1:** Write the landing page. Put it up. Capture emails.
**Week 2:** Manually deliver 5 briefs. Each takes ~60–90 minutes of your time. Interview over Zoom or Loom, draft the brief in Notion, email as Markdown. Charge $0 for the first 5 to validate demand; charge $49 for the next 5 to validate willingness to pay.
**Week 3:** Evaluate. Did the 10 users get value? Did any of them express interest in Second Team services? Did the paid 5 pay without resistance?
**Week 4:** Decide. Green light = start building V1. Yellow light = iterate interview script and rerun. Red light = abandon or pivot.

**Total cost:** ~$0 in software, ~40 hours of Adrian's time.

**Learning value:** worth more than any survey. This tells us whether the product has pull before we spend engineering time.
