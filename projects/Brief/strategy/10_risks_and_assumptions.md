# 10 — Risks and Assumptions

## The assumptions this whole thing rests on

Writing these out explicitly so we know what we're betting on. If any of these turn out to be wrong, the plan changes.

### Core assumptions (if wrong, whole plan fails)

1. **Entrepreneurs will pay $79 one-time for a 30-minute interview that produces a context document.** Concierge MVP tests this directly.
2. **The output of Brief visibly improves AI tool outputs.** The hero demo test proves this or kills the product.
3. **At least 3–5% of paid Brief users will book a Second Team consultation.** This is the funnel math that makes the whole thing worth it.
4. **Second Team can close 15–25% of consultations into paid services.** This is Second Team's general close rate; needs confirmation from Jayson.
5. **The "cold start" framing resonates with the ICP more than "brand voice" or "context layer" framings.** Landing page test decides this.

### Strong-hold assumptions (likely true but worth verifying)

6. **Most target users actually have 2+ AI tools.** If they only use ChatGPT, Brief's cross-platform value prop weakens.
7. **$79 is the right price point.** $49 might convert better but filter worse; $99 might filter better but lose volume. A/B test.
8. **The 10-question free interview is enough to produce a useful brief.** If users need 15–20 questions to get meaningful output, the free tier doesn't work and we need to rethink.
9. **Users will actually paste the brief into their AI tools after downloading it.** If they download and never use it, there's no aha moment and no word-of-mouth.
10. **The interview is our moat.** If a competitor can replicate our interview quality in 2 weeks with GPT-5, we have no moat.

### Background assumptions (we're not questioning but should flag)

11. **MCP will remain an open standard and won't fragment.** Current trajectory says yes.
12. **Anthropic and OpenAI won't ship a free first-party equivalent in the next 6 months.** They might. Platform risk.
13. **Second Team has the operational capacity to handle inbound leads from Brief.** Open question for Jayson.
14. **Adrian has the time to run concierge MVP and lead early development.** Capacity question.

## Risks ranked by severity × likelihood

### Severity 5 / Likelihood 3 — Platform absorbs our value prop

**What:** Anthropic ships a polished "Claude Business Onboarding" feature inside Cowork. OpenAI ships "ChatGPT Company Setup" inside Projects. Either of these could absorb 60–80% of Brief's value prop overnight.

**Mitigation:**
- Be loudly cross-platform from day one
- Ship the MCP server early (V2) as structural defense
- Accept that Brief might have a 12-month lifespan as a frontend and pivot to "Brief as Second Team's customer onboarding ritual" if platforms absorb the category

**Early warning signals to watch:**
- Anthropic or OpenAI job postings for "context onboarding" PM roles
- Beta features in Claude Cowork for guided business setup
- Product announcements at conferences mentioning "company context" features

### Severity 5 / Likelihood 2 — Concierge MVP shows no willingness to pay

**What:** We run 10 concierge briefs and nobody is willing to pay even $49. Means the business model doesn't work.

**Mitigation:**
- Structure the concierge MVP specifically to detect this within 4 weeks
- Have a fallback plan: if paid doesn't work, can Brief still exist as a pure Second Team lead magnet (free only, no paid tier)?
- Decide the kill criteria before running the test so we don't rationalize a failure

### Severity 4 / Likelihood 3 — Free-to-paid conversion is below 5%

**What:** Users love the free tier but don't upgrade. We have signups but no revenue.

**Mitigation:**
- Strengthen the "what you're missing" upgrade prompt after the free interview
- Test price points ($49/$79/$99)
- Make the free tier deliberately feel incomplete for the specific users who would pay (without being insulting)
- Recognize that low free-to-paid is acceptable if lead-gen for Second Team still works — the paid tier is a qualifier, not the main revenue

### Severity 4 / Likelihood 3 — Paid users don't book Second Team calls

**What:** We generate revenue from Brief Pro but the funnel to services doesn't convert. Brief becomes a standalone $79 product that doesn't serve its strategic purpose.

**Mitigation:**
- Make the Second Team CTA contextual and valuable, not spammy
- Offer something concrete on the consultation (free AI ops audit, specific recommendation)
- If Brief users never convert, either the ICP is wrong for Second Team or the handoff needs redesign — not necessarily a product failure

### Severity 3 / Likelihood 4 — Interview produces mediocre output

**What:** The Brief V1 interview asks the right questions on paper but produces flat, generic-feeling output that users don't find impressive.

**Mitigation:**
- The interview is the moat — invest disproportionate time in prompt engineering and eval curation
- Hire a positioning specialist (ex-StoryBrand, ex-April Dunford practitioner) as a paid consultant for 1–2 weeks to craft the question bank and response rubric
- Build an eval suite early and measure output quality on every release
- Use the concierge phase to refine before automating

### Severity 3 / Likelihood 3 — Adrian has no time to run this alongside Second Team

**What:** The concierge MVP alone takes 40 hours. Building V1 takes more. If Adrian's week is already full with Second Team client work, Brief becomes a zombie project.

**Mitigation:**
- Decide upfront with Jayson how much of Adrian's time is allocated to Brief
- Consider hiring a part-time engineer for the V1 build (the architecture is lightweight; one good engineer at 20 hrs/week can ship in 10 weeks)
- Set a hard deadline: if Phase 0 concierge isn't done by mid-May 2026, revisit whether the project is viable

### Severity 3 / Likelihood 2 — Competitor launches a copy-cat product

**What:** A YC-backed or seed-backed startup ships a similar cold-start context product in Q3 2026.

**Mitigation:**
- Lead-gen business model is our structural advantage — a copy-cat standalone has worse economics
- Interview quality moat holds if we keep investing
- Speed of launch matters: ship V1 before they do
- If a well-funded competitor emerges, pivot Brief to be Second Team-only (stop marketing widely, use it only for closed funnel) and focus Second Team services on what's truly differentiated

### Severity 2 / Likelihood 4 — Scraping and extraction quality is inconsistent

**What:** Firecrawl or our schema extraction returns inconsistent quality across different websites. Users have different pre-fill experiences.

**Mitigation:**
- This is a known weakness of web scraping for unstructured data
- Be transparent: show users what was auto-filled vs. empty, let them correct
- Don't promise 100% auto-fill — promise "head start" and deliver that honestly
- Accept variance; focus the moat on the interview, not the scrape

### Severity 2 / Likelihood 3 — Refund rate higher than expected

**What:** >15% of paid users request refunds within 14 days, hurting unit economics.

**Mitigation:**
- Monitor refund reasons and fix root causes
- If it's "didn't meet expectations," the landing page is overselling — tighten it
- If it's "didn't understand how to use it," the delivery experience needs improvement
- Keep the 14-day refund anyway — trust is worth more than short-term revenue

## Decision-killing scenarios (when we walk away)

We define these upfront so we don't fall prey to sunk-cost thinking later.

**Kill Brief if:**
- Concierge MVP: fewer than 3 of 10 users say the output meaningfully changed AI tool performance
- Concierge MVP: fewer than 3 of 5 paid users pay without friction
- V1 launch: fewer than 50 paid users in the first 90 days
- V1 launch: zero Second Team leads generated from Brief after 6 months
- Platform risk: Anthropic or OpenAI ships a genuinely equivalent feature, measured by whether the user can replicate Brief's output inside their platform for free

Any one of these is reason to pause and reassess. Two or more is reason to wind down.

**Pivot Brief (don't kill) if:**
- Paid tier doesn't convert but free users actively book Second Team calls → drop paid tier, use Brief as pure lead magnet
- Solopreneurs don't buy but agencies do → pivot ICP to small agencies and change pricing
- Cold traffic doesn't convert but Second Team's warm network does → Brief becomes a private tool, not a public product

## The assumption I'm most nervous about

If I had to pick one assumption that keeps me up at night, it's **#3: 3–5% of paid users will book a Second Team consultation.**

This rate is extrapolated from similar B2B lead-magnet funnels, not from Brief's specific data. It could easily be 1%, in which case Brief's strategic purpose doesn't work and it has to survive on the $79 revenue alone. At 1,000 signups/mo × 10% paid × 1% consultation = 1 lead/month. That's thin.

**Mitigation:** Make the consultation CTA extraordinarily compelling. Don't just say "book a call" — offer something concrete like "free 30-min AI ops audit, leave with 3 specific recommendations you can implement this week." That should raise the conversion rate meaningfully.

## Assumption tracking ritual

Every 30 days, review this document and mark which assumptions are:
- ✅ Validated by real data
- 🟡 Still unverified
- ❌ Invalidated (update plan accordingly)

Don't let invalidated assumptions sit in the plan unaddressed. That's the failure mode of most startups — refusing to see when the core thesis breaks.
