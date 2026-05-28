# Industry Trends: ADHD Productivity Apps + AI Scheduling

**Phase:** Phase 3 — Wave 1 (A2)
**Project:** startup-validation (Planny)
**Date:** 2026-05-28
**Confidence:** Medium-High (Tier 1 sources confirm the macro trends — CDC on ADHD prevalence, Gartner on AI agents, Rock Health on funding, Apple on Tiimo. Tier 2-3 sources for some market-size figures vary widely and are flagged.)

---

## Technology Trends

### 1. Task-specific AI agents embedded in apps
- **Description:** Movement from "AI assistant that chats" to "AI agent that executes multi-step tasks" (book the flight, reschedule meetings, block focus time). Gartner: <5% of enterprise apps had task-specific agents in 2025; 40% will by end of 2026.
- **Adoption stage:** Early-growing. Real consumer-grade examples shipped in 2025-2026 (Google Gemini Spark, OpenAI Operator-class agents, Apple Intelligence v2).
- **Impact on Planny:** Dual. **Opportunity:** users now expect "delegated" scheduling, not just visualization — Planny can lean into "your ADHD-aware AI plans the week for you." **Threat:** the bar for "AI-powered" is rising fast; basic GPT-wrapped task lists won't differentiate.
- **Timeline to mainstream:** 12-24 months for consumer expectation; already mainstream in early-adopter productivity cohort.
- **Source & tier:** Gartner press release Aug 2025 (Tier 1); Goldman Sachs 2026 outlook (Tier 1).

### 2. On-device LLMs / privacy-first AI
- **Description:** Apple Intelligence runs models on-device for iOS 18/19 and now iOS 27. Privacy-first deployment cited as a top adoption driver. Personal AI assistant market growing 41.9% CAGR with privacy as primary lever.
- **Adoption stage:** Growing fast; Apple shipped on-device LLM as a system framework available to third-party apps.
- **Impact on Planny:** **Opportunity** — ADHD users are sensitive to "where does my mental-health data go?" On-device inference is a strong trust signal. **Threat** — running on Apple's framework means Apple controls the stack.
- **Timeline to mainstream:** Already mainstream on iOS 18+ devices (>60% of US iPhone install base by mid-2026).
- **Source & tier:** Hostinger LLM stats roundup (Tier 3); Apple developer docs referenced (Tier 1).

### 3. Voice-first interaction
- **Description:** Voice-based AI interactions grew 340% in 2025. Prediction: >50% of consumer AI interactions voice-initiated by 2027.
- **Adoption stage:** Growing.
- **Impact on Planny:** **Opportunity** — ADHD users frequently report "I can't sit and type out my schedule." Voice capture / brain-dump is a near-perfect modality fit. Underexplored by competitors.
- **Timeline to mainstream:** 12-18 months.
- **Source & tier:** Sparkco AI / Bananalabs aggregations (Tier 3); cross-confirmed by Goldman Sachs (Tier 1) on voice as 2026 interface theme.

### 4. Calendar APIs maturing + MCP standard
- **Description:** Google Gemini Spark shipped May 2026 with Model Context Protocol (MCP) integrations to Canva, OpenTable, Instacart, Adobe, Spotify, GitHub, Notion, Slack. Apple connects Gemini/Claude/etc through iOS 27 Extensions framework.
- **Adoption stage:** Just-shipped; protocol war underway.
- **Impact on Planny:** **Opportunity** — MCP could let Planny tap into the user's whole stack (Slack, Notion, email) without building dozens of integrations. **Threat** — Google/Apple may own the orchestration layer.
- **Timeline to mainstream:** 6-18 months for indie devs; Google/Apple already there.
- **Source & tier:** TechTimes coverage of Gemini Spark (Tier 2); Gadget Hacks iOS 27 coverage (Tier 3).

### 5. Burnout-aware / context-aware scheduling
- **Description:** Newer AI scheduling tools (Morgen, Sunsama, Motion, Skedpal) evaluate emotional well-being, work patterns, time zones to produce "balanced" schedules — not just packed ones.
- **Adoption stage:** Growing in the "thoughtful productivity" niche; still rare in mainstream.
- **Impact on Planny:** **Opportunity** — directly aligns with ADHD need for energy-aware planning (low-dopamine days, hyperfocus windows). Few competitors execute this well for ADHD specifically.
- **Source & tier:** Morgen blog, Reclaim blog (Tier 3 — vendor); cross-referenced in Schedly trend write-up (Tier 3).

---

## ADHD Awareness & Diagnosis Trend

### Diagnosis rate change 2020 → 2025
- **CDC Data Brief #543 (Dec 2025, Tier 1):** First major CDC update on ADHD prevalence in ~20 years. **6% of US adults have a current ADHD diagnosis** (~15.5 million adults).
- **Adult diagnoses growing 4x faster than child diagnoses:** +123.3% adults vs +26.4% children. (Tier 1, additudemag citing CDC.)
- **Stimulant prescriptions for psychostimulants up 30% from 2018 to 2022** (Tier 1, CDC).
- **55.9% of adults with ADHD were not diagnosed until after age 18** — a huge "late-diagnosis adult" cohort actively seeking solutions.

### TikTok / social-media awareness driver
- Top 100 #ADHD TikTok videos: **~500 million combined views**, avg 5.47M per video (Tier 1, PLOS One 2025, UBC study).
- #ADHD is the **7th most popular health-related hashtag** on TikTok.
- BUT: <50% of claims in top videos align with diagnostic criteria — content quality is poor, which drives self-diagnosis and demand for "tools that help me cope" even where formal diagnosis is absent.
- Strategic read: Planny's TAM includes both diagnosed adults AND a much larger self-identifying cohort. App messaging should not require a diagnosis.

### Demographic skew
- **61% of women** with ADHD diagnosed in adulthood (vs 40% of men) — recent diagnosis surge is heavily female, late-diagnosed, age 25-40.
- Gen Z reports highest burnout (66%) and highest therapy participation (42%, +22pp since 2022) — primed audience.
- North America = 39% of global ADHD app market (largest single region).

### Strategic implication
- **Tailwind is strong and Tier-1-confirmed.** Planny does not need to "create" demand — the demand is exploding. The challenge is differentiation, not awareness.
- The primary persona should skew female, 25-40, late-diagnosed or self-identifying, US-based, already paying for therapy/meditation apps.

---

## Investment Activity

### Total funding & direction
- Digital health funding 2025: **$14.2B, +35% vs $10.5B in 2024** (Rock Health, Tier 1). Mental health was a "concentrated" category receiving outsized capital.
- AI-central startups: **$34.4M avg per round** vs $18.8M for non-AI (Rock Health, Tier 1) — clear AI premium.
- Trend direction: **Accelerating** at the megadeal end; flat-to-modest at seed.

### Notable rounds (ADHD-adjacent + AI scheduling)
| Company | Stage | Amount | Date | Notes |
|---|---|---|---|---|
| Motion (usemotion) | Series B/C/C2 | $60M total; $38M Series C led by Scale | 2024-2025 | Valuation $550M. AI calendar/task mgmt. Tier 2 (Built In SF, Finsmes). |
| Reclaim.ai | Acquired | $40.2M | Jul 26, 2024 | **CONFIRMED** acquired by Dropbox. 320k users, 43k companies. Tier 1 (TechCrunch, SEC-filed price via MarketScreener). |
| Inflow | Series A | $11M | 2023 | ADHD CBT app. Led by Octopus Ventures. Tier 2 (TechCrunch). ~$22.49/mo subscription. |
| Numo | n/a public | — | — | ADHD app. $15.99/mo. Attracting VC attention per The Census. Tier 3. |
| Rule | Pre-seed | £800k | 2025 | ADHD-tax fintech. London Venture Partners. Tier 2 (Yahoo Finance). |
| Neurode | Pre-seed | $5.2M | 2024 | ADHD medtech headband. Khosla Ventures + PsyMed. Tier 2 (Startup Daily). |
| Talkiatry | Series D | $210M | 2025 | Telepsychiatry megadeal. Tier 1 (Rock Health). |
| Grow Therapy | Late stage | $150M | 2025 | Hybrid mental health. Tier 1 (Rock Health). |

### Notable acquisitions
- **Reclaim.ai → Dropbox, $40.2M, July 2024 (CONFIRMED, Tier 1).** This is the single most important data point for Planny: a major incumbent (Dropbox) paid 8 figures for a scheduling-AI startup with 320k users. It both validates the category and shows what an exit can look like. It also signals consolidation pressure — productivity incumbents are buying AI scheduling rather than building.
- Inflow acquired Lina Health (telehealth) in Nov 2022 — direction-of-travel: ADHD apps adding clinical service layers.

### What this signals for a solo bootstrap entrant
- **Positive:** Acquirers exist and pay real money for relatively small user bases (320k → $40M = ~$125/user enterprise value). Category is validated.
- **Negative:** Well-funded competitors (Motion $60M, Tiimo with 50k paying subs and Apple's endorsement, Inflow with $11M war chest) are setting the bar on product quality and marketing spend.
- **Verdict for bootstrap:** Viable only with a tight wedge (ADHD-specific, weekly cadence, mobile-first) and a clear "why now I can't just use Motion or Tiimo" narrative. Do not compete on horizontal AI features.

---

## Behavioral Shifts

### Calendar fragmentation & tool sprawl
- 48% of workers say work feels "chaotic and fragmented"; 80% report lacking time/energy. Avg remote worker uses 4.8 collaboration tools. 40% waste meaningful time context-switching. (Tier 2-3 aggregations.)
- **Implication for Planny:** A weekly-rhythm planner that consolidates "what matters this week" across fragmented tools maps directly onto the pain. ADHD amplifies this 2-3x.

### Burnout / mental-load shift
- 66% of US workers report burnout (Modern Health 2025). Gen Z = 66% (highest cohort). Fully remote = 61%, hybrid = 57%.
- Hybrid workers setting their OWN schedules report **76% higher** burnout than those with structured schedules.
- **Implication for Planny:** Counter-intuitive — "flexibility" is itself an ADHD trap. A structured weekly schedule produced FOR the user (not just by them) is a documented preference. Strong positioning hook.

### Spending power — Gen Z + Millennials
- **Millennials = 45% of all in-app spending.** (Tier 3, marketingltb / sqmagazine.)
- 42% of Gen Z currently in therapy (+22pp vs 2022) — they pay for mental health.
- Health & wellness = 23% of total subscription consumer spend (Tier 2-3, RevenueCat State of Subs 2025).
- Subscription app ARPU benchmark: **$8.41/mo** (range $3-9/mo for sub apps).
- Mental health app retention is poor: **30% abandon within 90 days** (2024 study).
- **Implication for Planny:** Pricing power exists ($8-15/mo is realistic). Retention is the moat — not acquisition. Build for day-30, day-90, day-180.

### Therapeutic reimbursement
- CMS introduced new payment codes for digital therapies in 2025 — opens the door (long-term) for ADHD apps to be partially reimbursed if they pursue regulated digital-therapeutic positioning.
- Planny implication: optional 2-year path — keep clean clinical-evidence breadcrumbs.

---

## Expert Predictions

| Prediction | Source | Tier | Credibility |
|---|---|---|---|
| 40% of enterprise apps will have task-specific AI agents by end of 2026 (from <5% in 2025) | Gartner | 1 | High |
| Agentic AI could drive 30% of enterprise app revenue / >$450B by 2035 | Gartner | 1 | Medium (long horizon, best-case) |
| >40% of agentic AI projects will be cancelled by end of 2027 (cost, unclear value) | Gartner | 1 | High — important counter-signal |
| Personal AI agents become "default interface for digital experiences" by 2026 | Multiple syntheses citing Goldman Sachs / Salesforce | 1-2 | Medium-High |
| >50% of consumer AI interactions voice-initiated by 2027 | Salesforce trend report / aggregations | 2-3 | Medium |
| ADHD apps market: $2.78B (2026) → $3.22B (2027) → $4.3B (2030); CAGR ~12-15% | Multiple market-research firms (figures DIVERGE widely) | 3 | Low-Medium — flagged below |
| AI agents handle 40% of knowledge work by end of 2027 | Bananalabs / firecrawl syntheses | 3 | Low-Medium |

---

## Timing Assessment

### Is now a good time to enter? **YES, with caveats.**

**Reasons now is right:**
1. **CDC just legitimized adult ADHD** with its first major prevalence update in 20 years (Dec 2025) — peak cultural awareness.
2. **Apple chose an ADHD/neurodivergent planner (Tiimo) as iPhone App of the Year 2025** — strongest possible category endorsement; will pull marketing oxygen toward the niche.
3. **AI infrastructure maturity:** on-device Apple LLM + MCP + voice means a small team can build what required $10M two years ago.
4. **Acquirer evidence:** Dropbox/Reclaim deal proves category exits exist at modest user counts.
5. **Funding tailwind:** Rock Health 2025 confirms mental-health + AI is one of two concentrated themes.
6. **Behavioral pain is documented:** fragmented schedules, burnout, hybrid-flexibility paradox all point to "give me a structured weekly plan."

**Reasons to worry / what would make timing worse:**
1. **Apple/Google native scheduling threat (REAL).** Gemini Spark (May 2026) and the rumored iOS 27 Gemini-powered Siri are explicitly going after "personal life management." Apple's on-device calendar + Siri intent could deliver a "good enough" generic scheduler that takes the bottom out of the price floor.
2. **Gartner's 40% cancellation rate** signals an agentic-AI hype-cycle correction is coming 2026-2027 — investor and user fatigue risk.
3. **Tiimo just won App of the Year with 50k paying subs / 500k users** — they will get a massive halo and likely a strategic acquirer. Window is narrow before they dominate ADHD-planner mindshare.
4. **Mental-health app retention is brutal** (30% churn at 90 days) — Planny must out-engineer retention from day one or unit economics fail.

### Risk that AI assistants become commoditized by Apple/Google
- **HIGH for horizontal scheduling.** Spark + Gemini-Siri will eat undifferentiated AI calendars within 18 months.
- **LOW-MEDIUM for vertical / ADHD-specific.** Apple/Google have neither the empathy positioning nor the willingness to ship neurodivergent-specific UX. Tiimo's award is direct evidence Apple recognizes the niche but won't enter it themselves.
- **Defense:** Plant the flag on (a) ADHD-specific UX & language, (b) weekly cadence (Apple/Google default is daily or per-event), (c) emotional/energy-aware planning, (d) community / shared-experience trust signals.

---

## Strategic Implications for Planny

1. **Position as "ADHD-native weekly planner," not "AI scheduler."** The horizontal AI scheduler category will be eaten by Gemini Spark and Apple. The vertical is the defensible wedge — Tiimo just proved you can win Apple App of the Year by going narrow.

2. **Lead with voice / brain-dump capture, on-device privacy, energy-aware planning.** These three feature pillars all align with documented technology trends AND ADHD-specific pain. They also stay out of the direct collision lane with Calendar+Gemini.

3. **Price $8-15/mo and build for day-180 retention.** ARPU benchmarks support it. Mental-health churn is the real KPI; design onboarding, weekly review rituals, and "compassionate re-engagement" around the documented 30/90/180 cliffs.

4. **Target US, late-diagnosed women 25-40 as the beachhead persona.** CDC + UBC + Rock Health data all converge: this cohort is the most underserved, most willing to pay, and most active on TikTok where Planny's awareness loop will live cheapest.

5. **Window is ~12-18 months.** Tiimo will get bigger. Gemini Spark will improve. Apple iOS 27 will ship a smarter Siri. Get to public launch + paid users in 2026; do not let this slip to late-2027 where the category will look very different.

6. **(Bonus) Leave a clinical-evidence breadcrumb trail.** CMS digital-therapy payment codes (2025) are a 2-year optional unlock. Track outcomes from day one so it's available later without re-platforming.

---

## Source Quality Assessment

**Tier 1 (used):** CDC Data Brief #543 (Dec 2025); Gartner press releases Aug 2025 & Oct 2025; PLOS One peer-reviewed TikTok study (2025); Rock Health 2025 Year-End report; TechCrunch (Reclaim acquisition); MarketScreener (deal value); UBC News; Goldman Sachs 2026 outlook; Apple App Store Awards 2025 (announcement).

**Tier 2 (used):** SiliconANGLE, Built In SF, Finsmes, BetaKit, Yahoo Finance, Daring Fireball, Modern Healthcare, FierceHealthcare, MedCity News.

**Tier 3 (used with skepticism):** Market-research firm aggregations (Strategic Market Research, Market Growth Reports, Coherent Market Insights, Business Research Insights, datainsightsmarket), sqmagazine, harmonyhit, bananalabs, sparkco, firecrawl, aimagicx.

**Reliability skew:** Tier-1 sources strongly support the macro story (ADHD diagnosis surge, AI-agent emergence, AI-driven funding concentration, Reclaim/Dropbox deal, Tiimo award). Tier-3 sources diverge widely on ADHD-app market size — see Yellow Flags.

---

## Data Gaps

1. **No reliable revenue figures for Tiimo, Numo, Inflow.** Tiimo's "50k paying subs" is the most concrete figure found; multiply by ~$5-10/mo → ~$3-6M ARR estimate, not confirmed.
2. **No clear data on Israel ADHD app market** — secondary geo for Planny but no signals were available.
3. **No CAC benchmarks for ADHD-specific apps.** Mental-health apps generally show $30-80 CAC; ADHD-specific likely cheaper due to TikTok organic, but unconfirmed.
4. **No 2025-2026 funding rounds for explicitly ADHD-labeled apps** found beyond small pre-seeds (Rule, Neurode). Either deals are happening quietly or the ADHD-app VC moment hasn't peaked yet.
5. **No data on what happened post-acquisition to Reclaim's pricing / churn** — would inform whether Dropbox absorption is a positive or negative competitive signal.
6. **Apple iOS 27 + Gemini-Siri integration is rumor-stage** as of May 2026 — WWDC 2026 (June) will clarify scope of native threat. Re-check in 30 days.

---

## Flags

**Red Flags:**
- **Apple/Google native AI scheduling is a real and imminent commoditization threat for horizontal AI calendars.** Gemini Spark already ships. WWDC 2026 in 2 weeks may amplify. Planny's positioning MUST be vertical/ADHD-specific from day one.
- **Mental-health app retention crisis (30% churn at 90 days).** This is the dominant failure mode in the category. If Planny doesn't out-design retention, all the tailwinds in the world won't save unit economics.
- **Tiimo just won Apple iPhone App of the Year (Dec 2025)** in essentially the exact category Planny is targeting. They have a massive head start, a marketing halo, and 500k users. Any positioning that doesn't sharply differentiate from Tiimo is dead on arrival.
- **Gartner's 40% agentic-AI cancellation forecast for 2027** is a real warning that the AI hype is heading into a trough — investor and consumer fatigue could hit just as Planny is scaling.

**Yellow Flags:**
- ADHD app market-size figures vary wildly across Tier-3 sources: $1.91B → $2.78B → $4.06B → $7.7B by various years and dates. Treat any specific TAM number with low confidence; the directional growth (12-15% CAGR) is more reliable than absolute size.
- Some Tier-3 sources use copy-paste phrasing across reports — suggests a small number of underlying analyses being rebadged.
- The "8 million Inflow users" figure conflicts with "100k Google Play downloads" — likely the 8M includes everyone who's ever touched a free tier or web property; treat as inflated.
- TikTok-driven ADHD awareness includes significant misinformation (<50% accurate). Risk: marketing channel could be regulated or de-amplified by platforms within 2-3 years.
- "Trillion-dollar AI agent market" predictions (Goldman, Gartner best-case) carry a hype-cycle premium; useful for direction, not for planning.

---

## Sources

- [CDC Data Brief #543 (Dec 2025) — Adult ADHD prevalence](https://www.cdc.gov/nchs/products/databriefs/db543.htm)
- [Adult ADHD Diagnosis Growing More Common — ADDitude / CDC](https://www.additudemag.com/adult-adhd-diagnosis-cdc-report/)
- [CDC — Data and Statistics on ADHD](https://www.cdc.gov/adhd/data/index.html)
- [PLOS One — A double-edged hashtag: #ADHD on TikTok (2025)](https://journals.plos.org/plosone/article?id=10.1371%2Fjournal.pone.0319335)
- [UBC News — ADHD misinformation on TikTok](https://news.ubc.ca/2025/03/adhd-misinformation-on-tiktok/)
- [Gartner — 40% of enterprise apps will feature task-specific AI agents by 2026](https://www.gartner.com/en/newsroom/press-releases/2025-08-26-gartner-predicts-40-percent-of-enterprise-apps-will-feature-task-specific-ai-agents-by-2026-up-from-less-than-5-percent-in-2025)
- [Gartner — Over 40% of agentic AI projects will be cancelled by 2027](https://www.gartner.com/en/newsroom/press-releases/2025-06-25-gartner-predicts-over-40-percent-of-agentic-ai-projects-will-be-canceled-by-end-of-2027)
- [Gartner — Strategic Predictions for 2026](https://www.gartner.com/en/articles/strategic-predictions-for-2026)
- [Goldman Sachs — What to expect from AI in 2026](https://www.goldmansachs.com/insights/articles/what-to-expect-from-ai-in-2026-personal-agents-mega-alliances)
- [Rock Health — 2025 year-end digital health funding](https://rockhealth.com/insights/2025-year-end-digital-health-funding-overview-a-tale-of-two-markets/)
- [Modern Healthcare — AI drives digital health funding in 2025: Rock Health](https://www.modernhealthcare.com/health-tech/mh-ai-digital-health-2025-rock-health/)
- [TechCrunch — Dropbox acquires Reclaim.ai (Aug 2024)](https://techcrunch.com/2024/08/22/dropbox-acquires-index-ventures-backed-ai-scheduling-tool-reclaim-ai/)
- [MarketScreener — Dropbox acquired Reclaim.ai for $40.2M](https://www.marketscreener.com/quote/stock/DROPBOX-INC-45013534/news/Dropbox-Inc-acquired-Reclaim-ai-Inc-for-40-2-million-47716890/)
- [Reclaim — Reclaim is now part of Dropbox](https://reclaim.ai/blog/dropbox-acquires-reclaim)
- [Motion — Series A $13M announcement](https://www.usemotion.com/blog/we-raised-13-million-in-series-a-to-automate-team-project-management)
- [Built In SF — Motion secures $60M](https://www.builtinsf.com/articles/motion-raises-60m-funding-20250909)
- [TechCrunch — Inflow raises $11M Series A (Jan 2023)](https://techcrunch.com/2023/01/11/inflow-a-platform-for-managing-adhd-through-cbt-raises-11m/)
- [Yahoo Finance — Rule raises £800k for ADHD-tax fintech](https://finance.yahoo.com/news/rule-raises-800-000-tackle-163700188.html)
- [Startup Daily — Neurode $5.2M pre-seed for ADHD medtech](https://www.startupdaily.net/topic/funding/adhd-medtech-bags-5-2-million-pre-seed-round-for-its-alternative-headband-treatment/)
- [Daring Fireball — 2025 App Store Award Winners (Tiimo)](https://daringfireball.net/2025/12/2025_app_store_award_winners)
- [Tiimo — Winner of iPhone App of the Year 2025](https://www.tiimoapp.com/resource-hub/tiimo-winner-2025-app-store-awards)
- [TechTimes — Gemini Spark launch (May 2026)](https://www.techtimes.com/articles/317144/20260525/gemini-spark-googles-24-7-cloud-ai-agent-now-executes-tasks-third-party-apps.htm)
- [Gadget Hacks — iOS 27 third-party AI models](https://apple.gadgethacks.com/news/ios-27-third-party-ai-models-explained-gemini-claude-and-more/)
- [Dark Reading — Gemini Calendar invites attack vector](https://www.darkreading.com/cloud-security/google-gemini-flaw-calendar-invites-attack-vector)
- [The Census — ADHD apps find their flow](https://www.thecensus.io/p/adhd-apps-find-their-flow)
- [Choosing Therapy — Inflow ADHD App Review 2025](https://www.choosingtherapy.com/inflow-adhd-app-review/)
- [Fortune Business Insights — Productivity Apps Market](https://www.fortunebusinessinsights.com/productivity-apps-market-110254)
- [Strategic Market Research — ADHD Apps Market Report](https://www.strategicmarketresearch.com/market-report/adhd-apps-market)
- [Market Growth Reports — ADHD Apps Market](https://www.marketgrowthreports.com/market-reports/adhd-apps-market-115215)
- [McKinsey — Future of wellness trends](https://www.mckinsey.com/industries/consumer-packaged-goods/our-insights/future-of-wellness-trends)
- [Harmony HIT — State of Gen Z Mental Health 2025](https://www.harmonyhit.com/state-of-gen-z-mental-health/)
- [RevenueCat — State of Subscription Apps 2025](https://www.revenuecat.com/state-of-subscription-apps-2025/)
- [Apollo Technical — Remote Work Burnout Statistics](https://www.apollotechnical.com/remote-work-burnout-statistics/)
- [Gable — Hybrid Work Statistics 2026](https://www.gable.to/blog/post/hybrid-work-statistics)
