# Brief — Strategy Index

**Owner:** Adrian
**Partner review:** Jayson
**Last updated:** 2026-04-11
**Status:** Pre-build / concept validation

---

## What this folder is

This is the strategy documentation for **Brief** — a freemium lead-generation product for Second Team. Brief helps entrepreneurs create a Company Context Layer (company brief) that dramatically improves the quality of output from AI tools like Claude, ChatGPT, Cursor, and others.

The docs below capture the thinking, rationale, and open questions behind the product. They exist to:

1. Get Adrian and Jayson aligned before any build work starts
2. Serve as the source of truth for anyone who joins the project later
3. Force clarity on decisions that would otherwise be hand-waved

---

## One-paragraph summary

Most entrepreneurs who start using AI tools hit the same wall on day one: the AI has no idea who they are, what they sell, who their customers are, or how they speak. They paste a URL, type three generic sentences, and get generic output. Brief solves the cold-start problem by walking a user through a guided interview plus a website scrape and producing a portable Company Context document they can paste into any AI tool. It's free to start, one-time paid for depth, and its real purpose is to qualify leads for Second Team's done-for-you AI ops services.

---

## How to read these docs (in order)

1. [01_problem.md](./01_problem.md) — The cold-start problem, why it matters, why now
2. [02_solution.md](./02_solution.md) — What Brief is, what it does, what it deliberately is not
3. [03_icp.md](./03_icp.md) — Who we're building for (and who we're not)
4. [04_positioning.md](./04_positioning.md) — Category, POV, messaging, naming rationale
5. [05_product_and_scope.md](./05_product_and_scope.md) — V1 scope, free vs paid, what's in/out
6. [06_offer_and_pricing.md](./06_offer_and_pricing.md) — Pricing logic, one-time vs subscription
7. [07_roadmap.md](./07_roadmap.md) — V1 → V2 → V3, with decision gates
8. [08_market_and_competitors.md](./08_market_and_competitors.md) — Landscape as of April 2026, verified via web search
9. [09_gtm_and_funnel.md](./09_gtm_and_funnel.md) — How we get users, how they become Second Team leads
10. [10_risks_and_assumptions.md](./10_risks_and_assumptions.md) — What could kill this, what we're betting on
11. [11_metrics_and_success.md](./11_metrics_and_success.md) — What "working" looks like
12. [12_open_questions_for_jayson.md](./12_open_questions_for_jayson.md) — Decisions we need to make together
13. [13_first_90_days.md](./13_first_90_days.md) — Concrete plan, week by week

---

## Decision status

| Decision | Status | Notes |
|---|---|---|
| Build Brief as Second Team lead magnet (not standalone SaaS) | ✅ Decided | Adrian, confirmed 2026-04-11 |
| One-time pricing for V1 | ✅ Decided | Subscription would be dishonest for a static artifact |
| Defer MCP sync to V2 | ✅ Decided | Build after V1 proves multi-tool pain |
| Name the product "Brief" | 🟡 Proposed | Pending Jayson sign-off |
| Price point for paid tier ($49 / $79 / other) | 🟡 Proposed | Recommend $79; test in landing page |
| Concierge MVP before code | ✅ Decided | 10 manual briefs before any engineering |
| Launch deadline | 🟡 Proposed | Public landing page by end of April 2026 |
| Who owns delivery / support | 🔴 Open | Needs Jayson discussion |

Legend: ✅ decided · 🟡 proposed, needs confirmation · 🔴 open, needs conversation

---

## The one thing I need from Jayson after reading this

A yes/no on two questions:
1. **Strategic fit:** Does Brief belong inside Second Team as our top-of-funnel, or should it be structured separately?
2. **Capacity:** If Brief successfully generates 3–5 qualified AI-ops leads per month, can Second Team service them without disruption?

Everything else is tactical and can be worked out once those two questions are settled.
