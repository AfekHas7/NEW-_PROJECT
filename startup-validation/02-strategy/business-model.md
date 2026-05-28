# Business Model — Planny

**Phase:** Phase 4 — Strategy (Business Model)
**Project:** startup-validation (Planny)
**Date:** 2026-05-28
**Confidence:** Medium-High — pricing/CAC/LTV benchmarks Tier 1 (RevenueCat 2026, Adapty 2025, AppTweak 2026); ADHD-specific retention ו-trial conversion הם פרוקסי, לא נתונים אקטואליים של Planny

---

## תקציר מודל עסקי

**מודל:** B2C SaaS subscription, mobile-first (iOS-first → Android month 3-4)
**מפלח:** ADHD adults; beachhead = late-diagnosed US women 25-40 (persona "Maya", NYC/NJ/LA/Seattle knowledge workers)
**מודל הכנסה:** subscription בלבד (monthly / 6-month / annual) — אין free tier; trial 14-day opt-in (CC required) באנואלי בלבד
**מסלול:** Bootstrap → product-market-fit signals @ ~$5K MRR → re-evaluate (founder salary / external capital / acceleration) @ ~$10K MRR
**עיתוי קריטי:** WWDC June 8, 2026 (in 11 days) הוא binary risk event; כל positioning חייב להיות vertical/ADHD-specific לא horizontal AI scheduler

---

## Revenue Model

### Pricing Tiers

| Tier | Price | Effective $/mo | Free Trial | Refund |
|------|-------|----------------|------------|--------|
| Monthly | $9.99 | $9.99 | אין | 30-day no-Q |
| 6-month | $39.99 | $6.67 (33% הנחה) | אין | 30-day no-Q |
| Annual | $59.99 | $5.00 (50% הנחה) | 14-day opt-in (CC) | 30-day no-Q (sessions <10) |

### Anchor Logic
- **Tiimo $54/yr** (App Store of the Year 2025) מקבע את הרצפה לתמחור ADHD-specific
- **Numo $59.99/yr** = exact match — הוכחה שהמחיר עובד עם adult-ADHD audience
- **Inflow tools-only $96/yr** = תקרת ה-"trust" — מעליה backlash על billing reputation
- **Sunsama $204/yr / Motion $228-348/yr** = תקרת AI scheduling generic — לא comp set ל-Maya
- **Planny $59.99/yr** = parity עם Numo, מתחת ל-Inflow ב-37%, מאפשר reinvestment משמעותי

### למה לא Free Tier
1. **Inflow ניסה (tools tier)** — שילם $11M ב-Meta/TikTok ad spend → category-level billing reputation problem; free tier לא הציל את ה-CAC
2. **Tiimo עם free tier** — 90%+ נשארים free, conversion <5% per category proxy; Planny עם $1,500 בלבד לא יכולה לשרת חינמיים
3. **LLM API costs** — בלי revenue per active user, $0.10-0.30/mo per user × free base יסחט את ה-runway תוך 60 ימים
4. **Persona signal** — Maya רוצה "tool that takes itself seriously" — free tier מסכן את ה-trust-positioning
5. **המסלול ההגיוני:** subscription-only עם 14-day opt-in trial על annual + 30-day no-Q refund

### Plus: Pricing Psychology
- **3-tier display** עם annual pre-selected, badged "Most Popular / Save 50% + 14 days free"
- **6-month = decoy** (strictly dominated by annual on $/mo, strictly dominated by monthly on flexibility) — מרים annual selection 30-40% (InnerTrends, Monetizely 2025)
- **Apple price-point mapping (post-2023 system):** $9.99 / $39.99 / $59.99 ישירות
- **Israel localization (post month 6):** ₪34.90 / ₪139.90 / ₪199.90 (rounded to .90 psychology, ~94% PPP flat conversion)
- **"2 months free, billed yearly. Save $60 vs monthly"** — framing per Wingback/InnerTrends data

---

## Unit Economics

### Per-User Variable Costs (monthly)
| Component | Cost | Notes |
|---|---|---|
| Apple/Google fee | **30% year 1 / 15% Small Business Program** | SBP requires <$1M ARR; apply at launch |
| LLM API (GPT-4o-mini / Claude Haiku) | **$0.10-0.30/mo per active user** | Caching + prompt optimization keeps flat at scale |
| Push notifications (OneSignal free → paid tier) | **$0.001/user/mo** | Free up to 10K subscribers |
| Database (Supabase) | **$0.05/user/mo** | At small scale; drops to $0.02 at 5K+ |
| Auth + storage | **$0.02/user/mo** | Bundled in Supabase tier |
| **Total variable cost per active user** | **~$0.17-0.37/mo** | Excludes app store cut |

### Per-User Revenue (Net, after Apple/Google cut)

**Year 1 (30% cut):**
- Monthly tier: $9.99 × 70% = **$6.99**
- 6-month tier: $39.99 × 70% / 6 = **$4.67/mo**
- Annual tier: $59.99 × 70% / 12 = **$3.50/mo**

**Year 2+ (15% cut, post Apple SBP):**
- Monthly: $9.99 × 85% = **$8.49**
- 6-month: $39.99 × 85% / 6 = **$5.67/mo**
- Annual: $59.99 × 85% / 12 = **$4.25/mo**

**Weighted blend (תחזית tier mix, 40% monthly / 30% 6mo / 30% annual):**
- Year 1: (0.40 × $6.99) + (0.30 × $4.67) + (0.30 × $3.50) = **$5.24/mo effective net**
- Year 2 (SBP): (0.40 × $8.49) + (0.30 × $5.67) + (0.30 × $4.25) = **$6.37/mo effective net**

### Per-User Gross Margin

| Year | Revenue net (blended) | Variable cost | Gross margin $ | Gross margin % |
|---|---|---|---|---|
| Year 1 (30% cut) | $5.24/mo | $0.30/mo | **$4.94/mo** | **94.3%** |
| Year 2 (15% cut, SBP) | $6.37/mo | $0.30/mo | **$6.07/mo** | **95.3%** |

### LTV Calculation

**Approach A — Churn-implied LTV (monthly cohort):**
- Assumed monthly churn: **8-10%** (between best-in-class 4% and B2C blended 9%; penalty for ADHD follow-through risk, partially offset by mission resonance)
- LTV @ 8% churn = $5.24 / 0.08 = **$65.50**
- LTV @ 10% churn = $5.24 / 0.10 = **$52.40**

**Approach B — RevenueCat productivity benchmark:**
- Productivity LTV (US, best country-category combo): **$46.97** (RevenueCat SOIS 2026)
- ADHD-niche premium expected (+10-20%): **$52-57**

**Approach C — Annual cohort retention (RevenueCat):**
- ~36% retain after 12 months on cheap annual plans
- Annual: $59.99 × 70% = $41.99 net year 1; ~36% × $41.99 = $15.12 expected year 2 net → **$57 cumulative LTV at 24 months**

**Blended LTV estimate: $50-65 base case** — consistent with all three approaches and RevenueCat productivity benchmark.

### CAC Ceiling
- **LTV / 3 = $17-22 maximum sustainable CAC** (industry rule 3:1)
- **Apple Search Ads productivity CPA 2025: $2.84** (AppTweak) — well within ceiling, but volume capped on niche keywords
- **iOS CPI productivity NA: $2.84-4.70**; effective paid CAC (post trial conv) **$15-40**
- **Inflow-poisoned Meta/TikTok auctions:** effective CAC > $30 → unsustainable
- **Organic + Tracy Otsuka deal:** blended CAC **$5-12** target

### LTV:CAC Targets
| Channel mix | Effective CAC | LTV/CAC ratio | Status |
|---|---|---|---|
| Organic-heavy (TikTok + r/ADHDWomen + content) | $0-5 | 10:1+ | Ideal |
| Tracy Otsuka host-read + ASA long-tail | $5-12 | 4-12:1 | Healthy |
| ASA broad + niche Meta retargeting | $15-25 | 2-4:1 | Acceptable |
| Paid-only Meta/TikTok (Inflow auctions) | $30+ | <2:1 | Unsustainable |

---

## Scenarios — 12-Month Trajectory

### Conservative (50th percentile — solo founder, modest organic traction, no breakout)

| Month | Total Users | Paying | MRR | ARR (run-rate) | Reinvestment Pool |
|-------|-------------|--------|-----|----------------|-------------------|
| 1 | 200 | 8 | $42 | — | $1,500 + $42 |
| 2 | 500 | 25 | $130 | — | ~$1,200 + $130 cumulative |
| 3 | 900 | 55 | $290 | $3.5K | ~$900 + $290 |
| 6 | 2,000 | 150 | $780 | $9.4K | ~$300 base + $780/mo flow |
| 9 | 3,500 | 280 | $1,460 | $17.5K | $1,460/mo flow |
| 12 | 5,500 | 450 | $2,340 | **~$28K ARR** | $2,340/mo flow |

### Base (median expectation — Tracy Otsuka episode airs, micro-creator seeding works)

| Month | Users | Paying | MRR | ARR | Reinvest pool |
|-------|-------|--------|-----|-----|---------------|
| 1 | 350 | 18 | $94 | — | $1,500 + $94 |
| 2 | 800 | 50 | $260 | — | ~$1,200 + $260 |
| 3 | 1,500 | 110 | $570 | $6.8K | ~$900 + $570 |
| 6 | 4,000 | 320 | $1,660 | $19.9K | $1,660/mo |
| 9 | 7,000 | 580 | $3,015 | $36.2K | $3,015/mo |
| 12 | 11,000 | 850 | $4,420 | **~$53K ARR** | $4,420/mo |

### Optimistic (90th percentile — Tracy Otsuka viral + TikTok breakout + ADDitude editorial)

| Month | Users | Paying | MRR | ARR | Reinvest pool |
|-------|-------|--------|-----|-----|---------------|
| 1 | 600 | 35 | $182 | — | $1,500 + $182 |
| 2 | 1,800 | 120 | $625 | — | ~$1,300 + $625 |
| 3 | 4,000 | 280 | $1,455 | $17.5K | $1,455/mo |
| 6 | 10,500 | 850 | $4,420 | $53K | $4,420/mo |
| 9 | 18,000 | 1,520 | $7,900 | $94.8K | $7,900/mo |
| 12 | 26,000 | 2,300 | $11,960 | **~$143K ARR** | $11,960/mo |

### Pessimistic (10th percentile — WWDC Apple commoditization OR retention collapse)

| Month | Users | Paying | MRR | Notes |
|-------|-------|--------|-----|-------|
| 1 | 200 | 8 | $42 | WWDC June 8 announcement chills excitement |
| 3 | 600 | 25 | $130 | Pivot to "ADHD layer over Apple Intelligence" positioning |
| 6 | 1,200 | 70 | $365 | Slow grind, organic only, no Tracy deal closed |
| 12 | 2,500 | 180 | $935 | **~$11K ARR** — pivot or wind down |

### Pessimistic-2 (Retention disaster — D30 <5%)
- Month 3: 1,500 users, 110 paying — same as base
- Month 6: 1,800 users, 120 paying — 60% of cohort churns, MRR stuck at $624
- Month 12: 2,400 users, 140 paying — MRR $728, **~$8.7K ARR**, retention design failed, runway exhausted
- **This is the existential failure mode.**

---

## Sensitivity Analysis

### Variable 1: Trial-to-Paid Conversion
- **Benchmark range:**
  - RevenueCat median (opt-out, mobile): 38%
  - Opt-in trial (no CC): 18-25%
  - 5-9 day trials: 45% / 10-16 day trials: 44%
  - ADHD-specific guesstimate: **20-30%** (impulse spending offset by ADHD guilt; high-intent late-dx cohort offsets)
- **Planny model assumption: 25%** (14-day opt-in CC trial, ADHD audience)
- **Sensitivity:**
  - -50% (12.5% conv) → ARR drops ~40%
  - +50% (37.5% conv) → ARR climbs ~35%
- **Highest-leverage decision in entire model.** Trial structure + paywall design = the single product surface that determines whether business works.

### Variable 2: Day-30 Retention
- Productivity benchmark: **4.1% D30**
- Mental-health benchmark: **3.3% D30**
- Best-in-class evidence-based health apps: **16% D30**
- Planny target: **15% D30** (ADHD-native design + weekly cadence + gentle re-engagement)
- **Sensitivity:**
  - At 4.1% (category default): LTV collapses to $25-30, model broken
  - At 10%: LTV ~$45, marginal
  - At 15%: LTV $50-65, model works
  - At 20%+: LTV $75+, business genuinely good
- **Retention is the existential variable. More important than CAC, pricing, or feature set.**

### Variable 3: Apple/Google Fee (Small Business Program)
- **Year 1 default: 30%** (gross)
- **SBP eligibility: <$1M annual proceeds** → 15% from approval
- **Apple SBP:** apply via App Store Connect; approval typically <30 days
- **Google Play 15% tier:** automatic for first $1M/year per account
- **Sensitivity:**
  - 30% → 15%: gross margin per user climbs from 94.3% to 95.3%; net revenue per paid user climbs ~21%
- **Action item: Apply to Apple SBP at App Store Connect launch (week 2 of submission).**

### Variable 4: Marketing Channel CAC
- **Organic-only (zero direct spend):** effective CAC $0-5 — LTV/CAC 10:1+
- **Tracy Otsuka host-read ($1,500 deal):** if 100 paid subs result → CAC $15; if 200 → CAC $7.50
- **Apple Search Ads (long-tail, defensive):** $2.84-4.50 CPA → CAC $10-20 post-trial
- **Niche Meta retargeting (post-month 4):** $10-15 effective
- **Inflow-poisoned cold acquisition:** $30+ → unsustainable
- **Mitigation:** never spend >40% of monthly reinvestment pool on paid; always keep 60%+ in organic compounding (content, creator partnerships, SEO)

### Variable 5: Refund Rate
- **Target: <2% of annual buyers** (sessions-gated, <10 sessions in 30 days)
- **Inflow precedent (fuzzy refunds, billing complaints):** ~5-8% effective refund/dispute rate
- **Sensitivity:** every 1% increase = ~$X loss; at $50K ARR, 5% refunds = $2.5K leakage

---

## Cost Structure

### Fixed (monthly, at launch)
| Item | Cost |
|---|---|
| Apple Developer Program | $8/mo (annualized $99) |
| Google Play Developer | ~$0/mo (after $25 one-time) |
| Backend hosting (Vercel/Supabase free → paid) | $20-50/mo |
| LLM API (~50 active users early) | $10-30/mo |
| Push notifications (OneSignal free <10K) | $0 |
| Domain + email (Google Workspace) | $10/mo |
| ConvertKit / email service (<1K subs free) | $0 |
| RevenueCat (free <$2.5K MTR) | $0 |
| **Total fixed at launch** | **~$50-100/mo** |

### Variable (per active paid user)
- Apple/Google fee: 30% year 1 (15% post-SBP)
- LLM API: $0.10-0.30/mo
- Database: $0.05/mo
- Push + auth: $0.02/mo
- **Total: 30-35% of revenue + $0.15-0.35/active user**

### One-time (across first 6 months)
| Item | Cost |
|---|---|
| Legal (privacy policy + ToS + MHMDA Health Data Policy templates + light review) | $500-2,000 |
| Hebrew RTL localization (Israel launch month 6) | $300-900 |
| Brand assets / design | $0 (founder-produced) |
| App Store screenshots + listing optimization (DIY) | $0 |
| Apple Developer enrollment | $99 |
| Google Play enrollment | $25 |
| **Total one-time** | **$925-3,025** |

### Marketing (from $1,500 seed + revenue reinvestment)
**90-day initial allocation (from channels.md):**
- Tracy Otsuka pod episode: $800-1,500
- ADDitude newsletter slot OR ASA long-tail: $400-800
- Apple Search Ads (defensive brand + long-tail): $200-500/mo from month 2
- Free annual subs gifted to 25-50 micro-creators: $0 cash (revenue forgone, ~$1,500 perceived value)
- TikTok / r/ADHDWomen / Pinterest / Discord organic: $0
- Tools (Canva, ConvertKit, domain): $150

**Year 1 marketing total: $5,000-15,000** (mostly from reinvested revenue after month 3)

---

## Revenue Reinvestment Math (זה המייסד הדגיש)

### Compounding Formula

```
Monthly Spending Capacity = (Initial Seed - Cumulative Prior Spend) + Cumulative Net Revenue
```

**Month-by-month example (Base scenario):**

| Month | Net Revenue (after Apple cut) | Cumulative Net Rev | Cumulative Spend | Available Pool |
|---|---|---|---|---|
| 1 | $66 | $66 | $400 | $1,166 |
| 2 | $182 | $248 | $1,200 | $548 + $182 incoming |
| 3 | $399 | $647 | $1,500 (initial fully spent) | $647 + monthly inflows |
| 4 | $700 | $1,347 | $1,800 | reinvest fully each month from here |
| 6 | $1,162 | $4,000+ | scaling with revenue | $1,162/mo +- |
| 12 | $3,094 | ~$20K cumulative net | reinvest 100% | $3,094/mo |

**Practical implication:** Every paying user funds future acquisition. The faster Planny converts the first 50-100 users, the more aggressive the marketing engine becomes by month 3.

**Hidden risk #1 — retention dependency:** This compounds **only if retention holds**. If users churn at productivity benchmark (4.1% D30), reinvestment shrinks instead of grows. **Retention design is the existential variable.**

**Hidden risk #2 — cash flow lag:** Annual subscriptions get paid 100% upfront → Apple/Google holds for 30-45 days → Planny sees cash ~Day 60+ from subscription start. **Plan for 60-day working capital gap.**

**Hidden risk #3 — refund chargebacks:** 30-day no-Q refunds mean revenue isn't recognized as "safe" until day 30. If refund rate spikes to 5%+, reinvestment math breaks.

---

## Scalability Considerations

### What Scales Well
- **LLM cost per user stays flat ~$0.20/mo** even at scale (caching, prompt optimization, on-device inference for iOS 27+ post-WWDC)
- **Apple/Google handle billing infrastructure** — no Stripe/Paddle complexity, no PCI compliance
- **Mobile-first = no web support burden** — single codebase iOS/Android via shared backend
- **Organic content compounds** — TikTok / SEO / Pinterest pins have 3-6 month tails
- **Tracy Otsuka episode evergreen** — downloads accumulate 2-4 weeks post-drop + long tail

### What Breaks at Scale
- **Solo founder support load** — at 1,000+ paid, "talk to founder" becomes unsustainable → transition to community Discord at $2K MRR
- **App Store reviews maintenance** — at 5K+ users, negative reviews start emerging; ASO + review-response routine required
- **LLM compliance + safety monitoring** — at scale, need monitoring for harmful AI suggestions (medical advice edge cases, RSD-triggering responses)
- **Refunds at scale** — target <2% refund rate; at 5K paying × $60 avg × 2% = $6K/yr leakage (manageable); at 5% = $15K (problematic)
- **MHMDA compliance overhead** — Washington plaintiffs' firms active; at 10K+ users with WA exposure, formal Health Data Privacy Officer engagement required
- **Israel Amendment 13** — DPO threshold (10K or 100K — needs Israeli counsel clarification) becomes mandatory

### Scaling Triggers (operational)
| Trigger | Action |
|---|---|
| $2K MRR | Launch Discord community (reduces 1:1 founder support load) |
| $5K MRR | Hire fractional iOS contractor (one weekend/month feature shipping) |
| $10K MRR | Re-evaluate founder salary ($1.5-2.5K/mo); consider seed round optionality |
| 5K paid users | Engage MHMDA-aware privacy counsel for formal audit |
| 10K total users | Apple Small Business Program review (still <$1M proceeds) |
| Israel launch | Fractional Israeli DPO + counsel for Amendment 13 compliance |

---

## Dependencies

### Critical Dependencies (single-point-of-failure)
1. **Apple App Store approval** — Productivity category, no medical claims, clean marketing copy
2. **Google Play approval** — same; avoid Health Apps policy declaration
3. **Google Calendar OAuth Tier 1 approval** — 3-4 weeks Google review; submit ASAP (manual import fallback)
4. **OpenAI / Anthropic API stability** — fallback to alternative model required (provider-agnostic API layer)
5. **Apple Search Ads availability** in target geographies (US primary, IL secondary)
6. **RevenueCat (or alternative) for subscription management** — abstraction layer for IAP

### Strategic Dependencies (multi-year)
1. **Tracy Otsuka relationship** (or alternative ADHD media partner: William Curb, Kristen Carder, Dr. Tamara Rosier)
2. **CHADD / ADDitude editorial coverage** (or substitute)
3. **Focusmate integration partnership** (optional but high narrative value — Taylor Jacobson direct outreach)
4. **r/ADHDWomen community goodwill** (zero competitor presence + 700K members + unforgiving rules)

### Risk Mitigations
| Risk | Mitigation |
|---|---|
| App Store rejection | Productivity category + clean copy + privacy policy audit + no medical claims |
| Google Calendar OAuth delay | Submit week 1; manual `.ics` import as fallback |
| LLM provider lock | Build provider-agnostic API layer (OpenAI primary, Anthropic backup, future on-device) |
| Influencer drop-out | Diversify across 25-50 micro-creators, not single bet on Tracy Otsuka |
| Apple WWDC commoditization | Position vertical/ADHD-specific from day 1, never "AI scheduler" |
| Tiimo two-way sync release | Continuous shipping cadence; own weekly cadence + late-dx women positioning |

---

## Key Partnerships

### Day 1 (must)
- Apple Developer Program ($99/yr)
- Google Play Developer Program ($25 one-time)
- LLM provider (OpenAI GPT-4o-mini primary, Anthropic Claude Haiku backup)
- Backend infrastructure (Supabase + Vercel)
- RevenueCat (subscription management abstraction)

### Month 1-3 (priority)
- **Tracy Otsuka podcast** — host-read or cash + lifetime affiliate ($1,500-2,500 indie rate target)
- **ADDitude editorial relationship** — pitch founder story submission to submissions@additudemag.com
- **25-50 ADHD micro-creators** (10K-100K TikTok) — gifted annual access + 30% lifetime affiliate
- **r/ADHDWomen moderators** — AMA / beta tester program (4-6 week relationship build before any pitch)
- **Focusmate API integration** — partnerships@focusmate.com / Taylor Jacobson direct

### Month 6+ (growth)
- **CHADD organizational partnership** — newsletter listings, annual conference (defer to Year 2 budget)
- **ADDA professional directory listing**
- **iACTcenter / ICF ADHD coach affiliate program** — 25-35% lifetime commission
- **Apple HealthKit** (for sleep → energy mode integration)
- **Dr. Tamara Rosier** — clinical authority endorsement / podcast guest swap

---

## Founder Salary Plan

| Period | Salary | Trigger |
|---|---|---|
| Months 1-6 | **$0** | Full reinvestment; founder personal runway covers living |
| Months 7-12 | $0 → $1,500-2,500/mo | Conditional on $5K MRR threshold ($60K ARR run-rate) |
| Year 2 | $60-100K/yr | Conditional on $200K+ ARR; market-rate solo founder comp |

**Honest caveat:** No-salary policy works only if family/personal runway allows. If founder runs out of personal runway before month 6, the model collapses regardless of MRR trajectory.

---

## Exit / Path Scenarios (Long-term)

### Path A: Bootstrap to profitability ($300-500K ARR)
- Solo founder + 1-2 contractors (iOS, design)
- Self-funded long term
- Acquisition target benchmark: Sunsama-style $1.5M ARR bootstrap exit
- **Timeline:** 36-60 months

### Path B: Seed round ($500K-$1M)
- Trigger: $100-200K ARR + strong retention metrics (D30 >15%, annual retention >40%)
- Investors: ADHD-focused (Octopus Ventures, Worklife, A.Capital, Will Ventures)
- Comp: Inflow $11M Series A; Saner Techstars + Google; Shimmer $3.5M
- Use: hire iOS engineer + designer + ADHD coach advisory board
- **Timeline:** 12-18 months from launch

### Path C: Strategic acquisition
- Comp: Reclaim → Dropbox **$40.2M** (320K users, Jul 2024) → ~$125/user enterprise value
- Potential acquirers:
  - **Calm/Headspace** (mental wellness expansion into ADHD)
  - **ADDitude parent (WebMD?)** (content + product bundle)
  - **Microsoft** (productivity ecosystem)
  - **Google** (Workspace integration)
  - **Tiimo** (consolidation play if VC-backed)
- Realistic timeline: 24-36 months at $1M+ ARR

### Path D: Failure modes (be honest)
1. **Apple Intelligence commoditizes** (WWDC June 8) → pivot to "ADHD layer over Apple Intelligence" OR shut down
2. **Retention < 5% D30** → reach end of seed budget, can't fund reinvestment compound → wind down month 6-9
3. **Saner.AI raises Series A and clones features** → must out-execute on weekly cadence + women's positioning, or out-position
4. **Tiimo releases two-way calendar sync** → loses primary technical wedge → pivot to emotional/energy-aware AI as differentiator
5. **MHMDA/FTC enforcement action** (e.g., ad pixel violation) → settlement risk $1-7M, business-ending for bootstrap
6. **Founder personal runway exhaustion** → forced sale at low multiple OR shutdown

---

## Strategic Connections
- ראה `lean-canvas.md` ל-summary של מודל אחד-עמוד
- ראה `positioning.md` (upcoming) ל-pricing positioning logic מפורט
- ראה `go-to-market.md` (upcoming) ל-channel CAC details
- ראה `../05-financial/projections.md` (Phase 7) ל-detailed financial scenarios
- ראה `../01-discovery/raw/pricing-deep-dive.md` ל-pricing landscape מלא
- ראה `../01-discovery/raw/market-size.md` ל-TAM/SAM/SOM math מקור
- ראה `../01-discovery/raw/channels.md` ל-channel-by-channel CAC modeling
- ראה `../01-discovery/market-analysis.md` ל-Phase 3 synthesis (market + regulation + timing)

---

## Sources

### Tier 1 (primary, recent, methodologically strong)
- RevenueCat State of Subscription Apps 2025 + 2026 (115K+ apps, $16B+ revenue base)
- Adapty State of In-App Subscriptions 2025 + Free Trial Conversion Rates 2026
- Apple Developer official (App Store Connect pricing reference, Small Business Program)
- Google Play official (Play Console help, 15% tier policy, October 2025 pricing template changes)
- CDC NCHS MMWR Sept 2024; CDC Data Brief #543 (Dec 2025) — adult ADHD prevalence
- AppTweak 2026 — iOS CPI productivity NA $2.84 (+90% YoY)
- Business of Apps — CPI, retention, trial benchmarks
- Recurly subscription benchmarks (67M subscribers) — trial-to-paid YoY decline
- Apple App Store Awards 2025 — Tiimo iPhone App of the Year

### Tier 2 (specialized industry, useful)
- First Page Sage / ChartMogul — trial conversion studies (opt-in 18-25%, opt-out 49-60%)
- BusinessDojo, Mapendo — CPI and ARPU analyses (NA ARPU $6.20/mo)
- ChoosingTherapy 2025 Inflow review (pricing + billing reputation)
- 42matters — Israel app market statistics
- HCPLive, Wallace PhD — mental health app retention (3.3% D30)
- Amraandelma 2025 — productivity D30 4.1%
- InfluenceFlow / Influencer Marketing Hub — TikTok micro-creator rates
- AdResults / Adopter / Castos — podcast CPM benchmarks

### Tier 3 (anecdotal, used with skepticism)
- Trustpilot Inflow reviews (selection bias on negative)
- Pissedconsumer Fabulous reviews (category-wide ADHD billing complaints)
- SubJolt, Focus Digital — churn benchmarks (proxy)

---

## Flags

### Red Flags
1. **Apple WWDC June 8, 2026 (in 11 days)** — Mayday Labs acquisition + Gemini Spark precedent → high probability of "good enough" AI scheduling announcement in iOS 27 / Siri. **Directly threatens entire model if Planny is positioned horizontally.** Mitigation: vertical/ADHD-specific positioning from day 1.
2. **Retention D30 unknown for ADHD audience** — model breaks if <5%. Productivity category default is 4.1%; mental-health is 3.3%. **Retention design must ship in v1, not be deferred.**
3. **Apple Small Business Program eligibility may not be granted immediately** — if SBP denied, year 1 gross margin compresses from 95% to 94% (manageable), but net revenue per user drops 21% (material to reinvestment compounding speed).
4. **Trial-to-paid conversion declining industry-wide** (46% → 33% YoY per Recurly) — subscription fatigue is real; no-free-tier raises stakes on every paywall decision.
5. **Inflow's $11M ad spend has poisoned Meta/TikTok auctions** for ADHD-niche targeting — paid CAC > $30 unsustainable; organic-only acquisition is mandatory, not optional.
6. **WA MHMDA private right of action + ad pixel exposure** (BetterHelp/Cerebral/GoodRx fact pattern) — single enforcement action ($1-7M settlements) is business-ending for bootstrap. **No Meta/TikTok/Google pixels on any ADHD-related page.**

### Yellow Flags
1. **Founder no-salary policy works only if family/personal runway allows.** If runway exhausted before month 6, model collapses regardless of MRR.
2. **Israel TAM ceiling caps total addressable** at ~$50-140K ARR — strategic anchor, not revenue engine. Don't build projections that depend on IL revenue.
3. **Reinvestment math assumes compounding** — first 90 days are existential. If first 50-100 paying users don't materialize by month 3, runway tightens fast.
4. **Cash flow lag** — Apple/Google hold 30-45 days; refund window 30 days → 60-day working capital gap from subscription start to "safe" revenue.
5. **6-month tier may cannibalize annual** if persuasion math fails — monitor tier mix monthly; if 6mo >40% of mix, re-tune paywall to make annual more obvious.
6. **Tiimo iPhone App of the Year halo effect** — 12 months of marketing oxygen for direct competitor. Planny's wedge (weekly cadence + late-dx women + conversational re-plan) must be visibly distinct.
7. **California Auto-Renewal Law (SB 313, July 2025)** — single retention offer max, click-to-cancel required. Recommended flow already compliant, but legal review pre-launch needed (also NY, Colorado, FTC click-to-cancel rule).
8. **Refund rate sensitivity** — every 1% increase in refund rate erodes net LTV. Sessions-gated refund (<10 sessions) protects against gaming but adds support load.
9. **Founder runway personal exposure** — bootstrap = personal financial risk; the model has no buffer for medical emergency / family crisis / Israeli reservist call-up (founder-Israeli risk per market-analysis.md).
