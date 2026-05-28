# Financial Projections — Planny

**Phase:** Phase 7 — Financial (Projections)
**Project:** startup-validation (Planny)
**Date:** 2026-05-28
**Confidence:** Overall — Medium for Y1 (pricing/CAC/cost benchmarks Tier 1); Low for Y2-Y3 given unknown D30 retention for ADHD audience and binary WWDC June 8 risk event

---

## תקציר Projections

Planny משיקה ב-22 ביוני 2026 עם תקציב seed של $1,500 ו-100% reinvestment של הכנסות ב-3-6 חודשים הראשונים. המסקנה המרכזית: **הסכנה איננה במחסור כסף תפעולי אלא בריבית ההכנסה הנדחית** — Apple/Google מחזיקים תקבולים 30-45 ימים, חלון refund נוסף 30 ימים, ולכן ה-working capital gap האמיתי הוא ~60 יום משלב התשלום עד "כסף בטוח".

ב-**Base scenario** (D30 retention 12%, trial-to-paid 25%, mix 40/30/30 חודשי/חצי/שנתי), Planny צולחת cash flow break-even חודשי בחודש 3 (אוגוסט 26), עוברת ל-cumulative break-even בחודש 5 (אוקטובר 26), ומגיעה ל-$4,463 net MRR (~$53.5K ARR run-rate) עד סוף Y1. סף founder salary של $5K MRR נחצה בחודש 8 (ינואר 27) — נקודת ההחלטה הראשונה של "האם המשפחה רוצה משכורת או reinvestment".

ב-**Conservative** (D30 8%), break-even נדחה לחודש 7, ARR Y1 ~$28K, ואין משכורת ב-Y1 כלל. ב-**Optimistic** (D30 18%, Tracy Otsuka viral), break-even בחודש 2-3, ARR Y1 ~$143K, ומשכורת כבר בחודש 5. ה-**Pessimistic** (WWDC commoditization או retention collapse) זו הסתברות 10% עם החלטת המשך/סגירה בחודש 6.

**Inflection points עיקריים:** WWDC June 8 (binary risk in 11 days), Tracy Otsuka episode drop (חודש 1-3), Apple SBP approval (חודש 1-2), $2K MRR community trigger (חודש 6 base), $5K MRR salary decision (חודש 8 base), Android launch (Y2 חודש 1), Hebrew RTL (Y2 חודש 6), $10K MRR seed-round optionality (Y2 Q1-Q2).

**שורה תחתונה:** המודל עובד מתמטית גם בתרחיש Conservative — אבל **רק אם D30 retention >8%**. מתחת לסף הזה ה-reinvestment מתכווץ במקום להתרחב, ו-Planny נכנסת לספירלת מוות תוך 6-9 חודשים. רטנציה היא משתנה ה-#1, יותר מ-CAC, יותר מ-pricing.

---

## 3 Scenarios — Year 1 Month-by-Month

### CONSERVATIVE Scenario (50th percentile — slow organic, no breakout)

**Assumptions:**
- Day-30 retention: **8%** (above productivity 4.1% benchmark, below base hypothesis 12%)
- Trial-to-paid: **18%** (opt-in CC trial baseline per RevenueCat/Adapty)
- Tier mix: **50% monthly / 25% 6mo / 25% annual** (less annual lock-in)
- Blended net revenue per paid user: $5.91/mo (Y1, 30% cut)
- LLM cost: $0.30/user/mo (no caching optimization)
- Founder salary: $0 throughout Y1

| Month | Users | Paying | MRR gross | MRR net (70%) | Costs fixed | Costs variable | Net cash | Cumulative cash |
|-------|-------|--------|-----------|---------------|-------------|----------------|----------|-----------------|
| 1 (Jun 26) | 800 | 8 | $60 | $42 | $100 | $5 | -$63 | -$1,563 |
| 2 (Jul 26) | 1,800 | 25 | $186 | $130 | $100 | $15 | +$15 | -$1,548 |
| 3 (Aug 26) | 3,000 | 55 | $410 | $287 | $120 | $30 | +$137 | -$1,411 |
| 4 (Sep 26) | 4,500 | 85 | $635 | $445 | $150 | $45 | +$250 | -$1,161 |
| 5 (Oct 26) | 6,500 | 120 | $895 | $627 | $180 | $60 | +$387 | -$774 |
| 6 (Nov 26) | 8,500 | 150 | $1,120 | $784 | $200 | $80 | +$504 | -$270 |
| 7 (Dec 26) | 10,500 | 190 | $1,418 | $993 | $300 | $100 | +$593 | **+$323** |
| 8 (Jan 27) | 13,000 | 235 | $1,755 | $1,229 | $350 | $125 | +$754 | +$1,077 |
| 9 (Feb 27) | 15,500 | 280 | $2,090 | $1,463 | $400 | $150 | +$913 | +$1,990 |
| 10 (Mar 27) | 18,500 | 335 | $2,500 | $1,750 | $450 | $180 | +$1,120 | +$3,110 |
| 11 (Apr 27) | 22,000 | 395 | $2,948 | $2,064 | $500 | $210 | +$1,354 | +$4,464 |
| 12 (May 27) | 26,000 | 460 | $3,434 | $2,404 | $550 | $250 | +$1,604 | **+$6,068** |

**Y1 Conservative Totals:**
- Gross revenue: **~$15,330** (sum of monthly gross)
- Net revenue (after 30% cut): **~$10,730**
- Total costs (fixed + variable + initial $1,500 seed): **~$4,680** ops + $1,500 seed
- **Y1 Net cash position (excl. founder salary): +$6,068**
- Cash flow break-even (monthly): **Month 2 (Jul)**
- Cumulative break-even: **Month 7 (Dec)**
- ARR run-rate end Y1: **~$28.8K**
- Founder salary: **$0 triggered** (sub-$5K MRR threshold)

---

### BASE Scenario (median expectation — Tracy Otsuka closes, micro-creator seeding works)

**Assumptions:**
- Day-30 retention: **12%** (mid-point between productivity 4.1% and best-in-class evidence-based 16%)
- Trial-to-paid: **25%** (ADHD-niche, 14-day opt-in CC trial)
- Tier mix: **40% monthly / 30% 6mo / 30% annual** (per business-model.md)
- Blended net revenue per paid user: **$5.24/mo** (Y1, per business-model.md unit economics)
- LLM cost: $0.20/user/mo (with caching at 1K+ users)
- Founder salary: $0 through Month 7, decision point Month 8

| Month | Users | Paying | MRR gross | MRR net (70%) | Costs fix | Costs var | Net cash | Cum cash |
|-------|-------|--------|-----------|---------------|-----------|-----------|----------|----------|
| 1 (Jun 26) | 1,500 | 18 | $135 | $94 | $100 | $5 | -$11 | -$1,511 |
| 2 (Jul 26) | 3,500 | 50 | $375 | $263 | $100 | $20 | +$143 | -$1,368 |
| 3 (Aug 26) | 6,000 | 110 | $825 | $578 | $120 | $40 | +$418 | -$950 |
| 4 (Sep 26) | 8,500 | 175 | $1,313 | $919 | $150 | $60 | +$709 | -$241 |
| 5 (Oct 26) | 12,000 | 250 | $1,875 | $1,313 | $180 | $85 | +$1,048 | **+$807** |
| 6 (Nov 26) | 17,000 | 320 | $2,400 | $1,680 | $200 | $110 | +$1,370 | +$2,177 |
| 7 (Dec 26) | 22,000 | 410 | $3,075 | $2,153 | $300 | $145 | +$1,708 | +$3,885 |
| 8 (Jan 27) | 27,500 | 500 | $3,750 | $2,625 | $350 | $175 | +$2,100 | +$5,985 |
| 9 (Feb 27) | 32,000 | 580 | $4,350 | $3,045 | $400 | $200 | +$2,445 | +$8,430 |
| 10 (Mar 27) | 38,000 | 670 | $5,025 | $3,518 | $450 | $230 | +$2,838 | +$11,268 |
| 11 (Apr 27) | 44,000 | 760 | $5,700 | $3,990 | $500 | $265 | +$3,225 | +$14,493 |
| 12 (May 27) | 50,000 | 850 | $6,375 | $4,463 | $550 | $300 | +$3,613 | **+$18,106** |

**Y1 Base Totals:**
- Gross revenue: **~$33,200** (sum of monthly gross)
- Net revenue (after 30% cut): **~$23,640**
- Total costs (fixed + variable + initial $1,500 seed): **~$5,535** ops + $1,500 seed
- **Y1 Net cash position (excl. founder salary): +$18,106**
- Cash flow break-even (monthly): **Month 1-2 (barely negative Month 1, positive Month 2)**
- Cumulative break-even: **Month 5 (Oct 26)**
- ARR run-rate end Y1: **~$53.5K**
- **Founder salary trigger ($5K MRR threshold, ~$3.5K net): Month 8 (Jan 27)** — discussion, not automatic deployment
- Reinvestment available cumulative Y1: **~$18-23K** (after deducting any partial salary)

---

### OPTIMISTIC Scenario (90th percentile — Tracy Otsuka viral + ADDitude editorial + TikTok breakout)

**Assumptions:**
- Day-30 retention: **18%** (above evidence-based benchmark 16%, reflects ADHD-native design + mission resonance)
- Trial-to-paid: **32%** (high-intent late-dx cohort + strong paywall)
- Tier mix: **25% monthly / 30% 6mo / 45% annual** (more annual upfront, lock-in higher)
- Blended net revenue per paid user: **$4.85/mo** (Y1, more annual = lower MRR but higher cash upfront)
- LLM cost: $0.15/user/mo (heavy caching + prompt optimization at scale)
- Founder salary triggers Month 5

| Month | Users | Paying | MRR gross | MRR net (70%) | Costs fix | Costs var | Net cash | Cum cash |
|-------|-------|--------|-----------|---------------|-----------|-----------|----------|----------|
| 1 (Jun 26) | 3,000 | 35 | $263 | $184 | $100 | $10 | +$74 | -$1,426 |
| 2 (Jul 26) | 8,000 | 120 | $900 | $630 | $120 | $35 | +$475 | -$951 |
| 3 (Aug 26) | 18,000 | 280 | $2,100 | $1,470 | $150 | $80 | +$1,240 | **+$289** |
| 4 (Sep 26) | 30,000 | 450 | $3,375 | $2,363 | $200 | $135 | +$2,028 | +$2,317 |
| 5 (Oct 26) | 40,000 | 600 | $4,500 | $3,150 | $300 | $180 | +$2,670 | +$4,987 |
| 6 (Nov 26) | 50,000 | 850 | $6,375 | $4,463 | $400 | $255 | +$3,808 | +$8,795 |
| 7 (Dec 26) | 62,000 | 1,050 | $7,875 | $5,513 | $500 | $315 | +$4,698 | +$13,493 |
| 8 (Jan 27) | 75,000 | 1,250 | $9,375 | $6,563 | $600 | $375 | +$5,588 | +$19,081 |
| 9 (Feb 27) | 90,000 | 1,520 | $11,400 | $7,980 | $700 | $456 | +$6,824 | +$25,905 |
| 10 (Mar 27) | 105,000 | 1,750 | $13,125 | $9,188 | $800 | $525 | +$7,863 | +$33,768 |
| 11 (Apr 27) | 122,000 | 2,000 | $15,000 | $10,500 | $900 | $600 | +$9,000 | +$42,768 |
| 12 (May 27) | 140,000 | 2,300 | $17,250 | $12,075 | $1,000 | $690 | +$10,385 | **+$53,153** |

**Y1 Optimistic Totals:**
- Gross revenue: **~$91,560** (sum of monthly gross)
- Net revenue (after 30% cut): **~$64,180**
- Total costs (fixed + variable + initial $1,500 seed): **~$11,025** ops + $1,500 seed
- **Y1 Net cash position (excl. founder salary): +$53,153**
- Cash flow break-even (monthly): **Month 1 (immediate)**
- Cumulative break-even: **Month 3 (Aug 26)**
- ARR run-rate end Y1: **~$145K**
- **Founder salary trigger: Month 5 (Oct 26)** — $5K MRR net crossed, salary $2.5K/mo from M6
- Reinvestment available Y1: **~$40K** (after $13K founder salary M6-M12)

---

### PESSIMISTIC Scenario (10th percentile — WWDC commoditization OR D30 retention collapse)

**Assumptions:**
- Apple ships ADHD-aware AI scheduler at WWDC June 8 → forced reposition to "ADHD layer over Apple Intelligence"
- Day-30 retention: **6%** (productivity benchmark default; ADHD design wedge fails to differentiate)
- Trial-to-paid: **12%** (low-intent traffic, paywall fatigue)
- Tier mix: skews monthly (anxiety about commitment) — **65% monthly / 20% 6mo / 15% annual**
- Blended net revenue per paid user: $5.25/mo (heavier monthly weight)
- **Decision gate: Month 6 review — pivot, raise emergency capital, or wind down**

| Month | Users | Paying | MRR gross | MRR net (70%) | Net cash | Cum cash |
|-------|-------|--------|-----------|---------------|----------|----------|
| 1 (Jun 26) | 500 | 8 | $60 | $42 | -$63 | -$1,563 |
| 2 (Jul 26) | 900 | 15 | $113 | $79 | -$26 | -$1,589 |
| 3 (Aug 26) | 1,500 | 25 | $188 | $131 | +$11 | -$1,578 |
| 4 (Sep 26) | 2,200 | 40 | $300 | $210 | +$60 | -$1,518 |
| 5 (Oct 26) | 2,900 | 55 | $413 | $289 | +$109 | -$1,409 |
| 6 (Nov 26) | 3,500 | 70 | $525 | $367 | +$167 | **-$1,242** ← decision gate |
| 7 (Dec 26) | 4,200 | 90 | $675 | $473 | +$253 | -$989 |
| 8 (Jan 27) | 4,800 | 105 | $788 | $551 | +$311 | -$678 |
| 9 (Feb 27) | 5,500 | 125 | $938 | $656 | +$390 | -$288 |
| 10 (Mar 27) | 6,200 | 145 | $1,088 | $761 | +$471 | +$183 |
| 11 (Apr 27) | 6,900 | 165 | $1,238 | $866 | +$546 | +$729 |
| 12 (May 27) | 7,500 | 180 | $1,350 | $945 | +$620 | **+$1,349** |

**Y1 Pessimistic Totals:**
- Gross revenue: **~$7,675** (sum of monthly gross)
- Net revenue (after 30% cut): **~$5,370**
- Cash flow break-even (monthly): **Month 3 (Aug 26)**
- Cumulative break-even: **Month 10 (Mar 27)** — slow, painful
- ARR run-rate end Y1: **~$11.3K**
- **Decision gate Month 6 (Nov 26):** If still in pessimistic territory (<$500 net MRR, cumulative <-$1,000), trigger one of:
  1. **Pivot to "ADHD layer over Apple Intelligence"** — reposition + relaunch
  2. **Emergency bridge** (founder personal $3-5K or pre-seed friends/family check)
  3. **Sunset gracefully** — recover ~$500-1,000 from honoring annual refunds and shutting down infrastructure

---

## 3-Year Annual Projections (Base Case)

| Year | Users (end) | Paying (end) | MRR net (end) | ARR run-rate | Y End Cash (cumulative) | Founder Salary | Major Events |
|------|-------------|--------------|---------------|--------------|------------------------|----------------|--------------|
| **Y1 (2026-27)** | 50,000 | 850 | $4,463 | **$53.5K** | **+$18K** | $0 (M1-7) → $1.5-2.5K/mo decision M8 | Launch (Jun 22), Tracy Otsuka deal, Apple SBP application, iOS-only |
| **Y2 (2027-28)** | 145,000 | 2,500 | $15,930 | **$191K** | **+$80K** | $3-4K/mo from M14 | Apple SBP approved (-15% fee), Android launch M13, Hebrew RTL M18, partner mode v1.1 |
| **Y3 (2028-29)** | 290,000 | 6,000 | $38,220 | **$459K** | **+$280K** | $6-8K/mo | 2 advisory partnerships, referral program, possible seed round optionality, AuDHD/couples expansion |

### Y2 Assumptions (driving the $53K → $191K growth)

| Driver | Impact |
|---|---|
| Apple SBP approved (15% vs 30% fee) | +21% net revenue per paying user (blended $5.24 → $6.37/mo) |
| Google Play 15% tier (automatic <$1M proceeds) | Android paying users at 85% cut from day 1 |
| Android launch Month 13 (Y2 M1) | +30-50% reachable user base (~40K additional Y2 users) |
| Hebrew RTL launch Month 18 (Y2 M6) | Incremental $10-30K ARR from Israel (capped TAM) |
| Partner mode v1.1 (M15-18) | 15-25% viral acquisition lift via dyadic invitations |
| 2x marketing budget ($1K-3K/mo from reinvestment) | Tracy Otsuka renewal, ADDitude paid placement, ASA scaling |
| Compounding annual cohort retention (RevenueCat: 36% Y2) | Y1 annual buyers convert ~36% to Y2 → ~$15-20K base ARR carried |
| Founder salary $3-4K/mo from M14 | -$36-48K Y2 cash impact, still net positive |

### Y3 Assumptions (driving $191K → $459K growth)

| Driver | Impact |
|---|---|
| Established brand + organic compounding (TikTok/SEO/Pinterest 3-6mo tails) | Lower effective CAC ($3-7 blended) |
| Referral program (15-20% of new acquisitions) | Free user growth channel — direct ARR contribution ~$60-90K |
| AuDHD/couples mode (if validation positive in Y2) | New SKU $79.99/yr → $40-80K ARR contribution |
| 2 paid advisory partnerships (CHADD, ADDitude editorial integration) | Brand authority → conversion lift 10-15% |
| Possible seed round $500K-$1M @ $200-500K ARR | Optional — hire iOS engineer + designer if raised |
| Founder salary $6-8K/mo (market-rate solo) | -$72-96K Y3 cash impact |
| Annual cohort compounding (Y1 36%, Y2 ~30%) | Stable revenue base ~$60-100K from prior-year carry |

---

## Cash Flow Timeline (Base Case)

```
Month 0 (May 28, 2026 — today):
  $1,500 personal seed in bank
  No revenue, no Apple Developer payout yet

Month 1 (Jun 22 launch):
  -$1,500 seed deployment (Apple/Google enrollment, hosting, Canva, domain, Tracy deposit)
  $94 gross MRR booked
  $0 cash actually received (Apple holds 30-45 days)
  Cumulative cash: -$1,511

Month 2 (Jul 26):
  $263 gross MRR booked
  First Apple payout arrives (~Month 1 revenue): +$60
  Cumulative cash: -$1,368

Month 3 (Aug 26):
  $578 net MRR booked
  Cash flow positive MONTHLY (+$418)
  Apple payouts catching up
  Cumulative cash: -$950

Month 4 (Sep 26):
  Annual subs from M1-2 cohort cross "30-day refund safe" threshold
  Reinvestment pool meaningfully starts
  Cumulative cash: -$241

Month 5 (Oct 26):
  Cumulative break-even crossed (+$807)
  First "comfortable" month — founder can stop checking bank balance daily

Month 6 (Nov 26):
  $1,680 net MRR
  $2K MRR community trigger approaching → plan Discord launch for Month 7
  Cumulative cash: +$2,177

Month 7 (Dec 26):
  $2,153 net MRR — Discord launched
  Could afford small contractor ($300-500 one-off iOS feature ship)

Month 8 (Jan 27):
  $2,625 net MRR (~$5K gross MRR threshold crossed)
  **FOUNDER SALARY DECISION POINT**
  Options:
    A) Take $1,500/mo (keeps $1,125 reinvestment)
    B) Take $2,500/mo (keeps $125 reinvestment — barely covers ops)
    C) Stay $0 (full reinvestment toward $10K MRR by M12)

Month 12 (May 27):
  $4,463 net MRR ($53.5K ARR run-rate)
  Cumulative: +$18,106 (or +$5-10K after partial salary)
  Y1 review → Y2 plan: Android, Hebrew, SBP confirmed, raise decision
```

---

## Funding Runway Analysis

### No-Funding Path (Bootstrap — DEFAULT)

| Period | Founder Salary | Personal Runway Required | Status |
|---|---|---|---|
| M1-7 (Jun-Dec 26) | $0 | $X/mo from personal savings (founder family-specific) | Required |
| M8-12 (Jan-May 27) | $0-2.5K/mo | Partial offset; still personal runway needed | Decision-dependent |
| Y2 M1+ | $3-4K/mo from MRR | Personal runway no longer required | Sustainable |
| Y3+ | $6-8K/mo | Market-rate solo founder comp | Comfortable |

**Critical:** No-salary policy works only if founder family runway covers 7-14 months of living costs. If personal runway exhausted before M7, model collapses regardless of MRR.

### Seed Round Scenarios (When/Why Raise)

#### Scenario A: Raise at $5-10K MRR (Month 6-9, base case)
- **Amount:** $250K-500K pre-seed
- **Use:** Hire iOS engineer ($120-150K/yr) + accelerate Android + marketing test budget ($5K/mo)
- **Comp:** Inflow $11M Series A (overkill for stage); Saner.AI Techstars + Google check
- **Realistic investors:** Octopus Ventures, A.Capital, Worklife, Will Ventures (ADHD/mental health-focused)
- **Dilution:** 15-25%
- **Why:** Capture window before Apple Intelligence commoditizes; accelerate Tracy network effect
- **Risk:** Pressure to deliver hockey-stick metrics; founder loses optionality on bootstrap path

#### Scenario B: Raise at $20K MRR (Y2 Q1-Q2)
- **Amount:** $750K-1M seed
- **Use:** iOS + Android engineer + designer + 6-month marketing experimentation
- **Dilution:** 10-20% (more leverage at this stage)
- **Why:** Multi-platform expansion + retention investment + founder salary headroom
- **Risk:** Slower; competitors may close window

#### Scenario C: Bootstrap to profitability ($300K+ ARR)
- **No raise; solo founder + 1-2 contractors**
- **Sunsama-style path** — exit benchmark ~$1.5M ARR bootstrap acquisition
- **Why:** Founder optionality, no investor pressure, full equity retention
- **Risk:** Slower growth; Apple/Tiimo may close window; founder burnout risk

**Founder decision (Phase 8 — risk-analysis.md):** Depends on personal preference + family runway + WWDC outcome.

---

## Key Inflection Points

| Month | Date | Event | Significance |
|-------|------|-------|--------------|
| M0 (today) | May 28 26 | $1,500 seed deployed | Starting line; clock starts |
| M0 + 11d | Jun 8 26 | **WWDC Apple keynote** | Binary risk event — pivot trigger if ADHD-aware AI scheduler shipped |
| M1 | Jun 22 26 | **Launch** | Day 0 commercial; first $9.99 booked |
| M1-2 | Jun-Jul 26 | Apple SBP application submitted | Approval window 30 days; Y2 economics depend on this |
| M2-3 | Jul-Aug 26 | Tracy Otsuka episode drop | Single largest single-day acquisition event Y1 |
| M3 | Aug 26 | **Cash flow monthly break-even (base)** | Survival validated; reinvestment engine starts |
| M5 | Oct 26 | **Cumulative cash >$0 (base)** | First "safe" month |
| M5 | Oct 26 | $1K+ net MRR (base) | Sustainable trajectory confirmed |
| M6 | Nov 26 | **Pessimistic decision gate** | If <$500 MRR, pivot/sunset/bridge decision |
| M6 | Nov 26 | $2K MRR community trigger | Discord launch; reduce 1:1 support load |
| M7 | Dec 26 | $2K+ net MRR | First fractional iOS contractor possible |
| M8 | Jan 27 | **$5K gross MRR — founder salary decision** | $0 reinvestment vs $1.5-2.5K salary tradeoff |
| M10 | Mar 27 | $3K+ net MRR | Comfortable bootstrap; raise optionality opens |
| M12 | May 27 | $4-5K net MRR (~$53K ARR) | Y1 review; Y2 plan commits |
| Y2 M1 | Jun 27 | **Android launch** | +30-50% TAM unlock |
| Y2 M6 | Nov 27 | **Hebrew RTL launch** | Israel beachhead (~$10-30K ARR) |
| Y2 M12 | May 28 | $13K+ net MRR (~$160K ARR) | VC-qualifiable metrics |
| Y3 M12 | May 29 | $32K+ net MRR (~$385K ARR) | Comfortable bootstrap OR strategic raise/exit window |

---

## Sensitivity Visualizations

### If Day-30 Retention is Half of Base Hypothesis (6% vs 12%)
- Y1 ARR drops from $53K → ~$29K (-45%)
- Cumulative cash Month 12: ~+$10K vs +$18K (-44%)
- Time to $5K MRR slips from Month 8 → Month 12+
- Cumulative break-even slips from M5 → M9
- **Action:** Retention design (D7, D14, D30 specifically) is the #1 product priority; ship gentle re-engagement in v1, not v1.1

### If Trial-to-Paid Conversion Drops to 15% (vs 25% base)
- Y1 ARR drops from $53K → ~$32K (-40%)
- Time to $5K MRR slips from M8 → M11
- **Action:** Paywall A/B testing weekly from Month 1; if conversion <18% by M3, redesign paywall before scaling acquisition

### If Refund Rate Exceeds 5% (vs <2% target)
- Each additional 1% above 2% reduces net revenue by ~1%
- At 5% refund rate: Y1 cash impact ~-$1,200; at 8%: ~-$3,000
- **Action:** Sessions-gated refund (<10 sessions in 30 days) enforced from day 1; if refund rate >5% by M3, intervene immediately (paywall clarity, expectations management, onboarding)

### If Apple Small Business Program NOT Granted (stay at 30% fee in Y2)
- Net revenue per user stays at 70% (not 85%) → Y2 net MRR ~21% lower
- Y2 ARR: $191K → ~$158K
- Y2 cash position: +$80K → +$50K
- **Action:** Apply Day 1 (week 2 of submission); verify status before Y2 budget planning; have backup plan for slower growth

### If Tracy Otsuka Deal Doesn't Close
- Replace with 3-5 micro-creator deals at $200-400 each = $1,000-2,000
- Lower peak acquisition per event, but more distributed risk
- Y1 ARR impact: -10-15% in base case
- **Action:** Don't bet entire acquisition strategy on single creator; secondary deals lined up by M2

### If WWDC Ships ADHD-Aware AI Scheduler (Pessimistic-1)
- 90-day reposition required: "ADHD layer over Apple Intelligence"
- Acquisition slowdown: -50-70% for 60-90 days
- Y1 ARR: $53K → ~$11K (Pessimistic scenario realized)
- **Action:** Pre-built reposition messaging ready Day -1; press release drafted; pivot to vertical/specific (women, dyadic, AuDHD)

### If LLM Costs Spike to $0.50/user/mo (heavy users emerge)
- At 850 paying users: $425/mo additional cost = ~10% of net MRR
- Y1 impact: ~-$2,500
- **Action:** Rate-limiting on free chat; tier-up to GPT-4o for power users with $14.99 add-on; on-device inference for iOS 27+ (WWDC dependency)

---

## Comparison vs Industry (B2C Consumer SaaS — Mobile Subscription)

| Metric | Industry Healthy | Planny Base Y1 | Status |
|--------|------------------|----------------|--------|
| Net new MRR growth | 10-20% MoM | 15-30% MoM (Months 4-12) | Healthy |
| Time to first profit (monthly) | 6-18 months | Month 2 (no founder salary) | Excellent |
| Time to cumulative break-even | 12-24 months | Month 5 | Excellent |
| Gross margin | 70-85% | 94% Y1 / 96% Y2 | Excellent (mobile + LLM efficient) |
| ARR / employee | $50K+ at scale | $53K Y1 (solo) → improves | Acceptable solo |
| LTV / CAC ratio | 3:1+ | ~5-12:1 (organic-heavy) | Excellent |
| D30 retention (productivity) | 4.1% | 12% target / 6% pessimistic | Excellent if hits target |
| Trial-to-paid (opt-in CC) | 18-25% | 25% target | At benchmark |
| Refund rate | 2-5% | <2% target (sessions-gated) | Excellent if achieved |
| Net revenue retention | 100-110% | TBD (Y2 cohort data) | Unknown |

---

## Reinvestment Math (Compounding Detail — Base Case)

```
Monthly Spending Capacity = (Initial Seed - Cumulative Prior Spend) + Cumulative Net Revenue (>30d safe)

Month 1: Pool = $1,500 - $500 ops - $1,000 marketing prep = $0 (fully deployed)
Month 2: Pool = $0 + $94 net rev (delayed cash) = $94 actually available
Month 3: Pool = $0 + $263 net rev + $40 carry = $303 available marketing pool
Month 4: Pool = $0 + $578 net rev + $200 carry = $778 marketing pool
Month 5: Pool = ~$1,300/mo from this point — meaningful spend possible
Month 6: Pool = ~$1,700/mo
Month 12: Pool = ~$3,600/mo

Practical implication: First $1,500 funds tools + Tracy deposit + ASA pilot.
Cumulative net revenue overtakes initial seed deployment by ~M3-4.
By M6+, every paying user funds future acquisition at 100% reinvest rate.
```

**Working Capital Reality (cash vs accrual gap):**
- Annual subscription booked Day 1 = $59.99 gross
- Apple holds payment 30-45 days = received Day 30-45
- 30-day refund window = "safe" only Day 60+
- **Plan: Treat all cash <Day 60 as conditional; don't over-commit marketing on unrealized revenue**

---

## Honest Disclaimers

1. **These projections assume the Aha moment works** (voice brain-dump → first plan <90s). If it doesn't deliver the "this app gets me" reaction, all retention numbers collapse and the model breaks within 90 days.

2. **Day-30 retention is the #1 unknown.** No ADHD-specific cohort data exists publicly. We use productivity (4.1%) and mental-health (3.3%) benchmarks as floors; best-in-class evidence-based (16%) as ceiling. Real number is unknown until M2-3 cohort data emerges.

3. **WWDC June 8 outcome could nullify the BASE scenario** within 90 days. The Mayday Labs acquisition + Gemini Spark precedent raise probability of "good enough" AI scheduling shipping in iOS 27. Pivot ready Day -1.

4. **Founder hasn't validated demand directly via paid customer discovery.** Projections rest on inferred demand signals (CDC prevalence, Tiimo + Numo + Inflow market existence, r/ADHDWomen engagement). The first 50-100 paying users are the real validation event.

5. **LLM costs at scale may be higher** if heavy users (power-user 5%) drive 50%+ of API calls. Build rate-limiting + power-user upsell into pricing logic by M6.

6. **Reinvestment compounding works only if retention holds.** If churn exceeds reinvestment ROI (i.e., new $1 in acquisition returns <$1 in 6-month LTV), model breaks. This is the existential math.

7. **Cash flow lag (60-day working capital gap)** means cumulative cash projections lag actual revenue bookings. M3 "break-even" is on accrual; on cash basis, true break-even is M5-6.

8. **Y2-Y3 projections are directional, not committed.** They depend on SBP approval, Android execution quality, Israel localization quality, retention holding, no major regulatory event (MHMDA/FTC), no founder personal crisis, no Apple/Tiimo strategic move.

---

## Strategic Connections
- ראה `revenue-model.md` (Phase 7 — Financial) ל-pricing logic מפורט (when written; pricing summary in business-model.md §Revenue Model)
- ראה `cost-structure.md` (Phase 7 — Financial) ל-cost detail (when written; cost summary in business-model.md §Cost Structure)
- ראה `../02-strategy/business-model.md` ל-unit economics, LTV/CAC, scenarios source
- ראה `../02-strategy/go-to-market.md` ל-channel-by-channel CAC modeling
- ראה `../06-validation/risk-analysis.md` (Phase 8) ל-risk-weighted scenarios + WWDC contingency

---

## Sources

### Tier 1 (primary, recent, methodologically strong)
- RevenueCat State of Subscription Apps 2025 + 2026 — productivity LTV $46.97 US best country-category; D30 productivity 4.1%; annual cohort 36% Y2 retention; trial-to-paid opt-in 18-25%
- Adapty State of In-App Subscriptions 2025 + Free Trial Conversion Rates 2026
- Apple Developer official — Small Business Program (<$1M ARR → 15% fee), App Store Connect pricing
- Google Play official — 15% tier automatic <$1M proceeds, October 2025 pricing template changes
- AppTweak 2026 — iOS CPI productivity NA $2.84 (+90% YoY)
- Recurly subscription benchmarks (67M subscribers) — trial-to-paid YoY decline 46% → 33%
- Business of Apps — CPI, retention, trial benchmarks across categories

### Tier 2 (specialized industry, useful)
- First Page Sage / ChartMogul — trial conversion studies (opt-in 18-25%, opt-out 49-60%)
- Amraandelma 2025 — productivity D30 4.1% benchmark
- HCPLive, Wallace PhD — mental health app retention (D30 3.3%)
- BusinessDojo, Mapendo — NA ARPU $6.20/mo
- ChoosingTherapy 2025 Inflow review — billing reputation
- 42matters — Israel app market statistics
- Comp benchmarks: Reclaim → Dropbox $40.2M acquisition (320K users, Jul 2024); Inflow $11M Series A; Saner.AI Techstars + Google; Shimmer $3.5M seed

### Tier 3 (anecdotal, used with skepticism)
- Trustpilot/Pissedconsumer reviews (selection bias)
- SubJolt, Focus Digital — churn benchmarks (proxy, no ADHD-specific)

---

## Flags

### Red Flags

1. **Y1 cumulative cash in base case ($18K) does NOT fund founder full salary.** Salary must come from existing personal runway OR partial reinvestment sacrifice OR pivot to seed raise. The 7-month no-salary period is the real personal-runway test.

2. **Pessimistic scenario (WWDC commoditization or D30 collapse) requires hard decision at Month 6.** Pivot/bridge/sunset — no halfway option. Founder must agree to decision criteria pre-launch.

3. **Day-30 retention unknown for ADHD audience — model breaks if <6%.** No public ADHD-specific cohort data. First reliable signal is M3 cohort behavior. If D30 <6% by M3, intervention required before reinvestment exhausts.

4. **WWDC June 8 (in 11 days) is binary risk event.** If Apple ships ADHD-aware AI scheduler, 50-70% acquisition slowdown for 60-90 days. Pivot messaging must be ready Day -1, not Day +30.

5. **60-day working capital gap (Apple/Google hold + refund window).** Cumulative cash projections lag actual booked revenue. Don't over-commit marketing on Day 1-30 bookings.

6. **Inflow $11M Meta/TikTok ad spend has poisoned auctions** for ADHD-niche targeting. Paid CAC >$30 unsustainable. Organic-only acquisition is mandatory, not optional. If organic doesn't deliver 200+ paying users by M3, no paid backup exists.

### Yellow Flags

1. **3-year projections are speculative — Y3 numbers are directional, not committed.** SBP approval, Android execution, retention stability, no regulatory event all required.

2. **SBP application timing critical.** If approval delayed beyond M3, Y1 economics moderately worse; if denied entirely, Y2 ARR -21% vs projection.

3. **Israel + Android in Y2 add execution complexity.** Solo founder shipping iOS, Android, Hebrew RTL, partner mode v1.1 simultaneously is aggressive. Sequencing matters.

4. **6-month tier may cannibalize annual** if persuasion math fails. Monitor tier mix monthly; if 6mo >40% of mix by M3, re-tune paywall.

5. **Refund rate sensitivity** — every 1% above 2% target erodes net LTV directly. Sessions-gated refund (<10 sessions in 30 days) protects but adds support load.

6. **Founder personal exposure (bootstrap = personal financial risk).** Model has no buffer for medical emergency, family crisis, or Israeli reservist call-up. Y1 has ~3-5 months of zero-buffer period.

7. **California ARL (SB 313), NY, Colorado, FTC click-to-cancel — single retention offer max, click-to-cancel required.** Recommended flow already compliant, but legal review pre-launch needed.

8. **Annual cohort renewal assumption (36% Y2 per RevenueCat productivity benchmark)** is critical to Y2 base ARR. If ADHD audience renews at 20% (lower follow-through), Y2 ARR drops 10-15%.

9. **Tiimo iPhone App of the Year halo effect** gives them 12 months of marketing oxygen. Planny's wedge (weekly cadence + late-dx women + conversational re-plan) must be visibly distinct or projections compress.
