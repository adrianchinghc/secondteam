# CEOS Video Content Plan (v2)
_Built by Atlas | 2026-04-13_
_Personal brand content: Adrian Ching_

---

## Strategy Summary

**Target audience:** Entrepreneurs and leadership teams running EOS who are AI-curious. They know what a V/TO is, they run L10s, they set Rocks. They don't know a free AI tool exists that runs the entire system.

**Why this works:**
- Hits Pillar 1 (AI for Business Owners) + Pillar 3 (Systems and Leverage)
- Brad Feld (Foundry Group, Techstars) gives instant credibility to the tool
- EOS has 250K+ companies globally. Well-defined, searchable audience
- You actually run EOS at Second Team. Not a reviewer. An operator.
- SEA angle: EOS content in this region is underserved. You become the reference
- Direct overlap with Second Team's ICP (EOS-managed SMBs)

**Top-of-funnel play.** No monetization right now. Audience building that feeds into Second Team's pipeline.

---

## 1. YouTube Video

### Title (pick one, A/B test against thumbnail)

- **"This Free AI Tool Runs EOS For You (Full Setup + Demo)"** (recommended, best SEO)
- "I Replaced My EOS Tools With AI. Here's What Happened."
- "Brad Feld Just Open-Sourced an AI EOS System. I Tried It."

### Target length: 14-18 minutes

### SEO keywords
"EOS tools", "EOS software", "run EOS with AI", "CEOS Claude Code", "free EOS tool", "Brad Feld CEOS", "Entrepreneurial Operating System AI", "EOS for startups", "Ninety.io alternative"

---

### Video Outline

The structure below follows retention best practices: open with a payoff shot, explain what it means for the viewer immediately, then walk through each feature with a show-then-explain rhythm. Every section answers "what does this mean for you as an entrepreneur?"

---

#### COLD OPEN / HOOK (0:00 - 0:30)

**No intro. No "hey guys." Start with the payoff.**

[Screen recording: CEOS generating a complete V/TO from a conversation in Claude Code. The markdown file appears, fully structured with core values, core focus, 10-year target, marketing strategy, 3-year picture, 1-year plan.]

**Voiceover (while showing the screen):**
"This is a complete Vision/Traction Organizer. Built in under 10 minutes. By AI. For free."

[Cut to face cam]
"Brad Feld, the guy behind Techstars and Foundry Group, just open-sourced a tool called CEOS. It runs the entire Entrepreneurial Operating System from your terminal. 19 tools. V/TO, Rocks, Scorecards, L10 meetings, People Analyzer, all of it. I run EOS at my own company, so I tested every single one. Let me show you what works, what doesn't, and whether this can actually replace your current EOS setup."

**Why this works for retention:** The viewer sees the end result in the first 5 seconds. They know this video delivers something real. The "I run EOS" line establishes credibility. The "what works, what doesn't" creates a curiosity loop that holds them past the first 30 seconds.

---

#### WHAT IS CEOS AND WHY SHOULD YOU CARE (0:30 - 2:30)

**Framing: talk to the business owner, not the developer.**

[Screen: show the CEOS GitHub repo page briefly]

**Script direction:**
"If you run EOS, you're probably using one of three things. Ninety.io, Traction Tools, or, let's be real, a Google Doc and a spreadsheet."

"CEOS is different. It's open source. Free. Built by Brad Feld. And it turns Claude Code, which is an AI coding tool from Anthropic, into a full EOS operating system."

[Screen: show the /skills directory with all 19 skill folders]

"19 skills. Each one maps to a core EOS tool. Your V/TO, your accountability chart, your rocks, your scorecard, your L10 meeting, your IDS sessions. All stored as simple text files in Git, which means every single change is tracked, versioned, and searchable."

**What this means for you:**
"For business owners, this is important for three reasons. One, it's free. No subscription. Two, you own your data. It's files on your computer, not locked inside someone else's software. Three, because it's AI-powered, it actually helps you think through each tool instead of just giving you a blank template."

[Screen: briefly show a markdown file with YAML frontmatter to demystify what "text files" looks like]

---

#### SETUP (2:30 - 4:00)

**Keep this tight. Business owners don't want to watch a 5-minute install.**

[Screen recording: terminal]

**Script direction:**
"Setup takes about 2 minutes. Three commands."

[Show each command as you type it]
1. "Clone the repository." `git clone https://github.com/bradfeld/ceos.git`
2. "Move into the folder." `cd ceos`
3. "Run the setup script." `./setup.sh init`

[Show the setup completing, skills being installed]

"That's it. You now have 19 EOS tools inside Claude Code. Let me show you the five that matter most."

**Why "five that matter most":** This creates a roadmap in the viewer's head. They know there's a structure coming. It also signals you're curating for them, not just clicking through every feature. This keeps retention because they're mentally tracking progress: "okay, that's 1 of 5."

---

#### DEMO 1 of 5: V/TO (Vision/Traction Organizer) (4:00 - 7:30)

**This is the centerpiece demo. Every EOS company has a V/TO.**

[Screen: run the ceos-vto skill in Claude Code]

**Show, then explain. Don't explain before showing.**

[Let the AI ask you the first question about core values. Answer it naturally. Show 2-3 exchanges of the conversation.]

**Then cut to face cam and explain:**
"What it's doing is walking you through the exact same exercise an EOS implementer would run in a Vision Building Day. Core values, core focus, 10-year target, marketing strategy, 3-year picture, 1-year plan, and your issues list."

[Screen: show the completed V/TO markdown file]

"Here's what it generated. This is a complete V/TO. Let me compare it to the one I built manually for my company."

[Screen: side-by-side if possible, or talk through what it got right and where you'd edit]

**What this means for you:**
"If you've ever struggled to fill in your V/TO, or your team spends 3 hours arguing about core values and walks away with nothing written down, this gets you 80% there in 10 minutes. You still need to edit it. The AI doesn't know your business like you do. But having a structured draft to react to is way faster than starting from a blank page."

**The money shot:**
[Screen: run `git diff` to show the tracked changes to the V/TO file]

"And here's the part I didn't expect. Every change to your vision is tracked in Git. You can see exactly what changed, when, and why. For an accountability-driven system like EOS, that's actually powerful."

---

#### DEMO 2 of 5: ROCKS (Quarterly Priorities) (7:30 - 9:30)

[Screen: run ceos-rocks]

**Show the AI asking you to define your rocks. Set 3 rocks live.**

"Rocks are your 90-day priorities. Most teams set them and forget them. Let me show you how CEOS handles this."

[Show the AI structuring each rock with: owner, due date, measurable outcome, connection to the 1-year plan]

**What this means for you:**
"Notice what it does. It forces you to define what 'done' looks like. A lot of teams set rocks like 'improve marketing' or 'hire a sales person.' That's not a rock, that's a wish. This tool pushes you to be specific, and it connects each rock back to your 1-year plan from the V/TO."

[Screen: show the generated rock files]

"Each rock is its own file. Tracked individually. You can review progress on each one without opening a spreadsheet."

---

#### DEMO 3 of 5: L10 MEETING (9:30 - 12:00)

[Screen: run ceos-l10]

**This is the most relatable demo. Every EOS team runs L10s weekly.**

"The L10 is the heartbeat of EOS. Same day, same time, same agenda, every week. Let me show you what CEOS does with it."

[Show the meeting structure being generated: segue, scorecard review, rock review, customer/employee headlines, to-do review, IDS, conclude]

"It follows the standard L10 agenda. Segue, scorecard, rocks, headlines, to-dos, IDS, conclude. Nothing new there. But watch what happens when we get to IDS."

[Demo the IDS flow: Identify an issue, Discuss it with the AI, arrive at a Solution with clear to-do items]

**What this means for you:**
"Two things here that are actually useful. First, your L10 notes are now searchable. You can go back 6 months and find every time you discussed a specific issue. No more 'I think we talked about this.' Second, the to-dos that come out of IDS automatically feed into the to-do tracking system. Nothing falls through the cracks."

[Show the generated meeting notes file]

"Compare that to a whiteboard photo saved to someone's camera roll. This is permanent, structured, and everyone on your team can access it."

---

#### DEMO 4 of 5: PEOPLE ANALYZER (12:00 - 13:30)

[Screen: run ceos-people]

**Sensitive topic. Handle it with maturity.**

"The People Analyzer is one of the harder EOS tools to use well. You're evaluating your team against your core values and against GWC: do they Get it, Want it, and have the Capacity to do it."

[Show the AI walking through a people analysis. Use a fictional example, not a real team member.]

**What this means for you:**
"I wouldn't use this to make a firing decision. That requires human judgment. But I would use it to prepare for a quarterly conversation. It structures your thinking and forces you to be honest about each person against specific criteria. It's a thinking tool, not a decision-maker."

---

#### DEMO 5 of 5: SCORECARD (13:30 - 15:00)

[Screen: run ceos-scorecard]

"Your scorecard tracks the 5 to 15 most important numbers in your business, weekly. Revenue, leads, customer satisfaction, whatever your key metrics are."

[Show setting up metrics and a weekly data entry]

**What this means for you:**
"Most teams I know track their scorecard in a Google Sheet. It works, but it's disconnected from everything else. In CEOS, your scorecard metrics live alongside your rocks, your meeting notes, and your V/TO. Everything's in one system. And because it's in Git, you can see trends over time just by looking at the file history."

---

#### QUICK HITS: THE OTHER 14 TOOLS (15:00 - 15:45)

**Rapid montage. Don't dwell. Show breadth.**

[Screen: quick 5-second flashes of each remaining tool running]

"Beyond those five, CEOS also includes: an accountability chart builder, quarterly planning for your annual offsite, a 20-question organizational checkup, a Delegate and Elevate exercise, clarity break tracking, an EOS kickoff workflow that runs your Focus Day and Vision Building Days, quarterly conversations between managers and direct reports, annual planning, to-do tracking, process documentation, issue tracking, trend analysis, a calendar integration, and a dashboard."

"I won't walk through all of these. The five I showed you are the core. But know that the full system is here if you want it."

---

#### HONEST REVIEW: WHAT'S GOOD, WHAT'S NOT (15:45 - 17:00)

**This is where trust is built. Don't be a salesman for someone else's tool.**

[Face cam, direct to camera]

**What's good:**
"Three things impressed me. First, the V/TO generation is legitimately useful. It gets you to a structured draft faster than any session I've run manually. Second, the Git tracking. Every change to your vision, your rocks, your people decisions, it's all versioned. That's something no other EOS tool does. Third, it's free and you own your data. No subscription, no lock-in."

**What's not:**
"Three things to be aware of. First, you need Claude Code, which is a paid Anthropic subscription. So it's not completely free. Second, it runs in the terminal. If your leadership team isn't technical, you'll need to be the one running it. This is not Ninety.io where everyone logs in with a browser. Third, it's new. Version 1.0, released February 2026. There will be rough edges."

**Your take as an operator:**
"Here's my honest take. I'd use this alongside my existing EOS process, not instead of it. The AI is great for drafting, structuring, and tracking. But EOS works because of the hard human conversations. The implementer who calls you out. The accountability in the room. No AI replaces that. Use CEOS as your system of record and your thinking partner. Keep the humans for the hard stuff."

---

#### CTA + CLOSE (17:00 - 17:30)

**Short. No begging.**

"Link to CEOS is in the description. If you're running EOS and you want to see more content on how AI fits into your operations, subscribe. I run EOS at my company, I build software with AI, and I show the work. See you in the next one."

[End screen: subscribe button, link to next video]

---

## 2. Short-Form Script (TikTok / Reels / Shorts)

**Format:** 45-50 seconds. Screen recording + face cam overlay.

---

**HOOK (0-3 sec):**
[Screen: V/TO being generated in real-time]
"This AI just built my entire EOS Vision/Traction Organizer in 10 minutes."

**WHAT IT IS (3-15 sec):**
[Face cam]
"Brad Feld, the VC behind Techstars, just open-sourced a tool called CEOS. 19 AI-powered tools that run the full Entrepreneurial Operating System. V/TO, Rocks, Scorecards, L10 meetings, People Analyzer. All free. All stored as files you own."

**THE PROOF (15-35 sec):**
[Screen: rapid cuts showing 3-4 tools running]
"Watch. It walks you through your core values, sets your quarterly rocks with measurable outcomes, runs your L10 meeting with IDS, and tracks every change in Git so nothing gets lost."

[Face cam]
"I run EOS at my own company. The V/TO generation alone is worth trying this. It gets you 80% there in 10 minutes."

**CTA (35-45 sec):**
"Full walkthrough on my channel. Link in bio."

**On-screen text throughout:** "Free AI tool that runs EOS"

**Hashtags:** #EOS #AI #entrepreneur #business #startup #entrepreneurialoperatingsystem #bradfeld #claudecode

---

## 3. LinkedIn Post Draft

---

Brad Feld just open-sourced a tool that runs the entire Entrepreneurial Operating System using AI.

It's called CEOS. 19 skills built for Claude Code. V/TO, Rocks, Scorecards, L10 meetings, People Analyzer, IDS, the whole framework.

All your EOS data stored as markdown files in Git. No database. No SaaS subscription. No vendor lock-in. Git history becomes your audit trail.

I run EOS at my company. So I installed it and tested it against our real V/TO and our real Rocks.

Three things stood out:

The V/TO generation is good. Not "replace your implementer" good, but "get 80% of the way there in 10 minutes" good. It asks the right questions about core values, core focus, 10-year target, and marketing strategy. Then it generates a structured document you can actually use.

The L10 meeting structure is solid. Segue, scorecard review, rock review, IDS, to-dos. It generates meeting notes that are searchable and version-controlled. No more lost whiteboard photos.

The real unlock is the audit trail. Every change to your vision, your rocks, your people decisions is tracked in Git. For accountability-driven teams, that's powerful.

Where it falls short: it requires Claude Code (paid subscription). It's terminal-based, so your leadership team needs to be comfortable with that or you run it for them. And it won't replace the hard human conversations an implementer facilitates.

But as a system of record for EOS? This is better than what most teams are using today.

Full walkthrough and honest review on my YouTube (link in comments).

---

## 4. Thumbnail Concepts

**Concept A: "The Bold Claim" (recommended, A/B test this one first)**
- Adrian's face, direct to camera, slightly surprised expression
- Text overlay: "REPLACE YOUR EOS CONSULTANT?"
- Subtext: "Free Open Source Tool"
- Background: Blurred terminal with CEOS output visible
- Colors: Bold yellow text on dark background

**Concept B: "The Reveal"**
- Left side: CEOS GitHub repo or terminal screenshot
- Right side: Adrian's face, interested expression
- Text overlay: "FREE AI EOS TOOL"
- Subtext: "I Tested It"
- Colors: Dark background, green accent (terminal feel)

**Concept C: "The Comparison"**
- Split screen: Left = messy whiteboard with EOS stuff / Right = clean terminal with CEOS output
- Text overlay: "EOS + AI = ?"
- Adrian's face in corner, pointing at the terminal side
- Colors: Red (old way) vs Green (new way)

**Recommendation:** Test C against A. C has the visual contrast that performs well in thumbnails. A has the curiosity gap.

---

## 5. Content Calendar

| Date | Platform | Content | Notes |
|------|----------|---------|-------|
| This week | - | Install CEOS, test all 19 skills, take notes | Prep work |
| Week of Apr 21 | YouTube | Full CEOS walkthrough video | Record after testing |
| Same day | LinkedIn | Long-form post (above) | Publish same day as YT |
| Same day | X/Twitter | Thread version of LinkedIn post | Repurpose key points |
| Day after | TikTok | Short-form (above) | Cut from video footage |
| Day after | Instagram Reels | Same short, adjusted aspect ratio | Cross-post |
| Day after | YouTube Shorts | Same short | Cross-post |

---

## 6. Pre-Recording Checklist

Before you sit down to record:

1. Install CEOS and run through all 19 skills
2. Build a real V/TO for Second Team using the tool (this becomes demo footage)
3. Set 3 real rocks and note how the AI structures them
4. Run a simulated L10 meeting
5. Note which skills impress, which are mid, which break
6. Screenshot the Git diff of your V/TO changes (key visual moment)
7. Prepare your "honest take" bullet points so the review section feels natural
8. Test your screen recording setup. Make sure the terminal text is readable at YouTube resolution
9. Have a fictional employee name ready for the People Analyzer demo (don't use real team)

---

## 7. Monetization Notes (For Later)

Not building now. Logging options for when demand is proven:

1. **"CEOS for Non-Technical Founders" guide** (paid PDF): Setup walkthrough + best practices for teams uncomfortable with terminal. RM 49-99.
2. **CEOS Setup as a Micro-Service**: "I'll set up CEOS for your leadership team in 2 hours." RM 500-1,000 one-time.
3. **YouTube membership**: Exclusive content on running EOS with AI tools.
4. **Affiliate/referral**: If Anthropic launches a Claude Code referral program, this becomes passive income.

Strongest near-term play is #2. It's a service, not a product. Fits your DNA.

---

## Strategic Filter Check

- Does this move toward RM 50M by 2035? Yes. Builds audience overlapping with Second Team ICP.
- Does this serve the ICP? Yes. EOS-managed growing companies.
- Does this contribute to becoming AI-native? Yes. Showcases AI-native operations publicly.
- Does this help close a deal in 30-60 days? Indirectly. Attracts the right people.
- Is upside unlimited and downside survivable? Yes. One day of recording. Upside is viral potential in a defined niche.
