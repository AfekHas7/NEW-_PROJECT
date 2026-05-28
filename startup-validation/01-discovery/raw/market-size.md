# Market Sizing: ADHD Productivity / Scheduling Apps (US + Israel)

**Phase:** Phase 3 — Wave 1 (A1)
**Project:** startup-validation (Planny)
**Date:** 2026-05-28
**Confidence:** Medium — TAM/SAM figures are well-sourced from Tier 1/2; ADHD-specific unit economics rely on proxies because no public data exists for ADHD-only app cohorts. Conservative estimates used throughout.

---

## TAM (Total Addressable Market)

Three relevant TAM lenses, with multiple sources to triangulate:

### Lens 1 — Global Productivity Apps Market
| Source | 2025 Size | Growth | Tier |
|---|---|---|---|
| Mordor Intelligence | ~$11.96B | CAGR 8.63% to $18.09B by 2030 | Tier 1 |
| Fortune Business Insights | ~$13.15B (2025) → $14.46B (2026) → $30.85B by 2034 | CAGR 9.94% | Tier 1 |
| The Business Research Company | ~$12.32B | ~CAGR 9% | Tier 1 |
| Statista Market Forecast | Confirms ~$12-14B range | n/a | Tier 1 |

**Triangulated TAM (Global Productivity Apps 2025): ~$12-14B**, growing 8-10% CAGR. North America = 38.1% share (~$4.6-5.3B US slice).

### Lens 2 — Global ADHD Apps Market
| Source | 2025 Size | Growth | Tier |
|---|---|---|---|
| The Business Research Company | $2.22B (2025), $4.06B by 2029 | CAGR 16.2% | Tier 1 |
| Market Growth Reports | $1.79B (2025) | n/a | Tier 2 |
| Research and Markets | ~$2.0B (2026) | n/a | Tier 1 |
| Data Insights Market (ADHD planner subset) | $500M (2025) → $1.8B by 2033 | CAGR 15% | Tier 2 |

**Triangulated TAM (Global ADHD Apps 2025): ~$1.8-2.2B**, growing 15-16% CAGR (nearly 2x productivity-overall pace). **US slice estimated at ~$773M** (per Market Growth Reports breakout) — the single most directly relevant TAM number for Planny.

### Lens 3 — Scheduling Apps (sub-segment)
| Source | 2025 Size | Growth | Tier |
|---|---|---|---|
| Grand View Research | Global $663M (2025) → $1.81B by 2033 | CAGR 13.46% | Tier 1 |
| Grand View Research (US) | $250.4M (2025) → $637.2M by 2033 | n/a | Tier 1 |

**Note:** Grand View's "scheduling apps" segment skews to workforce/appointment scheduling, not personal weekly planners — likely understates the consumer planner opportunity but useful as a floor.

### Best TAM Number to Anchor on for Planny
- **Conservative TAM (US ADHD apps): $773M (2025)**
- **Aggressive TAM (US ADHD apps + US productivity overlap for ADHD adults): ~$1.0-1.2B**
- Global ADHD apps for context: $1.8-2.2B, growing to ~$4B by 2029.

---

## SAM (Serviceable Addressable Market — ADHD adults in the US)

### Population base (Tier 1 — CDC)
- **15.5 million US adults** with current ADHD diagnosis (CDC NCHS Rapid Surveys, Oct–Nov 2023; published MMWR 2024). Source: cdc.gov/mmwr/volumes/73/wr/pdfs/mm7340a1-H.pdf
- That = **6.0% of US adults** (≈1 in 16).
- 55.9% of these were first diagnosed in adulthood — the cohort most likely to seek self-management tools.
- Extrapolated to 2025: ~**16.13 million adults** (Huntington Psych analysis; Tier 2).
- Adult ADHD diagnoses grew **123.3% from ~2007-2022** vs 26.4% for children — 4x faster (Tier 2, Epic Research / additude).
- Underdiagnosis: academic literature commonly cites true adult ADHD prevalence around **4.4-10.2%** (NIMH / Brown Health / Utah Health — Tier 1/2), so the addressable pool may be larger than the diagnosed pool.

### Penetration assumption
- Mental health/wellness app penetration of target conditions runs ~5-15% of diagnosed population (proxy from Calm/Headspace anxiety user reach).
- Conservatively assume **8% of diagnosed US adult ADHD population would consider a paid scheduling app**: 16.13M × 8% = **~1.29M reachable buyers**.
- Aggressive case at 15% = **~2.42M**.

### ARPU assumption (subscription-only, no free tier)
- Productivity apps lead all categories in US LTV per RevenueCat 2026 SOIS: average plan-blended LTV ~$46.97. Source: revenuecat.com/state-of-subscription-apps
- ADHD-specific comps cluster around **$4-8/mo equivalent on annual plans** (Tiimo $4.50/mo annual; Routinery $2.50/mo annual; Inflow tools-only $8/mo annual).
- A reasonable Planny ARPU assumption: **~$60/year ($5/mo blended)** given subscription-only model, no free tier filter, and ADHD-niche premium.

### SAM math
| Scenario | Reachable buyers | Annual ARPU | SAM |
|---|---|---|---|
| Conservative | 1.29M | $60 | **~$77M/yr** |
| Base | 1.94M (12%) | $72 | **~$140M/yr** |
| Aggressive | 2.42M | $90 | **~$218M/yr** |

**SAM anchor: ~$77-140M annual revenue opportunity in the US ADHD-adult scheduling-app niche.** This is consistent with the $773M US ADHD-apps TAM figure (Planny's slice = ~10-18% of broader ADHD app category, which is realistic for a focused scheduling-only player).

---

## SOM (Serviceable Obtainable Market — Year 1 realistic capture)

### Reality check for a solo bootstrap founder with $1,500 budget

**The $1,500 budget is the binding constraint, not the market.** Working backward from CAC:

- iOS CPI in North America: **~$3.6-4.70** (Business of Apps, Mapendo 2025 — Tier 1/2).
- Android CPI in NA: ~$1.20.
- That's *install* cost. Actual paying-subscriber CAC after trial conversion (~38% RevenueCat median) is **~$10-30/user** (Tier 1).
- Onboarding+install-to-trial-start friction means effective paid CAC for an ADHD niche subscriber is likely **$15-40 on iOS, $8-20 on Android**.

### $1,500 paid-acquisition math
| Channel mix | Effective CAC | Paid subscribers Y1 |
|---|---|---|
| iOS-heavy paid | $25 | ~60 |
| Mixed iOS/Android paid | $15 | ~100 |
| Organic + content + community (likely path) | $0-5 effective | 200-1,000+ if any TikTok/community traction |

### Comparable bootstrap trajectories
- **Routinery** (ADHD-adjacent habit app, Korean indie): reached millions of downloads over multi-year window — Y1 paid subscribers likely in low-thousands.
- **Tiimo** (Denmark, ADHD/autism planner): now 500k+ users but took 6+ years and venture funding. App Store Award 2025.
- **Inflow** (UK-founded ADHD app): VC-backed, $11M+ raised; took 2-3 years to hit meaningful scale.
- **Bootstrap indie productivity apps** (e.g., one-person developers shipping on RevenueCat) typically hit **$10-50k ARR in Y1**, per RevenueCat's median-app distribution. The top quartile reaches $100k+ ARR Y1.

### SOM ranges for Planny Y1
| Scenario | Paid subs Y1 | Annual revenue Y1 |
|---|---|---|
| Pessimistic (paid-only $1.5k, no organic) | ~60-100 | ~$3,600-6,000 |
| Realistic (paid + modest organic/TikTok/ADHD community) | 300-800 | ~$18,000-48,000 |
| Optimistic (one viral TikTok hit + r/ADHD adoption) | 1,500-3,000 | ~$90,000-180,000 |

**SOM anchor for planning: $15-50k ARR Y1** is the realistic base case. **Reaching $100k ARR Y1 requires at least one community/content breakout** — possible but not the median outcome for a solo founder with $1,500.

---

## Unit Economics Benchmarks

| Metric | Benchmark | Source | Tier |
|---|---|---|---|
| **ARPU (subscription apps, blended)** | $3-9/mo | BusinessDojo, MobileAction 2025 | Tier 2 |
| **ARPU (productivity, US)** | $46.97 LTV/user (best country-category combo globally) | RevenueCat SOIS 2026 | Tier 1 |
| **ARPU (NA users on subscription apps)** | $6.20/mo | Mapendo / Coinis 2025 | Tier 2 |
| **iOS CPI (North America)** | $3.6-4.70 | Business of Apps, Mapendo | Tier 1 |
| **Android CPI (NA)** | ~$1.20 | Business of Apps | Tier 1 |
| **Paid CAC (US productivity subscription)** | $10-30/paying user | Business of Apps, BusinessDojo | Tier 2 |
| **iOS ARPU advantage** | Annual ARPU $138 (iOS) vs $72 (Android) per BusinessDojo | BusinessDojo Oct 2025 | Tier 2 |
| **Monthly churn (B2C mobile subscription, blended)** | ~9% | RevenueCat SOIS 2025 | Tier 1 |
| **Monthly churn (best-in-class B2C)** | 3-4% | SubJolt / Focus Digital 2025 | Tier 2 |
| **First-month cancellation rate (annual subs)** | ~30% | RevenueCat SOIS 2025 | Tier 1 |
| **First renewal churn (monthly plans)** | 15-40% | RevenueCat SOIS 2025 | Tier 1 |
| **First renewal churn (weekly plans)** | 30-50% | RevenueCat SOIS 2025 | Tier 1 |
| **Annual retention (cheap annual plans)** | ~36% still subscribed after 1 year | RevenueCat SOIS 2025 | Tier 1 |
| **Trial-to-paid (RevenueCat median mobile)** | 38% | RevenueCat SOIS 2025/2026 | Tier 1 |
| **Trial-to-paid (top quartile mobile)** | 60%+ | RevenueCat SOIS | Tier 1 |
| **Opt-in trial conversion (no card)** | 8.9-18.2% | First Page Sage, ChartMogul | Tier 2 |
| **Opt-out trial conversion (card required)** | 31.4-48.8% | First Page Sage, ChartMogul | Tier 2 |
| **Trial conversion decline YoY** | 46% → 33% (Recurly 2025) | Recurly | Tier 1 |
| **Day-1 retention (productivity apps)** | 17.1% | Amraandelma 2025 | Tier 2 |
| **Day-30 retention (productivity apps)** | 4.1% | Amraandelma 2025 | Tier 2 |
| **LTV (Productivity, blended)** | $46.97 (best country-category in world) | RevenueCat SOIS 2026 | Tier 1 |
| **LTV (Health & Fitness)** | $16.44 median, $31.12 upper quartile | RevenueCat SOIS 2026 | Tier 1 |

### Implied LTV math for Planny
- If monthly ARPU = $5, monthly churn = 7% (between best-in-class and average for niche/mission-aligned apps), simple LTV = $5 / 0.07 = **~$71/user**.
- If monthly churn drops to 5% (premium retention), LTV = **~$100/user**.
- If monthly churn is 10% (typical mobile B2C), LTV = **~$50/user**.
- **LTV:CAC ratio target of 3:1** implies sustainable CAC ceiling of $17-33/user — feasible only with organic/community-heavy acquisition.

---

## ADHD-Specific Economics

**Direct, audited data on ADHD-only app cohorts is not publicly available** (DATA GAP — companies like Inflow, Tiimo, Routinery don't publish churn/LTV). The proxies below are best available:

### What we know directly
- **Inflow study (Tier 1, PMC9931323)**: participants used the app a median of **3.86 times/week**; majority of 7-week users self-reported decreased ADHD symptoms. This implies higher engagement than typical mental-health apps — a positive signal.
- **Mental health apps overall**: only **3.3% retain at day 30**; **97% abandon within 30 days** (HCPLive, Wallace PhD analysis — Tier 2). Best-in-class evidence-based mental health apps hit **16% day-30 retention**.
- **Productivity apps**: day-30 retention 4.1% (Tier 2) — also brutal.

### What this implies for ADHD audience specifically
- ADHD adults have *higher willingness to seek tools* (per CHADD, ADDA, additudemag editorial content) — the search intent and community demand are demonstrable.
- BUT ADHD is itself a disorder of follow-through. **Retention risk is structurally elevated** vs. neurotypical productivity users. Inflow's 7-week study cohort had medical-study selection bias (self-selecting committed users) and shouldn't be projected to the general install base.
- WTP for ADHD-targeted apps appears robust at the **$3-8/mo annual-plan tier** (Tiimo $4.50, Routinery $2.50, Habitica $4.99). Inflow at $22.49/mo (tools only) and $47.99/mo (with coaching) shows a separate "ADHD + coaching" premium tier exists — but coaching is a different product.
- The ADHD community is concentrated on **TikTok, r/ADHD (3M+ subscribers), Instagram** — meaning organic/content acquisition is unusually viable for this niche vs. most B2C subscription apps.

### Proposed Planny working assumptions
- **Monthly churn: 8-12%** (vs. 9% mobile B2C average) — slight penalty for ADHD follow-through risk, partially offset by stronger mission resonance.
- **Trial-to-paid: 25-35%** (below 38% RevenueCat median if using paywall opt-in, near median if opt-out trial with card).
- **ARPU $5-6/mo blended**.
- **LTV: $50-75 base case**.

---

## Israel Market (Brief)

**Data is thin** — no Israel-specific ADHD app market sizing published.

- **42matters (Tier 2)**: 995 active Israeli mobile app developers on Google Play, 3,572 Israeli apps, avg 1.51M downloads — small but technically sophisticated ecosystem.
- ADHD prevalence in Israel is comparable to or slightly above OECD averages (Israeli MoH data, generally cited at ~5-6% of adults), but no current 2024-2026 government survey publicly available.
- Israeli adult population ~6M; at ~6% adult ADHD = **~360k diagnosed adults**. At 10% reachable = **~36k buyers**. At $60 ARPU = **~$2.2M annual SAM** — roughly 2-3% of US SAM.
- **Implication**: Israel is a useful Beta/launch market (founder home advantage, lower competition, Hebrew-language differentiation) but **not a primary revenue engine**. Treat as test bed, not TAM.

DATA GAP: No public sizing of Israeli ADHD app market. Founder should reference (a) Israeli MoH ADHD prevalence reports, (b) Sensor Tower / data.ai country reports for app spend in IL, (c) direct outreach to Israeli ADHD orgs (e.g., אדהד.ארגון).

---

## Comparable Pricing Landscape

| App | Monthly | Annual | Free Tier | Free Trial | ADHD-positioned? | Notes |
|-----|---------|--------|-----------|-----------|------------------|-------|
| **Motion** | $19 | $152 ($12.73/mo) | No | 7 days | No (general AI scheduler) | Pro tier; Business $29/$233 |
| **Reclaim.ai** | ~$10-15 | ~$96-180 | Yes (free tier) | n/a | No | Cheaper than Motion (per Setapp) |
| **Sunsama** | $22 | $204 ($17/mo) | No | 14 days | No (mindful daily planner) | Strong overlap w/ ADHD intent |
| **Tiimo** | $4.99-12 (varies by platform) | $42-54 ($3.50-4.50/mo) | Yes (basic) | 7 days | YES (neurodivergent-first) | App Store Award 2025; closest competitor |
| **Routinery** | $3 | $30 ($2.50/mo) | Yes | 7 days | YES (routine for ADHD/autism) | Cheapest in segment |
| **Inflow (tools only)** | $22.49 | $95.99 (~$8/mo) | No | 7 days | YES (ADHD-specific) | VC-backed; CBT-based |
| **Inflow (w/ coaching)** | $47.99 | $199 | No | 7 days | YES + coaching | Premium tier |
| **Habitica** | $4.99 | $47.99 | Yes | No | No (gamified habits, ADHD-popular) | Reddit favorite |
| **Calm** (mental wellness benchmark) | $16.99 | $69.99-79.99 | No | 7 days | No | Pricing ceiling for B2C wellness |
| **Headspace** (benchmark) | $12.99 | $69.99 (often 50% off) | No | 14 days | No | Annual ~$35 promo |

**Pricing implication for Planny:**
- **The ADHD-positioned subset clusters at $3-8/mo on annual plans** ($30-96/yr).
- Premium AI schedulers (Motion, Sunsama) at $150-200/yr exist for the productivity-pro market — Planny could anchor higher if AI value is clearly demonstrated, but starting at $50-80/yr annual / $7-10/mo monthly fits the ADHD price corridor best.
- **No-free-tier model is consistent with Inflow, Sunsama, Motion, Calm, Headspace** — defensible but raises trial conversion as the existential metric.

---

## Market Headwinds & Failure Modes

| Risk | Severity | Source | Tier |
|---|---|---|---|
| **Productivity apps day-30 retention is 4.1%** — structural abandonment | High | Amraandelma 2025 | Tier 2 |
| **Mental health apps day-30 retention is 3.3%** — even worse | High | HCPLive, Wallace PhD | Tier 2 |
| **"Productivity theater" failure mode** — apps add cognitive load instead of removing it; ADHD users especially vulnerable | High | Siddhify, Vocal Media | Tier 3 |
| **Feature overload / setup friction kills task apps within ~2 weeks** | High | Multiple Tier 2/3 sources | Tier 2/3 |
| **Trial conversion declining YoY** (46% → 33% Recurly 2025) — subscription fatigue real | Medium | Recurly | Tier 1 |
| **First-month cancellation 30%+ on annual plans** | Medium | RevenueCat SOIS 2025 | Tier 1 |
| **Crowded competitive set** — Tiimo, Routinery, Inflow already well-positioned in ADHD niche; Motion/Sunsama/Reclaim in AI scheduling | Medium-High | Direct observation, App Store | Tier 1 |
| **iOS CAC ($25-40 effective) consumes $1,500 budget after ~40-60 paying subs** — paid acquisition not viable at this budget | High | Business of Apps + math | Tier 1 |
| **ADHD users may have higher refund/dispute rates** (impulsivity) | Medium | Inferred — no hard data | DATA GAP |
| **App Store/Google Play 30% fee** on subscriptions <$1M ARR per dev | Medium | Apple/Google policy | Tier 1 |
| **AI feature commoditization** — ChatGPT/Claude/Gemini eating standalone "AI planning" niche | Medium | Industry trend | Tier 2 |

---

## Strategic Implications for Planny

1. **The market is real but small enough to matter — and big enough to support a profitable indie business.** US ADHD app TAM ~$773M; realistic SAM $77-140M; a 0.05-0.1% capture = $40-140k ARR is a defensible "happy bootstrap" outcome. Don't expect VC-scale numbers — but also don't dismiss the opportunity.

2. **$1,500 cannot buy paid acquisition at meaningful scale.** Effective iOS CAC of $25-40 means budget yields ~40-60 paying users. **Planny's GTM must be organic-first** — TikTok ADHD community, r/ADHD, Instagram, ADHD coaches/therapists referrals, content. The ADHD community is unusually concentrated and reachable. Plan accordingly or the budget runs out before product-market fit.

3. **Pricing should anchor at $5-8/mo annual / $50-80/yr** — between Routinery (too cheap, signals unserious) and Inflow tools-only ($8/mo). A monthly option at $9.99 and a 6-month and annual plan are consistent with the segment. Subscription-only (no free tier) is defensible but makes the **paywall, onboarding, and trial-to-paid conversion the single most important product surface** — trial-to-paid will determine whether the business works or not.

4. **Retention is THE existential risk, not market size.** Productivity-app day-30 retention is 4.1% and mental-health is 3.3%. ADHD users are structurally prone to abandonment. Planny must build for **behavioral retention** (streaks, gentle nudges, "low-commitment recovery" flows for ADHD-specific drop-off patterns) — not just feature completeness. The 36% annual retention figure for cheap annual plans is the ceiling Planny should aim at, and beating it requires ADHD-native engagement design, not generic productivity tropes.

---

## Source Quality Assessment

### Tier 1 (analyst reports, government, academic)
- CDC NCHS MMWR Sept 2024 — adult ADHD prevalence — **gold standard for the SAM denominator**
- CDC Data Briefs (Dec 2025) — ADHD data
- Mordor Intelligence — Productivity Apps Market 2025-2030
- Fortune Business Insights — Productivity Apps Market 2034 forecast
- The Business Research Company — Productivity Software & ADHD Apps reports
- Grand View Research — Scheduling Apps Market 2033
- Statista Market Forecast — Productivity worldwide
- RevenueCat State of Subscription Apps 2025 + 2026 (115k+ apps, $16B+ revenue)
- Recurly subscription benchmarks (67M subscribers)
- Business of Apps — CPI, retention, trial benchmarks
- PMC9931323 — Inflow CBT-based ADHD app feasibility study
- Apple/Google fee policies

### Tier 2 (TechCrunch-level / specialized industry / corporate analytics)
- Adapty State of In-App Subscriptions 2026
- First Page Sage / ChartMogul trial conversion studies
- BusinessDojo, Mapendo — CPI and ARPU analyses
- 42matters — Israel app market statistics
- HCPLive — Mental health app retention reporting
- Huntington Psychological Services — adult ADHD statistics aggregation
- Additude Magazine — ADHD statistics
- nchstats / NCHStats — US ADHD aggregations
- Wallace PhD (Medium / Advances in AI for Mental Health) — retention analysis
- Setapp, Toolguide, Productivewithchris — competitor pricing reviews
- Data Insights Market — ADHD planner sub-segment
- Market Growth Reports — ADHD Apps regional breakouts
- SubJolt, Focus Digital, CustomerGauge — churn benchmarks

### Tier 3 (blogs, secondary aggregators)
- Vocal Media, Siddhify — productivity-app failure analysis
- Jill Johnson Coaching aggregations
- Various app review blogs (Giodella, Morgen, Choosing Therapy, Zenmaster)

---

## Data Gaps

1. **ADHD-only app cohort retention/churn data** — Tiimo, Inflow, Routinery don't publish. Suggest: scrape App Store/Sensor Tower for download trends; reach out via founder-to-founder DMs; check Crunchbase for funding stage as a proxy for traction.
2. **Israel ADHD app market sizing** — no published reports. Suggest: Israeli MoH adult ADHD prevalence reports; Sensor Tower country deep-dive (paid); direct conversation with the ADHD Israel association (ארגון אדהד ישראל).
3. **ADHD adults' actual spending on productivity apps** — Additude/CHADD have audience surveys but pricing-elasticity data is not public. Suggest: founder runs own pre-launch landing-page test with price A/B; Maven Clinic / ADHD coaching businesses may have anonymized data.
4. **Refund/chargeback rates among ADHD subscribers** — purely inferred. Suggest: ask RevenueCat sales for a category benchmark, or check Apple/Google's refund category data via dev console.
5. **Reclaim.ai exact 2026 pricing** — public site changed; not captured cleanly in search. Suggest: direct visit reclaim.ai/pricing.
6. **Conversion data for ADHD-niche paywalls specifically** — DATA GAP. Adapty or RevenueCat case studies (paid) may have anonymized comps.

---

## Flags

### Red Flags
**None identified at the market-size level.** The market exists, is growing 15-16% (faster than productivity overall), and has a defensible US base of 15-16M diagnosed adults. The category supports multiple profitable subscription apps already (Tiimo, Routinery, Inflow).

### Yellow Flags

1. **Retention is structurally bad** in both productivity (4.1% D30) and mental-health (3.3% D30) categories. ADHD audience layered on this means retention design is do-or-die. Not fatal, but founder should explicitly plan around it.

2. **$1,500 budget vs. iOS CAC math doesn't work for paid acquisition.** Founder is implicitly betting on organic/community channels. If those don't work in the first 3-4 months, runway is exhausted with <100 paying users.

3. **Crowded competitive set.** Tiimo just won 2025 App Store Award; Inflow is VC-backed; Routinery is established. Differentiation must be sharp — "AI weekly schedule" needs to be visibly different from Tiimo's visual planner and Motion's AI scheduling, not a thin overlap of both.

4. **Trial-to-paid conversion is declining industry-wide** (46% → 33% YoY per Recurly). Subscription fatigue is real. Subscription-only with no free tier is a strong stance but raises stakes on every paywall decision.

5. **AI feature commoditization risk.** ChatGPT/Claude can already help an ADHD adult plan a week. Planny must offer durable ADHD-native UX advantages (notification patterns, gentle re-engagement, executive-function scaffolding) rather than a thin AI wrapper. Pricing power erodes fast if the differentiator is "AI."

6. **Israel as a secondary market is fine but data-thin.** Don't build financial projections that depend on Israel revenue.
