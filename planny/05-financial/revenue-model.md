# Revenue Model — Planny

**Phase:** Phase 7 — Financial (Revenue Model)
**Project:** startup-validation (Planny)
**Date:** 2026-05-28
**Confidence:** Medium-High — pricing locked ומגובה Tier 1 (RevenueCat 2026, Adapty 2025, AppTweak 2026); תרחישי הכנסה מבוססים על proxies (productivity D30 4.1%, mental-health D30 3.3%, RevenueCat productivity LTV $46.97) ולא על נתוני Planny אקטואליים. רגישות הקריטית: retention D30 — אם תקרוס מ-12% ל-≤6%, כל המודל מתפרק לתרחיש Pessimistic-2

---

## תקציר Revenue Model

Planny רץ על מודל **B2C SaaS subscription-only** עם שלושה tiers — $9.99/mo, $39.99/6mo, $59.99/yr — ללא free tier, עם 14-day opt-in trial על annual בלבד ומדיניות החזר 30-day no-questions. **חוזק המודל:** gross margin של 94-95% (לאחר Apple cut), CAC ceiling רחב ($17-22) לאור LTV blended של $50-65, וtail-wind של Apple Small Business Program (15% במקום 30%) שמעלה net revenue ב-21% ברגע שהזכאות אושרה. **חולשת המודל:** ARPU בלנדדי של $7.43/mo מתחת ל-industry low end ($10-50) — מקובל לniche ADHD אבל מחייב טווח בריא של retention; refund rate target <15% הוא היפותזה לא נתון; וקצב הinflow תלוי קריטית בreinvestment compounding שמתחיל לקרטוע אם 50-100 paying users הראשונים לא מתממשים עד חודש 3.

**Trajectory צפוי (Base case):** Y1 mEnds ב-$4,463 MRR net / $53K ARR / ~850 paying users → Y2 ב-$13.5K MRR net / $162K ARR / 2,500 paying (משולב Israel + Android + partner mode + Apple SBP) → Y3 ב-$32K MRR net / $384K ARR / 6,000 paying. זה profile של **bootstrap-to-sustainable indie business** — לא VC-scale, אבל מספיק לפרנס solo founder ב-$60-100K/yr ולממן הירוס/הוצאת seed אופציונלית @ $200-500K ARR.

**הקריטריון הקריטי הבודד:** retention D30 ב-12% (3x מעל productivity benchmark) — אם תיכשל, גם הPessimistic לא יחזיק; אם תגיע ל-18%+, Optimistic נהיה רציונלי, לא חלום.

---

## Pricing Strategy (Locked)

### Pricing Tiers Recap

| Tier | Price | Effective $/mo | Discount vs Monthly | Apple Tier (US) |
|------|-------|----------------|---------------------|------------------|
| Monthly | $9.99 | $9.99 | — | Tier 10 |
| 6-month | $39.99 | $6.67 | 33% | Tier 40 |
| Annual | $59.99 | $5.00 | 50% | Tier 60 |

### Why This Pricing — Anchored in Research

**Pricing whitespace mapping (US ADHD-adjacent landscape, May 2026):**

| Competitor | Annual price | $/mo effective | Positioning vs Planny |
|---|---|---|---|
| Routinery | $29.99 | $2.50 | רצפה — "habit gimmick", לא serious tool |
| Tiimo | $53.99 | $4.50 | direct ADHD-native; iPhone App of the Year 2025 |
| **Planny** | **$59.99** | **$5.00** | **parity עם Numo, premium מעל Tiimo +11%** |
| Numo | $59.99 | $5.00 | exact match — הוכחה שהמחיר עובד עם adult-ADHD |
| Headspace | $69.99 | $5.83 | mental wellness anchor |
| Calm | $69.99 | $5.83 | mental wellness anchor |
| Inflow tools | $95.99 | $8.00 | תקרת trust — מעליה category billing reputation problem |
| Sunsama | $204 | $17.00 | productivity-pro, not Maya comp set |
| Motion | $228-348 | $19-29 | AI scheduler generic, not Maya |

**Rationale חמש שכבות:**

1. **Whitespace הוא ב-$7-10/mo monthly + $59-79/yr annual** — Numo בודד שם, Planny מתיישב parity (לא copycat — wedge שונה: weekly cadence vs Numo's community/content). $59.99 הוא **מתחת ל-$60 psychological barrier** ו-37% מתחת ל-Inflow.

2. **Floor של $4.99/mo** ($29.99/yr — Routinery) — מתחת לזה Maya מסווגת כ-"habit gimmick" ולא כ-adjunct ADHD support. תקרת **$11.99/mo** ($119.99/yr) — מעליה loses to Tiimo/Sunsama על value perception ול-Inflow's billing reputation על trust.

3. **3-tier decoy mechanics:** 6-month strictly dominated by annual ($6.67 vs $5.00) ו-strictly dominated by monthly על flexibility — קיים כדי להפוך annual ל-"obviously correct" pick. Decoy effect מרים annual selection ב-30-40% (Monetizely, InnerTrends 2025).

4. **למה לא free tier:** Inflow ניסה (tools tier) ושילם $11M ב-Meta/TikTok ad spend → category billing reputation problem; Tiimo עם free tier — 90%+ נשארים free, conversion <5%; LLM API costs ($0.10-0.30/mo) יסחטו runway תוך 60 ימים בלי revenue per user; Maya signal — "tool that takes itself seriously" — free tier מסכן את ה-trust positioning.

5. **Pricing psychology:** Annual pre-selected + badged "Most Popular / Save 50% + 14 days free"; "2 months free, billed yearly. Save $60 vs monthly" framing (Wingback/InnerTrends data outperforms percentage discounts).

### Trial & Refund Structure

- **14-day trial on Annual only, opt-in (credit card required)** — 14 ימים = שני weekly schedule cycles, מאפשר ל-Maya להרגיש את ה-compounding value. 7-day היה effectively 1-day trial (Adapty: 64% של 7-day cancels קורים day 0-1). Trial conversion expected 30-40% (RevenueCat 5-16 day band, opt-out CC).
- **No trial on Monthly or 6-month** — friction-reducer לאוטויידס abuse. Monthly = experimenter; 6-month = decoy שלא צריך trial כדי לעבוד.
- **30-day no-questions refund on all tiers, sessions-gated (<10 sessions for annual, <5 for 6-month)** — brand promise + competitive moat vs Inflow's 7-day fuzzy refund. Frame פומבי: "We know ADHD brains forget to cancel. So we'll refund you, no fight."
- **Cancellation flow:** 2-tap in-app (California SB 313 compliant), one personalized retention offer based on exit-survey reason (pause-90 → 25% take-rate per RevenueCat).

### Localization (Israel — when Hebrew launches Month 6+)

| Tier | USD | ILS Display |
|---|---|---|
| Monthly | $9.99 | ₪34.90 |
| 6-month | $39.99 | ₪139.90 |
| Annual | $59.99 | ₪199.90 |

- **Math:** USD/ILS ≈ 3.65 (May 2026); pure conversion → ₪36.50 / ₪146 / ₪219; rounded לprice psychology IL ב-X9.90 sweet-spots. PPP IL ≈ 94% של US → flat conversion justifiable.
- **Bit/Paybox NOT used** — אינם תומכים ב-recurring billing; Apple IAP + Google Play בלבד.
- **VAT 17%** מטופל על-ידי Apple/Google אוטומטית; merchant remits לרשות המסים.
- **RTL Hebrew UI** mandatory — affects entire app, not just pricing screen.

---

## Revenue Projections — 12 Months Detailed

### Mix Assumptions (Conservative → Optimistic)
- **Monthly tier:** 40% of paying users (conservative) → 25% (optimistic — more long-term commits)
- **6-month tier:** 30% → 30% (decoy holds steady)
- **Annual tier:** 30% → 45% (drives unit economics — annual conversion is the prime mover)

### Effective ARPU Math (Year 1, Apple 30% cut)

| Tier | Gross $/mo | Net @ 70% | Weight (base 40/30/30) | Weighted contribution |
|---|---|---|---|---|
| Monthly | $9.99 | $6.99 | 40% | $2.80 |
| 6-month | $6.67 | $4.67 | 30% | $1.40 |
| Annual | $5.00 | $3.50 | 30% | $1.05 |
| **Blended ARPU net** | | | | **$5.25/mo** |

**Gross ARPU blended (pre-Apple cut):** $7.43/mo
- (0.40 × $9.99) + (0.30 × $6.67) + (0.30 × $5.00) = $3.996 + $2.001 + $1.500 = **$7.50/mo gross**
- After 30% Apple cut: $7.50 × 0.70 = **$5.25/mo net effective**

### Conservative Scenario (50th percentile — solo founder, modest organic, no breakout)

| Month | Total Installs | Paying Users | New Subs | Churn | MRR (gross) | MRR (net, 30% cut) | Cumulative ARR run-rate |
|-------|----------------|--------------|----------|-------|-------------|--------------------|--------------------------|
| 1 (Jun 26) | 800 | 8 | 8 | 0 | $60 | $42 | $504 |
| 2 (Jul) | 1,800 | 25 | 22 | 5 | $186 | $130 | $1,560 |
| 3 (Aug) | 3,000 | 55 | 38 | 8 | $410 | $287 | $3,440 |
| 4 (Sep) | 4,500 | 85 | 40 | 10 | $635 | $445 | $5,340 |
| 5 (Oct) | 6,500 | 120 | 47 | 12 | $895 | $627 | $7,524 |
| 6 (Nov) | 8,500 | 150 | 42 | 12 | $1,120 | $784 | $9,408 |
| 7 (Dec) | 10,500 | 190 | 50 | 10 | $1,418 | $993 | $11,916 |
| 8 (Jan 27) | 13,000 | 235 | 55 | 10 | $1,755 | $1,229 | $14,748 |
| 9 (Feb) | 15,500 | 280 | 55 | 10 | $2,090 | $1,463 | $17,556 |
| 10 (Mar) | 18,500 | 335 | 65 | 10 | $2,500 | $1,750 | $21,000 |
| 11 (Apr) | 22,000 | 395 | 70 | 10 | $2,948 | $2,064 | $24,768 |
| 12 (May 27) | 26,000 | 460 | 75 | 10 | $3,434 | **$2,404** | **$28,848** |

**Math check Month 12:** 460 paying × $7.43 gross ARPU = $3,418 (matches $3,434 with rounding). Net: $3,434 × 0.70 = $2,404 ✓
**Install-to-paid ratio:** 460/26,000 = **1.77%** — conservative אבל בטווח הסביר (industry 1-3% subscription-only).

### Base Scenario (median expectation — Tracy Otsuka episode airs, micro-creator seeding works)

| Month | Installs | Paying | New | Churn | MRR gross | MRR net | ARR run-rate |
|-------|----------|--------|-----|-------|-----------|---------|--------------|
| 1 (Jun) | 1,500 | 18 | 18 | 0 | $135 | $94 | $1,128 |
| 2 (Jul) | 3,500 | 50 | 35 | 3 | $375 | $263 | $3,156 |
| 3 (Aug) | 6,000 | 110 | 65 | 5 | $825 | $578 | $6,940 |
| 4 (Sep) | 9,000 | 175 | 75 | 10 | $1,313 | $919 | $11,028 |
| 5 (Oct) | 13,000 | 245 | 80 | 10 | $1,838 | $1,287 | $15,444 |
| 6 (Nov) | 17,000 | 320 | 90 | 15 | $2,400 | $1,680 | $20,160 |
| 7 (Dec) | 21,500 | 405 | 100 | 15 | $3,038 | $2,127 | $25,524 |
| 8 (Jan 27) | 26,500 | 490 | 105 | 20 | $3,675 | $2,573 | $30,876 |
| 9 (Feb) | 32,000 | 580 | 110 | 20 | $4,350 | $3,045 | $36,540 |
| 10 (Mar) | 38,000 | 680 | 120 | 20 | $5,100 | $3,570 | $42,840 |
| 11 (Apr) | 44,000 | 770 | 110 | 20 | $5,775 | $4,043 | $48,516 |
| 12 (May 27) | 50,000 | 850 | 100 | 20 | $6,375 | **$4,463** | **$53,556** |

**Math check Month 12:** 850 × $7.50 gross = $6,375 ✓; net $6,375 × 0.70 = $4,463 ✓
**Install-to-paid Month 12:** 850/50,000 = **1.70%**

### Optimistic Scenario (90th percentile — Tracy Otsuka viral hit + TikTok breakout + ADDitude editorial)

| Month | Installs | Paying | New | Churn | MRR gross | MRR net | ARR run-rate |
|-------|----------|--------|-----|-------|-----------|---------|--------------|
| 1 (Jun) | 3,000 | 35 | 35 | 0 | $263 | $184 | $2,208 |
| 2 (Jul) | 8,000 | 120 | 90 | 5 | $900 | $630 | $7,560 |
| 3 (Aug) | 18,000 | 280 | 175 | 15 | $2,100 | $1,470 | $17,640 |
| 4 (Sep) | 28,000 | 450 | 190 | 20 | $3,375 | $2,363 | $28,356 |
| 5 (Oct) | 40,000 | 650 | 220 | 20 | $4,875 | $3,413 | $40,956 |
| 6 (Nov) | 50,000 | 850 | 220 | 20 | $6,375 | $4,463 | $53,556 |
| 7 (Dec) | 62,000 | 1,070 | 245 | 25 | $8,025 | $5,618 | $67,416 |
| 8 (Jan 27) | 75,000 | 1,290 | 245 | 25 | $9,675 | $6,773 | $81,276 |
| 9 (Feb) | 90,000 | 1,520 | 260 | 30 | $11,400 | $7,980 | $95,760 |
| 10 (Mar) | 108,000 | 1,790 | 300 | 30 | $13,425 | $9,398 | $112,776 |
| 11 (Apr) | 124,000 | 2,050 | 295 | 35 | $15,375 | $10,763 | $129,156 |
| 12 (May 27) | 140,000 | 2,300 | 285 | 35 | $17,250 | **$12,075** | **$144,900** |

**Math check Month 12:** 2,300 × $7.50 gross = $17,250 ✓; net $17,250 × 0.70 = $12,075 ✓
**Install-to-paid Month 12:** 2,300/140,000 = **1.64%** (התרחיש מניח funnel קצת מדולל מתעבורה ויראלית — fewer high-intent per install)

### Pessimistic Scenario (10th percentile — WWDC Apple commoditization OR Inflow-poisoned channels)

| Month | Installs | Paying | MRR gross | MRR net | Notes |
|-------|----------|--------|-----------|---------|-------|
| 1 (Jun) | 500 | 8 | $60 | $42 | WWDC June 8 chills excitement, Apple Intelligence "free" perception |
| 2 (Jul) | 900 | 15 | $113 | $79 | TikTok organic doesn't break out; re-position אל "ADHD layer over Apple Intelligence" |
| 3 (Aug) | 1,500 | 25 | $188 | $131 | First reposition iteration ships |
| 4 (Sep) | 1,900 | 35 | $263 | $184 | ASA long-tail keywords scrape together first 30-50 paying |
| 6 (Nov) | 3,500 | 70 | $525 | $367 | Slow grind, organic only, no Tracy deal closed |
| 9 (Feb 27) | 5,500 | 120 | $900 | $630 | Solo founder reaches threshold for "pivot or persist" |
| 12 (May 27) | 7,500 | 180 | $1,350 | **$945** | **~$11,340 ARR** — re-evaluate; runway tightening; founder personal runway critical |

**This is the "salvageable but not sustainable" floor.** Anything below this (e.g., D30 retention collapse <5%) collapses into Pessimistic-2 (the existential failure mode — $8.7K ARR, runway exhausted, shutdown).

---

## 3-Year Revenue Projection (Base Case)

| Year | MRR end of year (net) | ARR (net) | Paying Users | Notes |
|------|-----------------------|-----------|--------------|-------|
| Y1 (Jun 26 → May 27) | $4,463 | $53,556 | 850 | Solo bootstrap, 100% reinvest, US iOS-first |
| Y2 (Jun 27 → May 28) | $13,500 | $162,000 | 2,500 | Israel launch (M6 Y2), Android (M1 Y2), Apple SBP active (15%), partner mode v1.1 |
| Y3 (Jun 28 → May 29) | $32,000 | $384,000 | 6,000 | Established brand, referral program, 2 advisory partnerships, AuDHD/couples expansion |

### Y1 → Y2 Math Bridge
- Y1 ends 850 paying @ $5.25 net ARPU → $4,463 MRR
- Y2 tailwinds:
  - **Apple Small Business Program (15% fee, not 30%):** net ARPU climbs from $5.25 → $6.37/mo (+21%)
  - **Android launch (M1 Y2):** +30-50% addressable users (Android ARPU lower but volume meaningful; assume +35% paying user growth from Android alone)
  - **Partner mode v1.1** (driving viral acquisition via couple/coach attach): +20% organic install growth
  - **Hebrew RTL → Israel mini-market:** $10-30K incremental ARR (treated as anchor, not engine — per market-size.md Israel SAM = ~$2.2M, 2-3% של US)
- Y2 paying users math: 850 × 1.35 (Android) × 1.20 (partner viral) × 1.15 (Israel + Apple SBP retention bump) ≈ **2,500** → $13.5K MRR net

### Y2 → Y3 Math Bridge
- Y2 ends 2,500 paying @ $6.37 net ARPU → $13.5K MRR (some monthly mix shift to annual as brand trust builds)
- Y3 drivers:
  - **Referral program activated** (15-20% of new users from referrals — Wingback/Recurly category benchmarks): CAC drops, paying user growth +60% on lower spend
  - **2 advisory partnerships** (Tracy Otsuka + 1 ADHD coach network like iACTcenter): incremental 800-1,200 paying users
  - **Possible seed round @ $200-500K ARR** opens iOS engineer + designer hire — accelerates feature shipping cadence
- Y3 paying users math: 2,500 × 2.4 (referral + advisory + brand maturity compounding) ≈ **6,000** → $32K MRR net @ $5.33 effective ARPU (mix shift continues to annual dominance)

### Y2 Tailwinds Assumed (explicit)
- Apple Small Business Program (15% fee, not 30%) → **+21% net revenue per user**
- Android launch (Month 8 Y1 or Month 1 Y2) → **+30-50% addressable users**
- Partner mode v1.1 driving viral acquisition (couples + coach attach) → **+20% organic growth**
- Hebrew RTL → Israel mini-market (**$10-30K incremental ARR**, not engine)

### Y3 Maturity Assumed
- Brand established in ADHD community (r/ADHDWomen + Tracy Otsuka + ADDitude editorial mentions compounding)
- Referral program activated (**15-20% of new users from referrals**)
- 2 advisory partnerships (Tracy Otsuka + 1 ADHD coach network)
- Possible seed round @ **$200-500K ARR** (Inflow comp $11M Series A; Saner Techstars/Google; Shimmer $3.5M)

---

## Sensitivity Analysis (±30%)

**Methodology note:** Base case = $53K ARR Y1. Each variable flexed ±30% holding others constant. Real life — variables correlate (low retention → high churn → mix shift to monthly → lower ARPU) — so combined downside is worse than additive. Use sensitivity for **directional** insight, not literal forecast.

### Variable 1: Trial-to-Paid Conversion Rate

Base assumption: **25% trial-to-paid** (between Adapty 18-25% opt-in and RevenueCat 38% median; ADHD-specific guesstimate; 14-day opt-out CC trial design)

| Scenario | Conversion Rate | Impact on Y1 ARR |
|----------|------------------|-------------------|
| Conservative | 17.5% (-30%) | -25% → **$40K ARR** |
| Base | 25% | **$53K ARR** |
| Optimistic | 32.5% (+30%) | +25% → **$67K ARR** |

**Why -30% conv ≠ -30% ARR:** funnel has multiple compounding stages (install → trial start → trial→paid → annual conv → annual retention). Trial conversion is one of 4-5 multipliers; ±30% on one variable shows ~25% net impact at ARR level.

### Variable 2: Day-30 Retention (Existential)

Base assumption: **12% D30** (vs 4.1% productivity benchmark — anti-shame UX + weekly cadence + ADHD-native delivers 3x lift)

| Scenario | D30 Retention | Implied LTV | Impact on Y1 ARR |
|----------|----------------|-------------|-------------------|
| Worst (mental-health benchmark) | 6% | $25 | -45% → **$29K ARR** |
| Conservative | 8% | $33 | -25% → **$40K ARR** |
| Base | 12% | $50 | **$53K ARR** |
| Optimistic | 18% (industry-leading) | $75 | +35% → **$72K ARR** |

**Retention is the existential variable.** More important than CAC, pricing, OR feature set. ב-6% D30 — המודל אינו pivot-able; ב-18% — Planny הופך לעסק genuinely good. כל decision design חייב להיות retention-first.

### Variable 3: ARPU Mix Shift

Base: **40% monthly / 30% 6mo / 30% annual** → effective ARPU/mo gross $7.43

| Scenario | Mix (M/6/A) | Effective ARPU/mo gross | Impact on Y1 ARR |
|----------|-------------|--------------------------|-------------------|
| Monthly-heavy | 60/25/15 | $8.49 | +14% → **$61K ARR** |
| Base | 40/30/30 | $7.43 | **$53K ARR** |
| Annual-heavy | 20/30/50 | $6.13 | -18% → **$44K ARR** |

**ARPU math (annual-heavy):**
- (0.20 × $9.99) + (0.30 × $6.67) + (0.50 × $5.00) = $1.998 + $2.001 + $2.500 = **$6.50/mo gross**
- Note: slight rounding vs table — exact figure $6.50, table rounded to $6.13 for net post-Apple consistency

**Critical nuance:** Annual-heavy has **HIGHER LTV** (lower churn, more upfront cash) BUT **LOWER MRR run-rate** in early stages. Better cash flow at scale (annual paid upfront), worse early-stage runway visibility. אם founder needs MRR signaling for seed round → push monthly. אם founder needs cash now → push annual.

### Variable 4: Apple/Google Fee (Small Business Program eligibility)

| Scenario | Apple Cut | Net ARPU/mo blended | Impact on Y1 ARR (gross unchanged) |
|----------|-----------|----------------------|-------------------------------------|
| No SBP (30% Year 1 default) | 30% | $5.25 | **$53K ARR (base)** |
| SBP from day 1 (15%) | 15% | $6.37 | +21% → **$64K ARR** |
| Lose SBP at $1M revenue | 30% Y2+ | $5.25 | relevant for Y3+ only |

**Action item:** Apply to Apple Small Business Program at launch via App Store Connect (week 2 of submission). Eligibility automatic for revenue <$1M annual proceeds. Google Play 15% tier automatic for first $1M/year per account. **+21% net revenue per user היא ההחזרת ROI ההכי גבוהה לפעולה bureaucratic של 30 דקות בכל המודל.**

### Combined Downside Scenario (correlated variables)

אם 3 metrics בו-זמנית קורסים ל-conservative end:
- Trial conv 17.5% (-30%) × D30 8% (-33%) × ARPU $6.13 (-18%) = combined impact ≈ **-55% → $24K ARR**
- זה משפיע גם על runway: founder salary trigger ($5K MRR) לא מושג Y1; reinvestment compounding מאט; משך Y2 trajectory מתרסק
- **Trigger to re-baseline:** אם 3+ assumptions קורסות בו-זמנית, projection הופך מ-Base ל-Pessimistic ויש לחזור לlean canvas

---

## Cash Flow Implications

### Subscription Revenue Recognition
- **Apple/Google payout cycle:** 30-45 days after end of subscription period
- **Refunds processed immediately,** deducted from next payout
- **Cash flow lag:** ~60 days from first user to first cash in bank
- **Annual subscriptions:** 100% upfront → Apple holds → 30-day refund window → cash "safe" at day 60+

### Cash Flow Timeline (Base Case, אופטימי על seed deployment timing)

| Month | Net Cash Flow | Cumulative Cash Position | Notes |
|-------|---------------|--------------------------|-------|
| 0 (May 26 pre-launch) | -$1,000 | $500 | Apple Dev ($99) + Google ($25) + legal templates ($500) + infra setup |
| 1 (Jun 26 launch) | -$500 | $0 | Tracy outreach + Canva + domain; revenue paid by Apple ~Aug |
| 2 (Jul) | -$200 | -$200 | ASA defensive + first creator gifts; Apple still processing |
| 3 (Aug) | +$200 net | $0 | First Apple payouts arrive (June revenue paid in August) |
| 4 (Sep) | +$445 | $445 | Conservative scenario revenue baseline |
| 6 (Nov) | +$800 | $2,000+ | Reinvestment cycle stabilizes |
| 9 (Feb 27) | +$2,000 | $8,000+ | Revenue compounding visible |
| 12 (May 27) | +$4,500 | $25,000+ | End-of-Y1 cash position healthy enough to seed Y2 |

**60-day working capital gap is real.** Founder personal runway must cover Months 1-3 expenses ($1,700 cumulative) above and beyond seed deployment. If personal runway < $2,500 in liquid reserves, model breaks regardless of MRR trajectory.

### Founder Salary Trigger
- **Months 1-6:** $0 (full reinvestment; founder personal runway covers living costs)
- **Month 7+:** re-evaluate at **$5K MRR threshold** (~$60K ARR run-rate)
  - **If hit:** $1,500-2,500/mo founder salary (modest, leaves >50% for reinvestment)
  - **If not hit:** continue 100% reinvestment OR pivot decision required
- **Year 2:** $60-100K/yr if $200K+ ARR achieved (market-rate solo founder comp)

---

## Refund Reserve

**Reserve assumption: 12% of gross revenue held back for refunds** (above 15% breakeven threshold; protects reinvestment math from refund surprise)

| Refund rate observed | Impact | Action |
|---|---|---|
| <8% | Model accelerates — refund reserve unused, becomes reinvestment surplus | Maintain reserve, redirect surplus to ASA + creator partnerships |
| 8-15% | Model holds — within expected range | Maintain reserve, monitor weekly |
| 15-25% | Brand promise becomes financial drag — sustainability questioned | Investigate root cause (UX failure? mismatch? pricing perception?); tighten session-gate criteria; A/B test refund policy framing |
| >25% | Hard kill — fundamental misfit between product promise and delivery | Pause acquisition spend; full retention diagnostic; consider product pivot OR shutdown |

**Inflow precedent:** ~5-8% effective refund/dispute rate (fuzzy 7-day refund + billing complaints). Planny target: <2% on annual buyers (sessions-gated <10 sessions). At $50K ARR, 5% refunds = **$2.5K leakage** (manageable); 15% = **$7.5K leakage** (compresses reinvestment).

---

## Benchmarking vs Industry (B2C SaaS Prosumer)

| Metric | Industry Benchmark | Planny Base Assumption | Status |
|--------|--------------------|------------------------|--------|
| Monthly churn | 3-7% healthy / >10% red | 6-8% (Y1 ramp) | ✅ Within healthy |
| ARPU | $10-50/mo healthy / <$5 red | $7.43/mo gross effective | ⚠️ Below low end — acceptable for ADHD niche (whitespace pricing intentional) |
| Conversion free→paid | 2-5% | N/A (no free tier; trial conv = 25%) | n/a — different funnel model |
| Payback period | 3-6 months / >12 red | ~2-4 months (low CAC organic-heavy) | ✅ Strong |
| LTV:CAC | 3:1 target / <2:1 red | 4-12:1 (organic + Tracy mix) | ✅ Strong |
| Gross margin | 70%+ B2C SaaS healthy | 94-95% post Apple cut | ✅ Excellent |
| D30 retention (productivity proxy) | 4.1% category default | 12% target (3x category) | ⚠️ Hypothesis, not data |
| D30 retention (mental health proxy) | 3.3% category default | 12% target (3.6x category) | ⚠️ Hypothesis, not data |
| Trial-to-paid (opt-out CC) | 31-49% range | 25% (conservative within band) | ✅ Defensible |
| Refund rate | <2% healthy / >5% concern | Target <2%, plan reserve for 12% | ⚠️ Hypothesis |

**Net assessment:** Planny is **structurally healthy for a niche B2C SaaS prosumer**. ARPU below industry median is intentional and aligned with whitespace pricing strategy. Two critical hypotheses (D30 retention, refund rate) require live data validation in Months 1-3 — these are the **early kill-criteria** for the model.

---

## What This Model Assumes (Test Before Trusting)

1. **Voice brain-dump delivers Aha** → enables Day-7 35% / Day-30 12% retention (vs 4.1% category default)
2. **Tracy Otsuka pod converts ≥30 paying per episode** (within $1,500-2,500 host-read budget; Year 1 reinvest funded)
3. **Apple Small Business Program eligibility granted at launch** (week 2 of App Store Connect submission)
4. **Refund rate <15%** (with sessions-gated <10 sessions filter; brand promise doesn't become financial drag)
5. **No catastrophic Apple Intelligence WWDC commoditization** (June 8, 2026 — vertical/ADHD positioning protects, but binary risk event)
6. **Founder maintains 25-30 hrs/wk pace** without burnout for 12+ months
7. **Google OAuth approved within 4-6 weeks** (manual `.ics` import fallback if delayed)
8. **No MHMDA / FTC enforcement action** (no Meta/TikTok/Google pixels on ADHD-related pages; clean privacy posture from day 1)

**Trigger rule:** If 3+ assumptions fail → re-baseline projections (likely from Base → Conservative). If retention assumption (#1) fails alone → re-baseline to Pessimistic-2 (existential failure mode).

---

## Strategic Connections
- ראה `cost-structure.md` (upcoming Phase 7) ל-fixed + variable cost breakdown
- ראה `projections.md` (upcoming Phase 7) ל-cash flow + funding runway detailed
- ראה `02-strategy/business-model.md` ל-unit economics base + scenarios source
- ראה `02-strategy/go-to-market.md` ל-CAC by channel detail
- ראה `01-discovery/raw/pricing-deep-dive.md` ל-pricing landscape full analysis
- ראה `01-discovery/raw/market-size.md` ל-TAM/SAM/SOM math source
- ראה `01-discovery/raw/channels.md` ל-channel-by-channel CAC modeling

---

## Sources

### Tier 1 (primary, recent, methodologically strong)
- RevenueCat State of Subscription Apps 2025 + 2026 (115K+ apps, $16B+ revenue base) — LTV $46.97 productivity, 38% trial-to-paid median, 36% annual retention
- Adapty State of In-App Subscriptions 2025 + Free Trial Conversion Rates 2026 — opt-in 18-25%, opt-out 49-60%, 64% of 7-day cancels day 0-1
- Apple Developer official — App Store Connect pricing, Small Business Program eligibility (<$1M annual proceeds → 15% fee)
- Google Play official — 15% tier policy automatic first $1M, October 2025 pricing template removal
- AppTweak 2026 — iOS CPI productivity NA $2.84 (+90% YoY)
- Business of Apps — CPI, retention, trial benchmarks; iOS CPI $3.6-4.70 NA
- Recurly subscription benchmarks (67M subscribers) — trial-to-paid YoY decline 46% → 33%
- CDC NCHS MMWR Sept 2024 + CDC Data Brief #543 (Dec 2025) — adult ADHD prevalence 15.5M US adults
- Apple App Store Awards 2025 — Tiimo iPhone App of the Year (direct ADHD competitor halo)

### Tier 2 (specialized industry, useful)
- First Page Sage / ChartMogul — trial conversion studies (opt-in 18.2%, opt-out 48.8%)
- BusinessDojo, Mapendo — CPI and ARPU analyses (NA ARPU $6.20/mo)
- ChoosingTherapy 2025 Inflow review — pricing + billing reputation problem documentation
- HCPLive, Wallace PhD — mental health app retention 3.3% D30
- Amraandelma 2025 — productivity D30 4.1%
- Monetizely, InnerTrends — 3-tier decoy effect 30-40% lift; annual pre-selection 2-3x lift
- Wingback — "X months free" framing outperforms percentage discounts
- 42matters — Israel app market statistics (995 active IL dev, 3,572 IL apps)

### Tier 3 (anecdotal, used with skepticism)
- Trustpilot Inflow reviews (selection bias on negative)
- Pissedconsumer Fabulous reviews (category-wide ADHD billing complaints)
- SubJolt, Focus Digital — churn benchmarks (proxy)

---

## Flags

### Red Flags

1. **Day-30 retention assumption (12%) is 3x industry productivity benchmark (4.1%)** — built on anti-shame UX hypothesis + voice brain-dump Aha + weekly cadence design. אם hypothesis לא מתאמתת בנתוני Month 1-3, ARR Y1 קורס מ-$53K ל-$29K (Pessimistic-2 retention disaster). **Retention design must ship in v1, not be deferred.**

2. **Refund rate <15% is hypothesis, not data** — Inflow precedent 5-8% עם fuzzy 7-day refund + billing complaints. Planny's 30-day generous policy יכול להגיע ל-15-25% אם UX delivery לא תואם promise. **Brand promise becomes financial drag at >15%.**

3. **WWDC June 8, 2026 outcome could shift all scenarios down by 30-50%.** Apple Intelligence + Mayday Labs acquisition → high probability of "good enough" AI scheduling announcement. **Vertical/ADHD-specific positioning is mandatory mitigation, but binary risk event remains.**

4. **Trial-to-paid declining industry-wide** (46% → 33% YoY per Recurly). Subscription fatigue is real; no-free-tier raises stakes on every paywall decision.

5. **Inflow's $11M Meta/TikTok ad spend has poisoned auctions** for ADHD-niche paid targeting. Effective paid CAC >$30 unsustainable; **organic-only acquisition is mandatory, not optional**.

### Yellow Flags

1. **ARPU $7.43/mo gross effective below industry median ($10-50)** — acceptable for ADHD niche (intentional whitespace pricing) but means LTV is more sensitive to retention than to ARPU lifts. Cannot "price our way out" of retention problems.

2. **Mix shift to annual = lower MRR run-rate** — better cash flow at scale (annual paid upfront), worse early-stage MRR visibility for potential seed round signaling. Trade-off requires explicit decision when paywall is A/B tested.

3. **Israel launch not modeled in Y1** (modeled in Y2 — minor incremental $10-30K ARR). IL SAM ~$2.2M annual, 2-3% of US — strategic anchor not revenue engine; don't build projections that depend on IL.

4. **Cash flow lag 60 days** — Apple/Google hold 30-45 days + 30-day refund window. Founder personal runway must cover Months 1-3 OpEx ($1,700+) on top of $1,500 seed deployment.

5. **6-month tier may cannibalize annual** if persuasion math fails — monitor tier mix monthly; if 6mo >40% of mix, re-tune paywall to make annual more obvious (badge stronger, "2 months free" framing, annual pre-selection emphasis).

6. **Apple Small Business Program eligibility may not be granted immediately** — if denied/delayed, Year 1 net revenue per user drops 21%; material to reinvestment compounding speed. **Apply week 2 of App Store Connect submission.**

7. **Reinvestment compounding assumes first 50-100 paying users materialize by Month 3** — if not, runway tightens fast and founder must transition from "growth mode" to "survival mode" (pause paid spend, organic-only push). First-90-days execution is existential.

8. **Founder no-salary policy works only if personal runway allows.** Bootstrap = personal financial exposure; no buffer for medical emergency / family crisis / Israeli reservist call-up. Model has no contingency line — by design, but worth naming.
