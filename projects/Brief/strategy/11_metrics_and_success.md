# 11 — Metrics and Success

## The north-star metric

**Qualified Second Team leads generated from Brief per month.**

Not signups. Not paid users. Not revenue. **Qualified leads.** Brief's entire purpose is funnel — everything else is instrumentation.

**Target trajectory:**
- Month 3 post-launch: 1 qualified lead
- Month 6: 3 qualified leads
- Month 12: 5–8 qualified leads per month
- Month 18: 8–12 qualified leads per month (approaching Second Team capacity ceiling)

"Qualified" means: someone who completed the paid Brief, booked a consultation, showed up, and left the call with a scope + price discussion underway.

## Secondary metrics (the funnel instrumentation)

### Top of funnel

| Metric | Month 3 Target | Month 6 Target | Month 12 Target |
|---|---|---|---|
| Landing page visitors/mo | 5,000 | 10,000 | 25,000 |
| Signup conversion rate | 5% | 7% | 10% |
| Free signups/mo | 250 | 700 | 2,500 |

### Activation

| Metric | Target | Why it matters |
|---|---|---|
| Interview completion rate (free) | >60% | If users abandon the interview, the UX or the questions are wrong |
| Time to first exported brief | <25 min median | The whole promise is "fast" — if it takes longer, the promise breaks |
| Number of exports per brief | >1.5 avg | Users who export to multiple tools are more engaged |

### Monetization

| Metric | Month 3 | Month 6 | Month 12 |
|---|---|---|---|
| Free → Brief Pro conversion | 3% | 5% | 8% |
| Paid users/mo | ~8 | ~35 | ~200 |
| One-time revenue/mo (at $79) | ~$600 | ~$2,800 | ~$16,000 |
| 14-day refund rate | <10% | <7% | <5% |

### Second Team funnel

| Metric | Month 3 | Month 6 | Month 12 |
|---|---|---|---|
| Paid users → consultation booked | 5% | 7% | 10% |
| Consultations booked/mo | <1 | 2–3 | 20 |
| Consultation → services sale | 15% | 20% | 25% |
| Services revenue from Brief/mo | ~$0 | ~$7.5K | ~$75K |

### Product quality (leading indicators)

| Metric | Target |
|---|---|
| NPS from paid users | >40 |
| "Did Brief visibly improve your AI output?" yes rate | >70% |
| Would recommend to a friend | >60% |
| Brief content referenced on social (brand mentions/week) | >3 |

## Revenue scenarios

### Pessimistic (40th percentile)

- 500 free signups/mo by month 6
- 3% paid conversion = 15 paid/mo = $1,185/mo Brief revenue
- 5% paid-to-consultation = <1 consultation/mo
- ~1 services deal per 2 months at avg $12K = $6K/mo services
- **Total: ~$7,185/mo contribution (~$86K/year)**

**Interpretation:** Worth running, but Brief is mostly a brand-building exercise at this level. Not enough to justify a full-time hire.

### Base case (50th percentile)

- 1,000 free signups/mo by month 6
- 5% paid conversion = 50 paid/mo = $3,950/mo Brief revenue
- 7% paid-to-consultation = 3–4 consultations/mo
- ~1 services deal per month at avg $15K = $15K/mo services
- **Total: ~$19,000/mo contribution (~$228K/year)**

**Interpretation:** A real, self-sustaining lead-gen channel for Second Team. Justifies continued investment.

### Optimistic (75th percentile)

- 2,500 free signups/mo by month 6
- 8% paid conversion = 200 paid/mo = $15,800/mo Brief revenue
- 10% paid-to-consultation = 20 consultations/mo
- 2–3 services deals/mo at avg $20K = $50K/mo services
- **Total: ~$65,800/mo contribution (~$790K/year)**

**Interpretation:** Brief becomes a material revenue contributor to Second Team. At this level, consider hiring dedicated support for the funnel and expanding ICP.

### What I'd tell Jayson

We should plan for the pessimistic case, build toward the base case, and celebrate if we hit the optimistic case. Under no circumstance should Brief's success require the optimistic scenario to be viable.

## Cost budget for year 1

| Category | Monthly | Annual |
|---|---|---|
| Hosting (Vercel + Supabase + services) | $100 | $1,200 |
| LLM API costs (Anthropic) | $300 | $3,600 |
| Scraping (Firecrawl) | $50 | $600 |
| Email delivery (Resend) | $20 | $240 |
| Analytics (PostHog) | $0 (free tier) | $0 |
| Stripe fees (3% of Brief revenue) | ~$50 | ~$600 |
| Landing page / design (one-time) | — | $2,000 |
| Content creation (if outsourced) | $800 | $9,600 |
| Light paid ads (validation) | $300 | $3,600 |
| **Total direct costs** | **~$1,600** | **~$21,440** |
| **Adrian's time (estimate, 10 hrs/week × $150)** | $6,000 | $72,000 |
| **Total all-in (with time cost)** | ~$7,600 | ~$93,440 |

**Breakeven:** Even the pessimistic case ($86K/year contribution) barely covers the all-in cost. The base case ($228K) is comfortably profitable. The math underlines why we need to be disciplined about Adrian's time investment.

## What success and failure look like at 6 months

### Success
- 50+ paid users cumulative
- 2+ Second Team services deals closed
- NPS >40
- Organic traffic starting to grow (content SEO compounding)
- Jayson and Adrian agree: "Brief is worth continuing."

### Failure
- <20 paid users cumulative
- Zero Second Team deals closed
- Refund rate >15%
- Declining week-over-week signups after launch bump
- Jayson and Adrian having "should we kill this?" conversations

### Ambiguous (needs reassessment, not automatic kill)
- Lots of signups, low paid conversion
- Paid conversion fine, no Second Team pipeline
- Strong reviews but slow growth

## Measurement stack

- **PostHog** for product analytics (signup, completion, export, upgrade events)
- **Stripe Dashboard** for revenue + refund tracking
- **Cal.com / Calendly** for consultation booking
- **HubSpot or Notion CRM** for tracking paid-user-to-services pipeline
- **Braintrust or Langfuse** for interview quality evals

## Review cadence

| Cadence | What happens |
|---|---|
| Daily (first 30 days post-launch) | Quick glance at signups, refunds, errors |
| Weekly | Full funnel review, content performance, refund reasons |
| Monthly | Deep review with Jayson: metrics vs targets, decisions for next month |
| Quarterly | Assumption re-validation, roadmap adjustments, kill/pivot conversation |
