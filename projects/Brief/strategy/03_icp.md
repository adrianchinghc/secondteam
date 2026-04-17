# 03 — Ideal Customer Profile (ICP)

## Primary ICP: "The Overwhelmed Operator"

### Who they are

A founder, solopreneur, or fractional executive running a small business (often solo, up to ~10 people) who is AI-curious, sometimes AI-enthusiastic, but feels they're not getting the full value out of the tools they've tried.

### Firmographic

- **Role:** Founder / owner / fractional CMO / solo consultant / agency owner
- **Company size:** 1–10 people
- **Revenue:** Usually $100K–$2M annual, sometimes pre-revenue
- **Industry:** Services-first (agencies, consultants, coaches, SaaS founders, content creators, e-commerce operators) — any industry where the person sells expertise or brand, not pure commodities
- **Geography:** English-first (North America, UK, Australia, SEA English-speakers) for V1
- **Tech posture:** Has used ChatGPT or Claude for at least 3 months; has tried at least 2 AI tools; hasn't built anything serious yet

### Psychographic

- **Beliefs:** "AI will change my business. I just haven't figured out how yet."
- **Fears:** Falling behind competitors who are "using AI properly." Wasting money on tools they don't use. Looking foolish in front of clients or team.
- **Aspirations:** Running a lean, high-leverage operation. Being the "AI-forward" person in their network. Using AI to do the work of a team they can't yet afford.
- **Self-image:** Resourceful, hands-on, builder-type. Not a developer but not afraid of tools. Watches YouTube tutorials and reads Substack.
- **Spending pattern:** Will spend $30–$200 on a one-time tool that solves a concrete pain. Allergic to new monthly subscriptions; already has too many.

### Jobs-to-be-done

**Functional job:** "Help me get better output from the AI tools I already use."

**Emotional job:** "Stop making me feel stupid when I open a blank ChatGPT window and don't know what to tell it."

**Social job:** "Let me show my team/peers/clients that I'm using AI professionally, not just playing with it."

### Triggers that make them buy

- They just subscribed to a new AI tool (ChatGPT Plus, Claude Pro, Cursor, etc.) and hit a wall within the first week
- They saw a competitor or peer post about their "AI stack" and felt behind
- They read a Substack/newsletter about context engineering and realized they don't have a context layer
- They tried to write a system prompt for Claude Projects, stared at it for 20 minutes, and gave up
- They're about to hire Second Team (or a similar agency) and want to arrive prepared

### Where they live

- Substack (business / AI newsletters — "The Neuron," "Ben's Bites," "Lenny's Newsletter")
- Twitter/X (AI commentary accounts, indie hacker community)
- LinkedIn (fractional CMO community, solopreneur hashtags)
- YouTube (productivity and AI channels)
- Reddit (r/ChatGPT, r/ClaudeAI, r/entrepreneur, r/SaaS)
- Podcasts (My First Million, Indie Hackers, The Founder Hour)

## Secondary ICP: "The Small Agency Owner"

### Who they are

Owner of a small digital agency (2–15 people) who wants to standardize how their team uses AI across client projects.

### Why they're secondary, not primary

They have a harder pain (multiple clients, team consistency, onboarding new hires) but a more complex purchase decision (team license, seat management, training). Build for them in V1 only to the extent they look like the primary ICP — defer team features to V2.

### What they care about specifically

- **Reusing briefs across clients** (agency uses Brief for each of their clients)
- **Consistency across team members** when they use AI tools
- **Onboarding new hires** to a client's context in minutes rather than days
- **Selling AI-assisted services** without looking ad-hoc

## Anti-ICP: who we explicitly don't serve

Writing this out matters. Every hour spent trying to please an anti-ICP is an hour not spent winning the primary ICP.

- ❌ **Large enterprises.** Writer, Notch, and Jasper already serve this segment. We lose.
- ❌ **Regulated industries needing compliance.** Writer and Notch. We lose.
- ❌ **Pure developers building custom LLM apps.** LangChain, Instructor, custom schemas. We're not technical enough. They're not our users.
- ❌ **Marketing teams at Fortune 5000 companies.** Jasper Enterprise. We lose.
- ❌ **Someone looking for an AI content generator.** We're not a content tool.
- ❌ **Someone with no existing AI tool usage.** Brief only makes sense if you already use ChatGPT/Claude/Cursor. We don't evangelize AI — we optimize it.

## ICP sanity check: a day in their life

Imagine **Sarah**, 34, runs a 5-person content marketing agency serving DTC e-commerce brands. She subscribed to ChatGPT Team for her team 6 months ago. Her designer uses it for subject lines, her strategist uses it for briefs, she uses it for client emails. Each of them writes their own context from scratch each time. The output is inconsistent. One of her junior team members got called out last month for a tone-deaf email that ChatGPT drafted for a client.

Sarah has been meaning to "build a brand voice thing" for the agency. She opened a Google Doc two months ago titled "ChatGPT Brand Guidelines." It has three bullet points. She closed it.

**Sarah is Brief's primary ICP.** Everything in the product should be designed so Sarah finishes the onboarding in under 30 minutes and leaves with something she can paste into her team's ChatGPT and feel proud about.

## ICP validation questions for the concierge MVP

The first 10 concierge users should be screened against these questions:

1. "How many AI tools do you currently pay for?" (Target: 2+)
2. "When was the last time you tried to write a 'system prompt' or 'custom instructions' for an AI tool?" (Target: within the last 3 months)
3. "Do you feel like your AI tools know your business?" (Target: no)
4. "Have you ever tried to write a brand voice doc or context doc and not finished?" (Target: yes)
5. "What would you pay one time for something that solved this in 30 minutes?" (Target: $40+)

If the first 10 users don't answer these as expected, the ICP framing is off and we need to revise before building.
