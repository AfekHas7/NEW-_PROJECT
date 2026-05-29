# Cost Structure — Planny

**Phase:** Phase 7 — Financial (Cost Structure)
**Project:** startup-validation (Planny)
**Date:** 2026-05-28
**Confidence:** Medium-High — fixed/variable line items מבוססים על business-model.md unit economics (Tier 1: RevenueCat 2026, Apple/Google official) + regulatory.md compliance estimates; LLM-per-user נתון מ-OpenAI/Anthropic public pricing; contractor/Y2 הערכות הן ranges based on market rates, not committed numbers

---

## תקציר Cost Structure

Planny מבני עם **gross margin של 94%+ ברמת unit economics** ועם **fixed costs מינוריים** ב-Phase 1 (תחת $150/mo). זה לא במקרה — זה הייעוד של bootstrap SaaS mobile עם Apple/Google handling billing infrastructure ו-LLM-on-demand pricing.

מה שמשתנה עם scale:
- **LLM API** — הוא ה-single most-variable line item. ב-Phase 1 (50-150 active) זה $30-80/mo; ב-scale (5K active) זה $1K-1.5K/mo. אבל זה משתנה proportional עם revenue (per-active-user $0.10-0.30/mo flat).
- **Apple/Google fee** — 30% גרוס בשנה 1, 15% משנה 2 אם SBP אושר. זה ה-largest variable line ב-revenue terms.
- **Backend (Supabase Pro)** — קופץ מ-$0 ל-$25-50 כשעוברים free tier, ואז ל-$100+ ב-2K+ users.
- **Customer support load** — לא בדולרים אלא בזמן founder; ב-1K+ paid users הופך ל-bottleneck.

מה שנשאר fixed (ולא משתנה עם scale עד Y2):
- Apple Developer Program ($99/yr)
- Domain + email ($120/yr)
- Free-tier services (OneSignal, Sentry, Mixpanel) — נשארים free עד 10K subscribers / 100K events
- Founder time (לא דולרים ב-Y1 לפי no-salary policy)

ה-Phase שבו ה-cost structure משתנה דרמטית הוא **Year 2**, כשנכנסים contractor + bookkeeping + Israel compliance + Hebrew localization. נכון לעכשיו (May 2026, pre-launch), ה-burn החודשי הריאלי הוא ~$100-150 קבועים + reinvestment של 100% מ-revenue ל-marketing.

ה-existential cost risk הוא לא הסכום אלא ה-**concentration**: $500-2,000 compliance legal הם 33-133% מה-seed budget, ו-LLM cost-runaway מ-heavy users יכול לשרוף gross margin אם לא יוטלו rate limits.

---

## Fixed Costs (Monthly)

### Launch Phase (Month 1-6, ≤500 paying users)

| Item | Cost/Month | Source | Notes |
|------|-----------|--------|-------|
| Apple Developer Program | $8.25 | $99/yr amortized | Required for App Store |
| Google Play one-time | ~$0 | $25 one-time | Negligible amortized |
| Backend hosting (Supabase free → Pro) | $25-50 | Free tier expires at usage | Auto-scales |
| LLM API (~50-150 active users early) | $30-80 | $0.20/active user avg | OpenAI GPT-4o-mini primary, Anthropic Haiku backup |
| RevenueCat (subscription mgmt) | $0 | Free <$2.5K MTR | Free tier sufficient |
| Push notification (OneSignal free) | $0 | Free up to 10K subscribers | Free tier sufficient |
| Email service (ConvertKit/Resend free) | $0-15 | Free up to 1K contacts | |
| Domain + Google Workspace email | $10 | $120/yr | |
| Analytics (Mixpanel/PostHog free) | $0 | Free up to 100K events | |
| Crash reporting (Sentry free) | $0 | Free tier | |
| Customer support (founder Gmail) | $0 | Pre-scale | |
| **Total monthly fixed** | **~$73-163** | | Excludes Apple/Google fee (variable) |

### Growth Phase (Month 7-12, 500-1,500 paying users)

| Item | Cost/Month | Notes |
|------|-----------|-------|
| Apple Developer Program | $8.25 | |
| Backend hosting (Supabase Pro) | $50-100 | Paid tier needed at ~1K MAU |
| LLM API (500-1,500 active) | $150-450 | Scales linearly at $0.10-0.30/active user |
| RevenueCat (post-$2.5K MTR) | $25-50 | Starts charging post-threshold |
| Push notification (OneSignal Growth) | $0 | Still free under 10K |
| Email service (ConvertKit Creator) | $15-29 | Growing list past 1K |
| Analytics (Mixpanel Free → Growth) | $0-50 | Free until 100K events/mo |
| Crash reporting (Sentry Team) | $26 | $26/mo for team plan when needed |
| Customer support (Help Scout / Front) | $25 | When DM volume crosses ~50/wk |
| ASO tools (AppTweak Lite / Sensor Tower) | $79-149 | Optional but useful at scale |
| Domain + email | $10 | |
| **Total monthly fixed** | **~$390-870** | |

### Scale Phase (Year 2, 2,500-5,000 paying users)

| Item | Cost/Month | Notes |
|------|-----------|-------|
| All Phase-2 items scaled | $700-1,200 | LLM + backend + tools grow |
| iOS contractor (part-time, 20 hr/mo) | $1,500-3,000 | Per business-model "Scaling Triggers" $5K MRR |
| Designer (project basis, amortized) | $300-1,000 | Quarterly engagements |
| Bookkeeping / accounting | $200-400 | Required at $50K+ ARR |
| Legal (occasional review) | $200-500 | Quarterly check-in |
| Israel fractional DPO (post 10K IL users) | $700-2,000 | $8K-25K/yr per regulatory.md |
| MHMDA-aware privacy counsel (one-off audits amortized) | $200-500 | Per regulatory.md scale tier |
| **Total monthly fixed (Y2)** | **~$3,800-8,600** | |

---

## Variable Costs (Per User)

### Per Active User (monthly)

| Item | Cost | Notes |
|------|------|-------|
| Apple/Google fee | 30% (Y1) / 15% (Y2 post-SBP) | Of gross subscription revenue |
| LLM API | $0.10-0.30/mo | Voice → AI plan + quick-add + weekly review |
| Database (Supabase) | $0.02-0.05/mo | Drops to $0.02 at 5K+ scale |
| Auth + storage | $0.02/mo | Bundled in Supabase tier |
| Push notifications | $0.001/mo | OneSignal free tier sustains <10K |
| Email (occasional broadcast) | $0.01/mo | Spread ConvertKit cost |
| **Total variable cost per active user** | **~$0.15-0.38/mo** | Plus Apple/Google fee on revenue |

### LLM Cost Detail (most variable line item)

Voice → AI plan estimate per session:
- Whisper transcription: $0.006/min × 30-90 sec = **$0.003-0.009 per session**
- LLM parsing (GPT-4o-mini): ~500 tokens input + 1,000 output × $0.15/$0.60 per 1M = **~$0.0007 per session**
- Voice quick-add: ~50 input + 100 output = **~$0.0001 per use**
- **Per session cost: ~$0.004-0.010**
- **Per active user/month (assume 4-8 voice sessions): $0.02-0.08/mo base**

Plus weekly review prompts, AI re-plan after missed task, partner sync (v1.1), conversational refinement = round to **$0.10-0.30/mo per active user** for typical use.

**Heavy-user worst case:** 20+ brain-dumps/mo × $0.05/session blended = $1.00+/mo → still gross-margin positive but cuts margin in half. Mitigation: soft rate-limit at 20 sessions/mo.

### Cost Per Paying User (gross margin calc)

Reference: business-model.md blended net revenue Y1 = **$5.24/mo** (blended across 40% monthly / 30% 6mo / 30% annual)

Variable cost per paying user (≠ active user; paying users typically more active):
- LLM: $0.20/mo (mid-range)
- DB + auth + storage: $0.07/mo
- Push + email: $0.01/mo
- **Total: ~$0.28/mo per paying user**

**Gross margin per paying user (Y1, 30% Apple cut):** $5.24 - $0.28 = **$4.96/mo (94.7%)**
**Gross margin per paying user (Y2, 15% SBP):** $6.37 - $0.28 = **$6.09/mo (95.6%)**

---

## One-Time Costs (Launch + Year 1)

### Pre-Launch (must-have before June 22, 2026)

| Item | Cost | When | Notes |
|------|------|------|-------|
| Legal: Privacy Policy + ToS (template + light review) | $300-800 | Pre-launch | |
| Legal: Medical Disclaimer wording | $0-200 | Pre-launch | Bundled with above |
| Legal: MHMDA-compliant Health Data Privacy Policy + consent UX | $500-1,200 | Pre-launch | **Mandatory per regulatory.md (private right of action)** |
| CCPA SPI opt-out + "Limit Use" links | $0-300 | Pre-launch | Bundled or template |
| Apple Developer Program (year 1) | $99 | Already enrolled | |
| Google Play Developer (one-time) | $25 | Pre-launch | |
| Brand assets / logo | $0 | Founder-produced | Per business-model.md |
| App Store screenshots + listing optimization | $0-300 | Pre-launch | DIY or Fiverr |
| ASO keyword research (one-time AppTweak/Sensor Tower) | $0-99 | Optional | |
| Apple Privacy Manifest + Google Data Safety form drafting | $0 | Pre-launch | Engineering |
| Marketing Language Policy (one-pager, founder-drafted, lawyer-reviewed) | $0-200 | Pre-launch | **Cheapest highest-impact regulatory control per regulatory.md** |
| **Total one-time pre-launch (low end / high end)** | **$924-3,124** | Scrappy target: ~$1,200-1,500 |

### Year 1 One-Time Additions

| Item | Cost | When | Notes |
|------|------|------|-------|
| Hebrew RTL translation + Hebrew Privacy Policy | $300-900 | Month 6+ if IL launch | Per business-model.md |
| Trademark search (Planny) | $200-500 | When viable | |
| Bookkeeping setup (QuickBooks / Wave) | $0-200 | At ~$25K ARR | |
| LLC / Ltd entity formation (if not done) | $300-800 | Recommended for Google Org Account | Per regulatory.md |
| **Total Y1 one-time (excl. Android)** | **$800-2,400** | |
| Android port (deferred to Y2 per scope) | $5K-15K | Y2 | Major effort, not Y1 |

**Compliance cost note:** regulatory.md estimates **$8K-19K** for US-only minimum-viable compliance at launch (full bespoke). The $500-1,200 line above assumes **template-first scrappy approach with light lawyer review**, which is the founder-realistic path given $1,500 seed budget. Full bespoke compliance is deferred to Y2 post-revenue.

---

## Marketing Reinvestment Allocation

### $1,500 Seed Budget Allocation (Month 1-3)

| Item | Allocation | Notes |
|------|-----------|-------|
| Tracy Otsuka pod episode (host-read or sponsorship slot) | $800-1,500 | Top creator ROI per business-model.md |
| ADDitude newsletter slot OR ASA long-tail | $300-500 | Secondary creator/channel ROI |
| Apple Search Ads test (Month 1-2, defensive brand + long-tail) | $200-500 | Defensive ASA per business-model.md sensitivity |
| Privacy policy legal review (one-time) | $500 | One-time, critical (counts against seed) |
| Tools (Canva, ConvertKit, domain, Carrd Pro) | $50-150 | One-time setup |
| **Total launch quarter outlay** | **~$1,850-3,150** | Exceeds $1,500 seed; gap funded by Month 1-3 revenue (~$94-570/mo base scenario) |

**Practical sequence:**
- Month 0 (pre-launch May-June 2026): legal $500 + tools $150 = $650 of seed
- Month 1: ASA test $200 + Tracy outreach $0 = $200
- Month 2: Tracy episode $800-1,200 = remainder of seed
- Month 3+: 100% revenue reinvestment per founder policy

### Reinvestment Plan (Month 4-12, scaling with revenue)

Based on **Base scenario** from business-model.md (Net MRR after Apple cut, blended):

| Month | Paying Users (base) | Net MRR (base) | Reinvestment Cap | Recommended Allocation |
|-------|---------------------|----------------|------------------|------------------------|
| 4 | ~180 | ~$945 | $945 | $400 ASA + $300 creator gifts + $245 ops/tools |
| 6 | 320 | $1,675 | $1,675 | $500 ASA + $500 podcast slot + $400 newsletter + $275 buffer |
| 9 | 580 | $3,040 | $3,040 | $1,000 ASA + $800 creator pod + $600 newsletter + $400 SEO content + $240 misc |
| 12 | 850 | $4,455 | $4,455 | $1,500 ASA + paid retargeting + $1,000 podcasts + $800 newsletter + $700 content + $455 ops |

**Channel allocation principle (per business-model.md sensitivity):** Never spend >40% of monthly pool on paid; keep 60%+ in organic compounding (content, creators, SEO).

### Reinvestment vs. Founder Salary Tension

Per business-model.md founder-salary plan:
- **Months 1-6: $0 salary, 100% reinvestment**
- **Months 7-12: conditional $1,500-2,500/mo at $5K MRR threshold ($60K ARR)**

If founder takes $2,500/mo from Month 7 onwards in base scenario:
- Month 7-9: Net MRR ~$2,000-3,000 → reinvestment shrinks to $0-500/mo (most goes to salary + fixed)
- Month 10-12: Net MRR ~$3,500-4,500 → reinvestment ~$500-1,500/mo (constrained)
- **Trade-off:** Founder salary at $5K MRR essentially **halts marketing compounding**. Recommend deferring salary to $8-10K MRR threshold if personal runway allows.

---

## Break-Even Analysis

### Variable Cost Break-Even

- Net revenue per paying user (Y1 blended): **$5.24/mo**
- Variable cost per paying user: **$0.28/mo** (LLM + DB + auth + push + email)
- **Contribution margin per paying user: $4.96/mo gross profit**

### Fixed Cost Coverage Break-Even

| Phase | Fixed Costs (mid) | Paying Users to Break-Even |
|-------|-------------------|---------------------------|
| Launch (Month 1-6) | ~$120/mo | **~24 paying users** |
| Growth (Month 7-12) | ~$630/mo | **~127 paying users** |
| Scale (Y2, with contractor) | ~$6,200/mo | **~1,022 paying users** (using Y2 margin $6.09) |

**Reality check vs. base scenario:**
- Month 3 base: 110 paying → covers Launch-Phase fixed costs **4.5x over**
- Month 6 base: 320 paying → covers Growth-Phase fixed costs **2.5x over**
- Month 12 base: 850 paying → covers projected Y2 Scale-Phase fixed costs **0.83x** — meaning Y2 scale is NOT yet self-funding at base Month 12 trajectory; need to grow further before adding contractor/DPO

### Cash Flow Break-Even (including 100% reinvestment + zero salary)

Under founder's stated policy (Months 1-6, $0 salary, 100% reinvest):
- **Cash-flow break-even = when MRR covers (fixed costs + reinvestment commitments)**
- Months 1-3: trivially covered (fixed <$150, reinvestment = whatever's left)
- Months 4-6: covered, as reinvestment is a residual not a fixed obligation
- This is the **operational break-even** — every month is structurally cash-positive at the entity level, by design

### True Profitability Break-Even (founder taking $2,500/mo salary)

Required Net MRR = $2,500 salary + $630 fixed (Growth phase) + $500 reinvestment buffer = **$3,630/mo Net MRR**

Converting Net MRR → Gross MRR (Y1, 30% Apple cut): $3,630 / 0.70 = **$5,186 Gross MRR**

- ARR run-rate: **~$62K ARR**
- Paying users to hit: $5,186 / $7.43 blended gross = **~698 paying users**
- **Expected timing (base scenario):** Month 10-11 (paying users curve hits 700 between Month 10 [median ~700] and Month 12 [850])

### True Profitability Break-Even (Y2 with full stack: contractor + bookkeeping + DPO + $5K founder salary)

Required Net MRR = $5,000 salary + $6,200 fixed (Scale phase) + $2,000 reinvestment + $500 buffer = **$13,700/mo Net MRR**

Converting (Y2, 15% SBP cut): $13,700 / 0.85 = **$16,118 Gross MRR**

- ARR run-rate: **~$193K ARR**
- Paying users (Y2 blended gross $8.99/mo with same tier mix at 85% take): **~1,793 paying users**
- **Expected timing:** Mid-to-late Y2 (Month 18-22) per base trajectory extrapolation

---

## Cost Risks & Surprises

### High-Risk Cost Items

1. **LLM API runaway** — heavy users brain-dumping 20+ times/mo could hit $1-5/user/mo
   - Mitigation: rate-limit (soft 20 sessions/mo), cache common patterns, prompt optimization, on-device inference for iOS 27+ post-WWDC
2. **Apple/Google fee 30% if SBP not granted Year 1** — net revenue per user drops 21% (material to reinvestment compounding speed per business-model.md)
   - Mitigation: apply to Apple SBP via App Store Connect Day 1 / Week 2 of submission
3. **Refund rate >5%** — 30-day no-Q refunds processed instantly; Inflow precedent shows ~5-8% effective refund/dispute rate is realistic for category
   - Mitigation: sessions-gated annual refund (<10 sessions in 30 days), tight onboarding quality, honest day-12 emails
4. **Google OAuth Tier 1 review delay (3-4 weeks)** — could delay launch
   - Mitigation: submit day 1 of testing; manual `.ics` import fallback per business-model.md
5. **Legal cost ballooning** — $500-1,200 template approach assumes founder-discipline on marketing copy; if "treats ADHD" language slips, FTC/FDA exposure could trigger $10K+ remediation
   - Mitigation: written Marketing Language Policy + brand-book regulatory red-lines (~$0-200 one-time, highest leverage)

### Medium-Risk Cost Items

6. **WA MHMDA private right of action** — single plaintiff suit could cost $25K-100K in defense, even if defensible
   - Mitigation: get separate Health Data Privacy Policy + separate collection/sharing consent flows correct at launch (already budgeted in pre-launch legal)
7. **Apple App Store rejection on health categorization** — if reviewer flags as Health & Fitness, triggers March 2026 medical device declaration
   - Mitigation: categorize as Productivity, document decision, avoid medical-treatment copy in description
8. **LLM provider price increase** — OpenAI/Anthropic have raised prices before; ~20-50% spike not impossible
   - Mitigation: provider-agnostic API abstraction layer (already in business-model.md dependencies)
9. **Cash flow lag** — Apple/Google hold 30-45 days + 30-day refund window = 60-day working capital gap from subscription start
   - Mitigation: maintain $500-1,500 buffer in operating account; don't reinvest most-recent month's revenue

### Low-Risk / Predictable

- Apple/Google developer fees ($99 + $25)
- Backend hosting (Supabase scales gracefully, transparent pricing)
- Email service (ConvertKit/Resend transparent tier pricing)
- Push notifications (OneSignal free tier robust)
- Domain + Workspace

### Hidden Costs to Plan For

- **Founder time burn** (not in dollars but real) — track hours/week; at 60+ hr/wk for 6+ months, burnout risk = existential
- **Customer service load at scale** — at 1K+ paid users, "talk to founder" becomes 4-8 hr/day per business-model.md scaling triggers
- **Bad-actor refund chargebacks** (Apple Disputes — uncommon but possible)
- **App Store review delays** (sometimes 7-14 days for updates, especially health-adjacent apps)
- **LLM provider rate limits** → may force paid tier earlier than expected
- **Founder personal runway exhaustion** — no model buffer for medical emergency / Israeli reservist call-up (per business-model.md yellow flag #9)

---

## Cost Optimization Levers

### Pre-Launch
- Use **free tiers everywhere possible** (Supabase, Firebase, OneSignal, Mixpanel, Sentry, RevenueCat <$2.5K MTR)
- **DIY design** (founder produces brand assets)
- **DIY copy** (founder voice = brand voice = ADHD-native authenticity)
- **DIY ASO** (plus optional $99 keyword tool for one-off research)
- **Template-first legal** + light lawyer review (vs $5K-15K full bespoke per regulatory.md)
- **Written Marketing Language Policy** as $0 highest-leverage regulatory control

### Post-Launch (Month 1-6)
- **Apply to Apple Small Business Program Day 1** of App Store Connect submission (15% vs 30% from approval; +21% net revenue per user impact)
- **LLM prompt optimization** — cache common parsing patterns; estimated 20-40% cost reduction
- **Heavy-user soft rate-limit** at 20 voice sessions/mo to cap LLM exposure
- **Vercel/Supabase auto-scaling** — no over-provision
- **Provider-agnostic LLM abstraction** for competitive pricing

### Scale (Y2)
- Move from ConvertKit → Loops or Resend if cheaper at scale
- Negotiate **LLM enterprise rates** (>$1K/mo OpenAI usage opens commercial terms)
- **Reserved instances** for backend (10-20% savings)
- **On-device LLM inference** for iOS 27+ post-WWDC (zero marginal cost for some flows)
- **Discord community @ $2K MRR** reduces 1:1 founder support load (per business-model.md scaling triggers)

---

## Comparison vs Competitors (Cost Structure)

| Cost Item | Tiimo | Motion | Sunsama | Inflow | Planny |
|-----------|-------|--------|---------|--------|--------|
| Team size | ~15 | ~50 | ~5 | ~15 | 1 |
| Estimated burn/mo | $200K+ | $1M+ | $50K | $200K+ | <$1K (Y1) |
| Pricing | $7.99-12/mo | $19-34/mo | $20-25/mo | $47.99/mo | $5-9.99/mo (effective) |
| Strategy | VC-burn | VC-burn | Bootstrapped | VC-burn | Bootstrap reinvest |
| LTV / CAC structural | Premium product, paid creator | High CAC, high price | Low burn, organic | Burned-out brand | Niche organic + 1 creator hero |
| Y1 ARR target | n/a (mature) | n/a (mature) | ~$1.5M (mature) | growth-grade | $28-53K base |

**Planny's cost discipline is its structural advantage.** Inflow's $11M VC didn't translate to product velocity better than what Planny can do with $1,500 seed + reinvestment, *if* Planny focuses on the right wedges (weekly cadence, late-dx women, ADHD-native voice). The asymmetric bet: Inflow's $30+ paid CAC is Planny's organic CAC ceiling — Planny structurally wins the unit economics game from day 1.

---

## Strategic Connections
- ראה `revenue-model.md` (upcoming) ל-revenue projections by tier mix
- ראה `projections.md` (upcoming) ל-3-scenario cash flow detailed
- ראה `02-strategy/business-model.md` ל-unit economics + LTV/CAC + scenarios source
- ראה `02-strategy/go-to-market.md` (upcoming) ל-channel allocation detail
- ראה `01-discovery/raw/regulatory.md` ל-compliance cost source + risk vectors
- ראה `01-discovery/raw/channels.md` ל-channel CAC modeling source

---

## Sources

### Tier 1 (primary, recent)
- Apple Developer official — Small Business Program (15% under $1M proceeds), App Store Connect pricing
- Google Play official — 15% tier policy, $25 one-time developer fee
- OpenAI API pricing (GPT-4o-mini: $0.15/$0.60 per 1M tokens input/output; Whisper $0.006/min)
- Anthropic API pricing (Claude Haiku reference)
- Supabase pricing page (Free → Pro $25 → Team)
- RevenueCat pricing (free <$2.5K MTR)
- AppTweak 2026 — iOS CPI productivity NA $2.84
- FDA 2026 General Wellness guidance (compliance scope)
- WA RCW 19.373 (MHMDA penalty structure: $7,500/violation + private right of action)
- FTC HBNR final rule (April 2024) — $51,744/violation
- Library of Congress — Israel Amendment 13 (DPO threshold + ISS)

### Tier 2 (specialized industry, useful)
- RevenueCat State of Subscription Apps 2026 (productivity LTV benchmark $46.97)
- Adapty State of In-App Subscriptions 2025-2026
- OneSignal pricing tiers (free <10K subscribers)
- Sentry / Mixpanel / ConvertKit public pricing pages
- IAPP / Cooley — MHMDA implementation cost estimates
- IAPP / Safetica / BigID — Israel Amendment 13 DPO cost ranges ($8K-25K/yr)

### Tier 3 (anecdotal / proxy)
- Indie podcast sponsorship rates (Tracy Otsuka comp range $800-2,500 estimated)
- Fiverr / Upwork — App Store screenshot/video preview production
- iOS contractor market rates (US-based, part-time 20 hr/mo @ $75-150/hr)

---

## Flags

### Red Flags
1. **LLM API cost is the most variable line item** — heavy users could 5x base assumption ($0.20/mo → $1.00+/mo). Without rate-limiting in v1, a single power-user cohort can compress gross margin from 95% to ~85%. **Mitigation: ship soft rate-limit at launch.**
2. **One-time legal cost ($500-1,200 scrappy / $8K-19K full bespoke) is 33-800% of seed budget** — must prioritize template-first approach. Full bespoke compliance is deferred to Y2 post-revenue; Y1 relies on disciplined Marketing Language Policy + template-based MHMDA-compliant Health Data Privacy Policy.
3. **MHMDA private right of action** = single plaintiff suit could cost $25K-100K in defense even if defensible. Get separate Health Data Privacy Policy + separate consent flows right at launch, not later. **This is non-negotiable, not optional.**
4. **Founder salary at $5K MRR halts reinvestment compounding** — if founder takes $2,500/mo from Month 7, reinvestment pool shrinks to $0-500/mo and growth slows materially. Recommend deferring salary to $8-10K MRR if personal runway allows.

### Yellow Flags
1. **Apple/Google fee 30% Y1** limits gross margin headroom; if SBP application denied or delayed, reinvestment compounding slows ~21% per business-model.md sensitivity.
2. **Hebrew RTL ($300-900) + Israel DPO ($8K-25K/yr post-10K users)** adds Y2 cost when Israel launches; budget at $10K-30K incremental Y2 compliance for IL market.
3. **Contractor costs at scale (Y2) increase fixed burn ~5x** ($630/mo Growth phase → $3,800-8,600/mo Scale phase); requires $193K+ ARR to be self-funding with full stack.
4. **Cash flow lag (60-day gap)** between subscription start and "safe" revenue means $500-1,500 operating buffer must be maintained; don't reinvest most-recent month's revenue.
5. **Customer support load** at 1K+ paying users becomes 4-8 hr/day for founder; Discord transition @ $2K MRR helps but doesn't eliminate. Plan for transition cost (Discord setup + community moderation policy + initial seeding).
6. **App Store review delays** for health-adjacent apps can be 7-14 days for updates; cash-flow neutral but feature-velocity costly. Plan release cadence accordingly.
