# Assumptions Tracker — Planny

**Phase:** Phase 8 — Validation (Assumptions)
**Project:** startup-validation (Planny)
**Date:** 2026-05-28
**Confidence:** Overall **Medium** — היקף נרחב של assumptions (25) המתורגמות ישירות מ-Phase 1-7 (intake, discovery, strategy, brand, product, financial); רובן עדיין untested ב-real customer behavior. רמת ביטחון של כל assumption בודדת מצוינת בטבלה.

---

## תקציר

ה-tracker הזה מתעד את 25 ה-assumptions הקריטיות שעליהן Planny נשענת. כל assumption נגזר ישירות מ-deliverable של Phase 1-7 (intake.md, target-audience.md, positioning.md, value-proposition.md, business-model.md, go-to-market.md, mvp-definition.md, projections.md). המטרה: להפוך כל הנחה סמויה ל-testable claim עם confidence level, test plan, עלות, חלון זמן ו-failure implication ברורים.

**ההיררכיה:** Critical (existential אם נכשל — A6, A13, A16) → High (פוגע ב-unit economics או אסטרטגיה — A1, A2, A3, A4, A5, A11, A12) → Medium (מעוות תכנון, לא הורג — A7-A10, A14-A22) → Continuous Monitor (A19, A14, A15, A22).

**איך משתמשים:** עדכון שבועי (Monday review), שינוי confidence level כש-evidence נכנס, trigger ל-`kill-criteria.md` כשמספר Critical assumptions מתערערים. ה-tracker מתחבר ישירות ל-`validation-playbook.md` (experiments) ול-`risk-analysis.md` (priority risks).

**שורה תחתונה ל-launch:** 4 assumptions חייבים אימות ב-2 שבועות לפני launch (A8 Tracy, A10 Reddit, A13 WWDC, A9 micro-creators). 6 assumptions ייכנסו ל-test בחודש launch. 4 קריטיים בלבד ב-Day 30/60/90 cohort analysis. השאר — continuous monitoring.

---

## Assumption Inventory

| # | Assumption | Category | Confidence Now | Status | How to Test | Test Cost | Test Timeline | Failure Implication |
|---|------------|----------|----------------|--------|-------------|-----------|----------------|---------------------|
| A1 | Late-diagnosed US women 25-40 ("Maya") are the right beachhead vs broader ADHD adults | Customer | Medium | Untested | Waitlist demographics + 10 customer interviews (US trip) + first 100 paying user analysis | $0 | 2-3 weeks (waitlist) + 60 days (paying cohort) | Persona zone shift to V1 Working Parents or AuDHD; positioning rewrite |
| A2 | Voice brain-dump <90s is the Aha moment (≥70% complete in first session) | Product | Medium | Untested | TestFlight closed beta with 50-100 waitlist users, time-to-first-plan instrumentation | $0 | 3-4 weeks (TestFlight) | Onboarding rework before public launch; possibly text-first variant |
| A3 | Maya willing to pay $9.99/mo or $59.99/yr (parity with Numo, below Inflow) | Pricing | Medium | Untested | Pricing screen test in beta + waitlist conversion @ early-bird $39 | $0 | 4-6 weeks | Tier restructure; consider $7.99/mo or freemium with hard limits |
| A4 | 14-day annual-only opt-in CC trial converts ≥25% trial-to-paid | Conversion | Medium | Untested | Real launch cohort data (week 5-9 conversion); paywall A/B test from M2 | $0 | 6-8 weeks | Trial structure change (longer trial / opt-out / no-CC option for gifted) |
| A5 | Two-way Google Calendar + Apple EventKit sync is THE technical moat vs Tiimo | Differentiation | Medium-High | Untested | Customer feedback Day 30, % of users connecting both calendars, NPS verbatims | $0 | 8-10 weeks | Wedge re-examination; lean harder on voice + ADHD UX as moat |
| A6 | Day-30 retention ≥10-15% achievable with anti-shame UX (vs 4.1% productivity benchmark) | Retention | Low-Medium | Untested | Cohort analysis Day 30, 3 cohorts deep by Month 3 | $0 | 8-12 weeks | **EXISTENTIAL** — reinvestment compounding breaks; kill or radical pivot |
| A7 | Refund rate <15% sustainable with sessions-gated <10 refund policy | Brand promise | Medium | Untested | Monitor refunds from M1; trigger review @ M3 | $0 | 12 weeks | Brand promise expensive; tighten sessions gate or shorten refund window |
| A8 | Tracy Otsuka podcast slot bookable for ≤$1,500 cash + affiliate (vs $6K-9K rack) | Distribution | Low | Untested | Email outreach Day 1 + Loom + audio sample | $0 | 2-3 weeks | Pivot to Kristen Carder ($800-1,200) + ADDitude paid slot + micro-creator triple-down |
| A9 | 30-50 ADHD micro-creators (10K-100K) will accept free annual subs in exchange for honest posts | Distribution | Medium | Untested | DM outreach to 80 creators Week 1-2 | $0 | 2-3 weeks | Replace gifting with $200-400 paid placements; shrink to 10-15 creators |
| A10 | r/ADHDWomen (700K members) allows founder organic presence and AMA per mod rules | Distribution | Medium | Untested | Read subreddit rules + modmail Week 1; 4-week comment karma build | $0 | 1 day rules check; 4-6 weeks karma | Reddit-out distribution; reweight to Facebook ADHD groups + Discord servers |
| A11 | Apple Small Business Program eligibility granted within 30 days of submission | Cost | High | Untested | Apply via App Store Connect Week 1 of submission | $0 | 2-4 weeks | Y1 net margin -21%; Y2 ARR projection $191K → $158K |
| A12 | Google Calendar OAuth sensitive scope verification approved within 4-6 weeks | Product/Compliance | Medium | Untested | Submit Day 1; manual `.ics` import fallback prepared | $0 | 4-8 weeks | Launch delay OR ship v0.9 with Apple-only + manual import; F3 update 2 weeks post-approval |
| A13 | Apple WWDC June 8 does NOT ship ADHD-aware AI scheduler (Likelihood ~10%) | Market | Medium | Untested | Watch keynote live June 8; war-room June 8-15 | $0 | 11 days | Pause launch; activate Version C repositioning (AuDHD / couples / coach B2B / perimenopausal) |
| A14 | LLM cost ≤$0.30/active user/mo at scale (Apple Speech + GPT-4o-mini hybrid) | Cost | Medium-High | Untested | Monitor cost/user weekly from first 100 users; usage analytics | $0 | 8 weeks | Pricing increase OR rate-limit power users OR add $14.99 power tier |
| A15 | Founder maintains 25-30 hrs/wk pace for 12 months without burnout | Team | Medium | Untested | Self-track weekly hours + energy scoring; advisor check-in monthly | $0 | Ongoing | Burnout → product velocity collapses → kill or hand off |
| A16 | Founder commits to Planny over the 2 other startups under comparison | Team | Medium | Untested | Self-evaluation Day 30, 60, 90 + scorecard.md verdict | $0 | 4 weeks (initial), ongoing | **EXISTENTIAL** — founder pivots, project ends |
| A17 | TikTok organic content (founder POV, 5 posts/week) reaches Maya at sufficient scale | Distribution | Medium | Untested | First 10 posts analytics (views, follows, profile clicks); algorithm warm-up by post 30-50 | $0 | 2-4 weeks | Channel reweight to Pinterest + IG Reels cross-post + heavier Reddit |
| A18 | Apple Search Ads CPA ≤$15 in productivity category on long-tail ADHD keywords | CAC | Medium-High | Untested | $200-400 test spend over 14 days; CPT cap $1.50 | $200-400 | 2-3 weeks | Paid spend reduced to brand-defensive only; shift to creator gifting |
| A19 | Inflow / Saner.AI / Indy by Shimmer / Tiimo do NOT catch up technically in 6 months (no two-way sync, no late-dx women positioning) | Competitive | Medium | Untested | Quarterly competitive review; weekly release-note monitoring | $0 | Ongoing | Pivot wedges; lean harder on founder-credential + brand voice |
| A20 | iOS-only launch acceptable — Android skip in M1-3 doesn't lock out >40% of Maya | Product | Medium | Untested | Watch Android waitlist requests + Maya demographic (US women 25-40 iPhone share ~75%) | $0 | Ongoing | Android timeline accelerated from M4 → M2 |
| A21 | Maya has Google Calendar (Workspace) OR Apple Calendar (personal) — not just paper/Reminders | Product | Medium-High | Untested | Survey early users (waitlist + first 100); calendar connection rate Day 7 | $0 | 4-6 weeks | Apple-only build acceptable; or build manual entry path for non-calendar users |
| A22 | Refund processing <48hr sustainable at scale (founder-managed via RevenueCat + Apple) | Operations | Medium | Untested | Track refund response time from M1; trigger @ M3 review | $0 | 6-8 weeks | Slower refunds, brand impact, possibly automate via RevenueCat webhooks earlier |
| A23 | Founder ADHD disclosure delivers measurable trust signal (≥50% of new sign-ups cite founder/built-by-ADHD) | Brand | Medium-High | Untested | Onboarding survey question + Reddit comment sentiment analysis + DM volume | $0 | 4 weeks | Reposition founder voice volume; lean on Maya quotes + clinician advisor instead |
| A24 | Tracy Otsuka / How to ADHD / Sunsama / Kristen Carder partnerships not exclusively locked | Distribution | Medium | Untested | Outreach + check existing sponsorship terms publicly | $0 | 2-4 weeks | Find alternative pods (William Curb, Katy Weber, Tamara Rosier guest spots) |
| A25 | Pricing whitespace at $7-10/mo confirmed by Maya behavior (no race to free, no resistance to $9.99) | Pricing | High | Untested | Conversion rate by tier monthly; cohort price-elasticity check at M2-3 | $0 | 8-12 weeks | Price up to $11.99 OR down to $7.99 based on signal |

---

## Confidence Levels

- **High (data-backed or near-certain):** A11 (Apple SBP eligibility known criteria), A25 (pricing whitespace confirmed by Numo $59.99 + Tiimo $54 anchors)
- **Medium-High:** A5 (two-way sync wedge documented per Tiimo Nolt #1 request), A14 (LLM benchmarks known), A18 (AppTweak data Tier 1), A21 (US Maya demographic), A23 (Reddit ADHD founder threads pattern)
- **Medium:** A1, A2, A3, A4, A7, A9, A10, A12, A13, A17, A19, A20, A22, A24
- **Medium-Low:** A6 (D30 retention — no ADHD-specific public data; existential), A15, A16
- **Low:** A8 (Tracy Otsuka indie rate unconfirmed; rack rate 4x budget)

---

## Priority Testing Order

### Test in Next 2 Weeks (Pre-Launch — through 2026-06-11)
1. **A8 (Tracy outreach)** — Email Day 1 (today); decision rule "if no response by Week 3 → activate fallback"
2. **A10 (Reddit r/ADHDWomen rules)** — 30-min subreddit rules check + modmail Week 1
3. **A13 (WWDC June 8)** — 11 days; war-room scenario plans A/B/C locked
4. **A9 (Micro-creator outreach)** — 80 DMs sent Week 1-2, track 25-35 acceptance
5. **A24 (Partnership exclusivity check)** — Public review of How to ADHD × Sunsama sponsorship; alternative pods identified

### Test During Launch Month (M1, June 22 - July 22)
6. **A2 (Voice Aha)** — TestFlight beta instrumentation Week 3-4; time-to-first-plan median, completion %
7. **A12 (Google OAuth approval)** — Submit Day 1; track Google review queue weekly
8. **A11 (Apple SBP submission)** — Apply Week 2 of App Store submission
9. **A17 (TikTok organic reach)** — Post analytics from post 1; warm-up by post 30
10. **A18 (Apple Search Ads CPI)** — $50/day test from launch Day +4
11. **A21 (Maya calendar mix)** — Onboarding survey + connection rate Day 7

### Test in Month 2-3 (July - September)
12. **A1 (Persona-fit)** — Demographics of first 100 paying users + 10 in-person US trip interviews
13. **A3 (Pricing acceptance)** — Tier mix analysis by Day 60
14. **A4 (Trial-to-paid conversion)** — First full 14-day trial cohort matures end of M2
15. **A6 (D30 retention)** — Cohort 1 matures end of M2; trigger review
16. **A7 (Refund rate)** — Accumulated 30-day refund window data
17. **A14 (LLM cost/user)** — Monthly cost/active-user calculation
18. **A22 (Refund processing time)** — Tracking from M1; baseline established M3
19. **A23 (Founder ADHD trust signal)** — Onboarding survey aggregate analysis
20. **A25 (Pricing whitespace confirmation)** — Tier conversion rate analysis

### Test Continuous (Ongoing Monitor)
- **A5** (Two-way sync moat — verbatim feedback + competitor watch)
- **A15** (Founder pace — weekly self-check)
- **A16** (Founder commitment — Day 30/60/90 self-evaluation)
- **A19** (Competitive landscape — quarterly review)
- **A20** (iOS-only acceptability — Android waitlist requests)

---

## How to Use This Tracker

1. **Update status every Monday** — what was tested last week, what was learned, what was inconclusive
2. **Refresh confidence levels** as evidence accumulates (Untested → Partial → Validated / Invalidated)
3. **Flag changes** in confidence to founder personal log + advisor (if any) within 24hr of evidence
4. **Trigger `kill-criteria.md` review** if 2+ Critical assumptions (A6, A13, A16) invalidate, or any 3 High-priority assumptions invalidate simultaneously
5. **Re-score** in `scorecard.md` at Day 30, Day 60, Day 90 with updated confidence levels

### Status taxonomy
- **Untested** — no evidence yet
- **Partial** — one signal in, awaiting more
- **Validated** — evidence supports assumption
- **Invalidated** — evidence contradicts; action required
- **Continuous** — ongoing monitor, no terminal state

---

## Strategic Connections
- ראה `validation-playbook.md` ל-experiments concrete לכל assumption (when written)
- ראה `risk-analysis.md` ל-risk matrix וקישור assumptions ↔ risks (when written)
- ראה `kill-criteria.md` ל-decision thresholds כאשר assumptions נשברים
- ראה `scorecard.md` ל-final score משולב של כל הוולידציה (when written)
- ראה `../00-intake/brief.md` ל-source intake assumptions
- ראה `../01-discovery/target-audience.md` ל-Maya persona ו-A1 source
- ראה `../02-strategy/business-model.md` ל-A3, A4, A6, A7, A11, A14, A25 sources
- ראה `../02-strategy/go-to-market.md` ל-A8, A9, A10, A17, A18, A24 sources
- ראה `../04-product/mvp-definition.md` ל-A2, A5, A12, A20, A21 sources
- ראה `../05-financial/projections.md` ל-A6, A11, A14, A22 sources

---

## Sources

### Phase 1 (Intake)
- `/home/user/NEW-_PROJECT/startup-validation/00-intake/brief.md` — founder reinvestment policy, US trip context, ADHD disclosure decision, $1,500 seed

### Phase 3 (Discovery)
- `/home/user/NEW-_PROJECT/startup-validation/01-discovery/target-audience.md` — Maya persona (A1, A21), pain hierarchy (A2, A6, A7)
- `/home/user/NEW-_PROJECT/startup-validation/01-discovery/competitor-landscape.md` — Tiimo Nolt feature gap (A5), Inflow billing reputation (A7), competitor catch-up (A19)
- `/home/user/NEW-_PROJECT/startup-validation/01-discovery/market-analysis.md` — WWDC platform risk (A13)

### Phase 4 (Strategy)
- `/home/user/NEW-_PROJECT/startup-validation/02-strategy/business-model.md` — pricing tiers (A3, A25), trial conversion benchmarks (A4), D30 retention sensitivity (A6), refund rate (A7), SBP economics (A11), LLM cost (A14), CAC targets (A18)
- `/home/user/NEW-_PROJECT/startup-validation/02-strategy/go-to-market.md` — Tracy Otsuka outreach (A8), micro-creator program (A9), r/ADHDWomen approach (A10), TikTok cadence (A17), ASA spend plan (A18), partnership exclusivity (A24), founder time allocation (A15)
- `/home/user/NEW-_PROJECT/startup-validation/02-strategy/positioning.md` — founder ADHD disclosure trust signal (A23), two-way sync moat (A5)

### Phase 6 (Product)
- `/home/user/NEW-_PROJECT/startup-validation/04-product/mvp-definition.md` — voice Aha (A2), Google OAuth timeline (A12), iOS-only decision (A20), calendar dependencies (A21), LLM cost monitoring (A14)

### Phase 7 (Financial)
- `/home/user/NEW-_PROJECT/startup-validation/05-financial/projections.md` — D30 retention as #1 unknown (A6), Apple SBP economics (A11), LLM cost spike sensitivity (A14), refund operational cost (A22), trial conversion sensitivity (A4)

### External benchmarks
- RevenueCat State of Subscription Apps 2026 (A4, A6, A7, A25)
- Adapty State of In-App Subscriptions 2026 (A4)
- AppTweak Apple Ads Benchmarks 2025 (A18)
- ChoosingTherapy 2025 Inflow review (A7)

---

## Flags

### Red Flags

- **A6 (D30 retention) is existential** — entire business model rests on it. No public ADHD cohort data; first reliable signal Month 2-3. If <6%, `kill-criteria.md` KC4 triggers.
- **A13 (WWDC outcome) is binary external event** — Planny cannot control. 11-day countdown to evidence. Version C pause-and-evaluate readiness mandatory.
- **A16 (founder commitment) is psychological/personal risk** — 3-startup comparison makes pivot probability non-trivial. Scorecard verdict at Day 30 critical.
- **A8 (Tracy Otsuka) is single-point dependency** for highest-leverage Tier-1 channel. Rack rate may be 4x budget. Fallback plan must activate by Week 3 if no response.
- **A12 (Google OAuth) is launch-date blocker** — 2-4 week review queue; if delayed >5 weeks, ship v0.9 without two-way Google sync, which weakens A5 wedge.

### Yellow Flags

- **25 assumptions to track is a lot for solo founder** — recommend bi-weekly review focused on Critical + High Priority only (A1-A14); Continuous Monitor assumptions reviewed monthly
- **Confidence levels are founder-self-assessed** until first cohort data — risk of motivated reasoning. Recommend external advisor review at Day 30
- **No formal "Invalidated" trigger process** — relying on founder discipline to mark assumptions failed before sunk-cost reasoning kicks in. Mitigation: pre-commit to confidence drops in writing
- **Test costs assumed $0 for most** — true for time-only tests, but founder-hour cost is real and finite (25-30 hrs/wk allocation)
- **A6 + A13 + A16 form a Critical cluster** — any 2 invalidating = soft kill territory per `kill-criteria.md`
