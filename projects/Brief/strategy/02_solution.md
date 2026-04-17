# 02 — The Solution

## One-sentence description

**Brief is a guided interview tool that turns a founder's business into a portable Company Context document they can paste into any AI tool to immediately get sharper, more on-brand output.**

## The user experience in 90 seconds

1. User lands on brief.secondteam.ai, sees a split-screen demo: ChatGPT writing a sales email with generic context vs. the same email written with a Brief attached. The second version is obviously better.
2. User enters their website URL.
3. Brief scrapes the homepage, about page, and pricing page and pre-fills ~40% of the context schema automatically.
4. User walks through a 10-question guided interview (free) or 25-question deep interview (paid) covering positioning, ICP, voice, and red lines.
5. User gets a structured Company Context document they can copy-paste into Claude Projects, ChatGPT custom instructions, Cursor rules, or any other AI tool.
6. At the bottom of the delivered brief: "Want Second Team to build the AI ops stack that uses this? Book a free 30-min consultation."

## What Brief produces

Brief outputs a single structured document (Markdown by default) containing the user's company context, organized into four layers by stability and retrieval pattern:

### Identity layer (rarely changes)
- Mission
- Vision
- Core values
- Origin story
- Red lines (never-say list, never-do list)

### Positioning layer (changes yearly)
- Ideal Customer Profile (firmographic + psychographic + JTBD)
- Anti-ICP (who we don't serve)
- Category and point of view
- Differentiators with proof points
- Competitors and how we're framed against each
- Brand voice (dimensions, vocabulary, sample sentences)
- Messaging hierarchy (primary + pillars + proof)

### Operational layer (changes quarterly)
- Offers, products, pricing
- Business Model Canvas basics
- Current strategic priorities (Rocks / OKRs)

### Evidence layer (append-only)
- Case studies and testimonials
- Golden writing samples ("our best")
- FAQs and objection handling
- Glossary and terms of art

**Note:** Free tier only covers Identity + basic Positioning + basic Voice. Paid tier covers the full schema.

## Why this schema specifically

The schema is borrowed from proven positioning frameworks with explicit rationale for each inclusion:

- **JTBD (Clayton Christensen)** — forces functional/emotional/social split, produces far better hooks than "pain points"
- **Category POV (April Dunford)** — without category framing, AI defaults to generic category averages
- **Voice dimensions (Nielsen Norman 4-axis model)** — numeric scalars steer LLMs more reliably than adjectives
- **Red lines / never-say list** — negative constraints are 2–3x more effective than positive ones for LLM steering
- **Golden samples** — 5–10 labeled samples of "our best writing" enables few-shot steering that beats any style guide
- **Business Model Canvas (Osterwalder)** — familiar, widely taught, non-technical users recognize it

Every component in the schema has a reason. There are no "nice to haves." If we can't explain why an LLM would produce better output with a field than without, it doesn't belong in Brief.

## What Brief is NOT

To stay honest about scope, here's what Brief explicitly will not do in V1:

- ❌ **Generate marketing content.** Brief makes other AI tools better at generating content. It is not a content tool itself. This is what keeps Brief upstream of (and not competitive with) Jasper, Writer, Copy.ai.
- ❌ **Host a chat interface.** Users don't chat with Brief. They fill it out, download their context, and use it inside the AI tools they already love.
- ❌ **Store their business data permanently.** Brief is an onboarding tool, not a CRM or brand management platform.
- ❌ **Integrate with CRMs, CMSs, or analytics.** Not in V1. Maybe never.
- ❌ **Provide strategic consulting.** The interview helps the user articulate what they already know. If they need real strategy help, Second Team services exists for that.

## Why this solution is defensible

**1. Upstream position.** Brief is the first tool a user touches when adopting AI. Every content tool, every agent, every AI app downstream benefits from Brief's output. This is a structural advantage — we're not competing with downstream tools, we're feeding them.

**2. Interview quality as moat.** The 25-question deep interview is the hardest part to get right. It requires positioning expertise, prompt engineering, and months of iteration on what question order produces the best responses. A competitor can copy the schema; they can't copy the interview craft.

**3. Lead-gen business model.** Because Brief's real monetization is Second Team services, we can outcompete on price (one-time $79 vs. $29/mo subscriptions) and feature depth (we don't need to hold features back for a content-generation upsell). Competitors selling Brief as a standalone product can't match this.

**4. Platform-neutral exports.** Jasper, Writer, Copy.ai all want lock-in. Brief is explicitly export-first. This is the opposite of walled-garden positioning and it's uncopyable by incumbents without cannibalizing their own product.

## Why this solution is NOT venture-defensible as a standalone

Equally important to say out loud: if Brief were a standalone startup, I'd be nervous about its moat. Jasper has $180M ARR and is already adjacent. Anthropic and OpenAI both ship company-context features inside their platforms. Notch raised $45M for a related problem.

**Brief only makes sense as a lead magnet for Second Team.** As a standalone SaaS, the competitive density is too high to justify venture investment. As a freemium funnel into a services business, the unit economics are excellent because one converted services client ($5K–$50K) pays for thousands of free users.

This is why the positioning of Brief matters so much: it's not a product, it's a wedge.
