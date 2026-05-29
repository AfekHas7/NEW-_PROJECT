# Kill Criteria — Planny

**Phase:** Phase 8 — Validation (Kill Criteria)
**Project:** startup-validation (Planny)
**Date:** 2026-05-28
**Confidence:** Overall **Medium-High** — ה-thresholds מבוססים ישירות על benchmarks Tier 1 (RevenueCat, Adapty, AppTweak), על kill criteria שכבר נכתבו ב-`go-to-market.md` ו-`mvp-definition.md`, ועל financial sensitivity מ-`projections.md`. החולשה: D30 retention threshold (5%) הוא best-guess כי אין ADHD-specific public data.

---

## תקציר Kill Criteria

ה-document הזה מגדיר 7 תנאים ספציפיים ומדידים שבהם המייסד מתחייב לעצור / לפבט / להמיט hard kill. **המטרה היא לא לקבל החלטות לחוצות באמצע הסערה** — אלא להחליט מראש, כשהראש קר, איזה signals יעצרו את הפרויקט.

**ההיררכיה:**
- **Existential (Hard Kill):** KC4 (D30 retention <5%) — בלי retention, ה-reinvestment compounding נשבר, ה-model הקפיטליסטי קורס. אין pivot שמציל את זה.
- **Critical (Pause + Evaluate):** KC2 (WWDC Apple commoditization), KC7 (founder pivots לסטארטאפ אחר) — שניהם יכולים להוביל ל-hard kill תלוי באבחנה.
- **High (Pivot or fix):** KC3 (Voice Aha fails), KC5 (Refund rate >25%), KC6 (CAC ceiling breach) — recoverable אם מתערבים מהר.
- **Medium (Recoverable):** KC1 (Pre-launch demand failure) — signal של positioning, לא של business model.

**מתי בודקים:** ה-Time-Based Gates ב-Day 30, 60, 90 הם החובה. KC1 נבדק ב-Week 2 pre-launch. KC2 ב-June 8 (11 ימים). KC4-6 מבוססים על cohort data שמבשיל ב-M2-3. KC7 נבדק בכל Self-Evaluation Day 30/60/90.

**הקווים האדומים שלא זזים:** D30 retention <5% ב-M3 = hard kill. Refund rate >25% ב-M3 = hard kill. WWDC ADHD-aware Apple feature shipped = pause + 48hr decision. **המייסד מתחייב מראש שלא להזיז goalposts כשהכישלון מתקרב.**

---

## 7 Specific Kill / Pivot Criteria

### KC1: Pre-Launch Demand Failure

- **Trigger:** **<30 emails on waitlist** after 2 weeks of distribution (by 2026-06-11), OR **<150 waitlist by end of Week 4** (June 25)
- **Test:** Experiment 1 in validation-playbook.md (waitlist conversion from landing page + organic distribution)
- **Decision:** Pivot positioning (Maya may not resonate; try V1 Working Parents wedge) OR delay launch 2-4 weeks for messaging reset
- **Severity:** Medium — recoverable; signal is positioning/messaging, not business model
- **Linked assumption:** A1, A10, A17, A23
- **Data source:** ConvertKit waitlist counter; UTM source attribution

### KC2: WWDC Apple Scheduler Commoditization

- **Trigger:** Apple announces **ADHD-aware AI scheduler** at WWDC June 8 with 2 of 3 criteria met:
  1. Free + default in iOS 27
  2. Ships within 6 months (not 12-18)
  3. Positioning explicitly mentions ADHD/neurodivergence/executive function
- **Probability:** ~10% (Mayday Labs acquisition Apr 2024 + Personalized Siri delayed Mar 2025)
- **Test:** Watch keynote live June 8; war-room June 8-15 with 48hr decision window
- **Decision:** Pause launch entirely; activate Version C pivot options:
  1. AuDHD niche (Tiimo skews here but no app owns)
  2. Couples Mode primary ("ADHD planner for couples")
  3. B2B for ADHD coaches (3-5K coaches force-multiplier)
  4. Perimenopausal-ADHD women 38-44 (94% report worsening symptoms)
- **Severity:** Critical — depends on Apple's exact features; if "good enough" generic AI scheduler only (1 of 3 criteria), Version B (reposition as "ADHD layer over Apple Intelligence") instead of Hard Kill
- **Linked assumption:** A13

### KC3: Voice Aha Moment Failure

- **Trigger:** TestFlight beta (Week 3-4) cohort shows:
  - **<40% complete voice brain-dump** in first session, OR
  - **Median time-to-first-plan >120 seconds** (target ≤75s, public promise <90s)
- **Test:** TestFlight closed beta with 50-100 users from waitlist; in-app instrumentation
- **Decision:** Onboarding flow rework before public launch (delay 1-2 weeks); evaluate text-first variant with voice as power-user feature
- **Severity:** High — must be fixed before launch; existential if unfixable (entire product hypothesis breaks)
- **Linked assumption:** A2
- **Data source:** TestFlight session analytics + instrumented onboarding events

### KC4: Day-30 Retention Below Existential Floor

- **Trigger:** **Day-30 retention <5%** by Month 3 (3 cohorts of data — June, July, August launch cohorts all matured)
- **Test:** Experiment 11 (Cohort retention analysis) — RevenueCat / Mixpanel D30 tracking
- **Decision:** **HARD KILL or radical pivot** — model is broken. Anti-shame UX did not deliver retention lift vs category baseline. Reinvestment compounding inverts (churn > new revenue).
  - Hard Kill path: refund all annual subs proactively, communicate to waitlist + paying users, document learnings, App Store remove or leave live with disclosure
  - Radical Pivot: V1 Working Parents from `brainstorm.md` (different persona, different retention curve), OR coach B2B (different unit economics)
- **Severity:** **EXISTENTIAL** — no business without retention; this is the single variable that can kill Planny no matter what else succeeds
- **Linked assumption:** A6
- **Benchmark anchor:** Mental health 3.3% D30, Productivity 4.1% D30, Evidence-based health 16% D30; Planny target 12-15%

### KC5: Refund Rate Above 25%

- **Trigger:** **Refund rate >25%** for any cohort by Month 3 (or >15% for 2 consecutive months)
- **Test:** Experiment 10 (Always-on refund tracking) — Apple/Google IAP refund webhooks + manual refund log
- **Decision:** Re-examine onboarding quality, paywall expectations, value proposition mismatch
  - Soft fix attempt: tighten sessions gate (<10 → <5 sessions), shorten refund window (30 → 14 days), improve paywall clarity
  - If after 1 month of fixes refund rate still >20% → kill (brand promise + unit economics both broken)
- **Severity:** High — financial model breaks; brand promise "30-day no-Q refund" becomes expensive liability
- **Linked assumption:** A7, A22
- **Benchmark anchor:** Industry healthy 2-5% refund; Inflow "fuzzy refunds" complaints ~5-8% effective; Planny target <15%

### KC6: CAC Above Affordable Ceiling

- **Trigger:** **Blended CAC >$40** for 2 consecutive months, OR **Apple Search Ads CPA >$15** with no path to <$12 within 30 days
- **Test:** Experiments 8 + 9 (channel CAC tracking) + accumulated launch data via UTM + RevenueCat attribution
- **Decision:**
  - First action: kill paid spend (ASA pause), double down on organic (TikTok + Reddit + creators)
  - Second action: if blended CAC still >$30 after 60 days organic-only → pivot positioning (Maya may not be findable at low CAC) or kill
- **Severity:** Medium-High — unit economics break (LTV $50-65 / CAC >$40 = LTV/CAC <1.5:1, below industry healthy 3:1)
- **Linked assumption:** A18, A1
- **Benchmark anchor:** LTV $50-65 / CAC ceiling $17-22 (3:1 rule); Inflow-poisoned auctions >$30 unsustainable

### KC7: Founder Pivots to Another Startup

- **Trigger:** Founder explicitly says **"I'm focusing on Startup 2 or Startup 3 instead"** in Self-Evaluation Day 30, 60, or 90 — OR founder time allocation drops below **15 hrs/wk for 3 consecutive weeks** without an explicit "vacation/recovery" frame
- **Test:** Self-reported by founder; weekly time tracking; scorecard verdict at Day 30/60/90
- **Decision:** Hand off to advisor / mentor for objective evaluation; or honest kill
  - Pause path: if founder can articulate "I need 2 weeks reset and will return" → ok, document
  - Pivot path: if founder commits to another startup → graceful Planny sunset (refund annual subs, leave App Store live with disclosure)
- **Severity:** Total — no business without founder commitment in solo bootstrap; bigger threat than retention because there's no metric pivot
- **Linked assumption:** A15, A16

---

## Quick Kill Reference Card

| Metric | Hard Kill | Soft Kill (Pivot) | Green |
|--------|-----------|---------------------|-------|
| Waitlist emails (Day 0, 2 weeks pre-launch) | <30 in 2 weeks | 30-150 in 2 weeks | >150 in 2 weeks |
| Voice brain-dump completion (TestFlight) | <40% | 40-60% | >60% |
| Median time-to-first-plan | >120 sec | 90-120 sec | <90 sec |
| Trial-to-paid conversion | <10% | 10-20% | >20% |
| Day-7 retention | <20% | 20-30% | >30% |
| Day-30 retention | <5% | 5-10% | >10% |
| Refund rate | >25% | 15-25% | <15% |
| Blended CAC | >$40 | $20-40 | <$20 |
| Apple Search Ads CPA | >$15 | $8-15 | <$8 |
| LLM cost per user / mo | >$0.50 | $0.30-0.50 | <$0.30 |
| Apple WWDC June 8 | ADHD-aware shipped + 2/3 criteria | Generic AI scheduler shipped | None shipped |
| Founder commitment | Pivots away | Distracted but here | Fully focused |
| Paying users Day 90 | <15 | 15-50 (pivot) / 50-100 (extend) | >100 |

---

## Kill Decision Process

### Trigger Detected
1. **Founder confirms with data** (no panic, no anecdote — show the number)
2. **Pause 48 hours** — sometimes signals are noisy; verify with second data pull
3. **Discuss with advisor** (if any) or trusted person who knows the context
4. Apply this decision tree:

```
Is the failure existential (KC4 D30 retention) or recoverable (KC1 waitlist)?
├── Existential → consider hard kill
│   ├── Can radical pivot solve it (different persona, B2B)? → soft kill + pivot
│   └── No clear pivot → hard kill, refund annual subs, document, sunset
└── Recoverable
    ├── Can be fixed in <30 days → fix and re-test
    └── Cannot → pivot OR kill

Is the founder still committed (KC7)?
├── Yes → fight through the recoverable failures
└── No → kill mercifully; do not drag a dying founder through a dying project
```

### Hard Kill Process
1. **Communicate to waitlist + paying users** within 7 days
2. **Refund all annual subs proactively** (not just the unsatisfied ones) — brand goodwill for future ventures
3. **Document learnings** publicly (founder TikTok / Reddit / Twitter — late-dx ADHD community values transparency)
4. **App Store:** leave live with disclosure "no longer actively maintained" OR remove entirely (founder choice)
5. **Move forward** to next venture (Startup 2 or 3 from comparison)
6. **Time budget for sunset: ≤2 weeks**, not 2 months

### Pivot Process
1. **Re-examine `brainstorm.md`** alternative variations (V1 Working Parents, V5 Shift Workers, AuDHD, Couples Mode, Coach B2B)
2. **Re-run Phase 4-7 lightweight** with pivoted assumption (focus on positioning + GTM + unit economics; keep MVP architecture)
3. **Re-launch with explicit new positioning** within 30-45 days; communicate change to existing users transparently
4. **Maximum 1 pivot per 6 months** — beyond that, hard kill (signal that founder is searching for product-market fit in wrong space)

---

## Time-Based Decision Gates

### Day 14 Pre-Launch (June 11)
- Waitlist: **<30** → KC1 hard kill territory; **30-150** → KC1 soft kill (delay + reposition); **>150** → proceed
- Tracy Otsuka response: no response → activate Kristen Carder fallback
- WWDC scenario A/B/C plans: locked in writing

### Day 30 Post-Launch (~July 22)
- Cumulative paying users: **<15** → Hard Kill territory (extreme low signal)
- Day-7 retention: **<25%** → Investigate (onboarding leak)
- Voice brain-dump completion: **<50%** → Onboarding intervention urgent
- Refund rate: **>20%** → Investigate refund reasons via exit survey
- Founder energy/commitment: low → Burnout risk flag; advisor check-in
- ASA CPA: **>$15** with no improving trend → pause spend, reallocate

### Day 60 Post-Launch (~August 22)
- Cumulative paying users: **<50** → Soft Kill (consider pivot to V1 Working Parents)
- Refund rate: **>20%** → Examine onboarding + paywall expectations
- CAC trending up → Adjust channel mix toward organic
- LLM cost trending **>$0.40/user** → Implement caching + rate limits before M3
- Tracy Otsuka episode (if booked): aired with <10 paying users attributable → high-leverage channel failure signal

### Day 90 Post-Launch (~September 22)
- Day-30 retention cohort 1: **<5%** → **HARD KILL** (KC4 triggered)
- Day-30 retention cohort 1: **5-8%** → Soft Kill (retention engineering sprint 30 days, pause acquisition)
- 30-100 paying users + retention 5-10% → **Pivot to V1 Working Parents** OR pause for 30-day retention sprint
- 100+ paying users + retention 10%+ → **GREEN**, continue per `business-model.md` Base scenario at higher cadence
- Refund rate >15% → Investigate; if root cause unfixable in 30 days → consider kill

### Month 6 Post-Launch (~November 22)
- Full cohort retention: needs to be **8%+ for sustainable** reinvestment compounding
- Net MRR: **$1,500+** for runway sustainability (Conservative scenario floor)
- Cash position: **positive cumulative** (Base) or **>-$1,200** (Pessimistic decision gate)
- Founder personal runway: remaining ≥6 months OR salary trigger crossed
- If cumulative cash <-$1,500 AND no clear path to $2K MRR by M9 → activate pessimistic decision gate (pivot / bridge / sunset)

### Month 12 Post-Launch (~May 27)
- Net MRR: $4K+ (Base) for Y2 continuation
- ARR run-rate: $50K+ for funding optionality
- Founder salary: triggered if $5K MRR crossed (M8 base case)
- Y2 plan committed: Android + Hebrew RTL + partner mode v1.1

---

## Founder Pre-Commit Statement

The founder commits to honoring these kill criteria. This is signed (mentally) before launch — written here for accountability.

**Acknowledged risks:**
1. The data may tell me to stop. I will believe the data over my own hope.
2. I may have to refund all paid users proactively. I will do it within 7 days of a hard kill decision.
3. My identity isn't tied to Planny succeeding. I am a founder who runs experiments — one is Planny.
4. There are 2 other startups I can pivot to. The opportunity cost of staying with Planny when data says stop is real.
5. WWDC June 8 is outside my control. I will not lose 6 months to a fight I cannot win.

**Promise to self:**
- I will **check the data weekly** (Monday review aligned with `assumptions-tracker.md`)
- I will **not move the goalposts** when failure is imminent (no "let's wait one more month" past the gates above)
- I will **tell my friends/advisors honestly** when it's not working, not when it's already dead
- I will **sleep on hard decisions (48 hours minimum)** but not **procrastinate** — pause ≠ avoidance
- I will **refund users mercifully** if I kill, not protect runway over relationships
- I will **document publicly** (build in public ethos) — late-dx ADHD community values honest founders, and the next venture benefits from it

**Anti-commitments (things I will NOT do):**
- I will not raise emergency capital from family/friends to prolong a project the data says is dead
- I will not silently downsize and "soft" continue while telling myself I'm still launched
- I will not delete the app + ghost the users
- I will not blame the market, Apple, or competitors for a retention failure that is a product failure

---

## Strategic Connections
- ראה `assumptions-tracker.md` ל-25 assumptions שמהן נגזרו ה-kill criteria
- ראה `risk-analysis.md` ל-priority risks ול-likelihood × impact matrix (when written)
- ראה `validation-playbook.md` ל-experiments concrete שבודקים כל kill criterion (when written)
- ראה `scorecard.md` ל-overall verdict שמשקלל את כל הסיגנלים יחד (when written)
- ראה `../00-intake/brief.md` — founder's softer original exit criterion (100 paying / 30-50 acceptable); ה-doc הזה הוא ה-formalization שלו
- ראה `../02-strategy/go-to-market.md` §Kill Criteria @ Day 90 — source ל-KC1, KC3, KC4, KC6
- ראה `../04-product/mvp-definition.md` §Failure Criteria — source ל-KC3, KC4, KC5
- ראה `../05-financial/projections.md` §Pessimistic Scenario — source ל-Month 6 decision gate

---

## Sources

### Phase 1 (Intake)
- `/home/user/NEW-_PROJECT/startup-validation/00-intake/brief.md` — founder's original soft exit criterion (100 paying / 30-50 acceptable / minimum 15)

### Phase 4 (Strategy)
- `/home/user/NEW-_PROJECT/startup-validation/02-strategy/go-to-market.md` §Kill Criteria @ Day 90 (lines 577-597)
- `/home/user/NEW-_PROJECT/startup-validation/02-strategy/business-model.md` §Sensitivity Analysis + §Pessimistic Scenarios

### Phase 6 (Product)
- `/home/user/NEW-_PROJECT/startup-validation/04-product/mvp-definition.md` §Failure Criteria (Kill Switches), §Success Criteria thresholds

### Phase 7 (Financial)
- `/home/user/NEW-_PROJECT/startup-validation/05-financial/projections.md` §PESSIMISTIC Scenario (Month 6 decision gate), §Sensitivity Visualizations

### External benchmarks
- RevenueCat State of Subscription Apps 2026 — D30 retention by category (productivity 4.1%, mental health 3.3%, evidence-based health 16%); refund rates 2-5% healthy
- Adapty State of In-App Subscriptions 2026 — trial-to-paid 18-25% opt-in CC
- AppTweak Apple Ads Benchmarks 2025 — productivity CPA $2.84 (+90% YoY)
- ChoosingTherapy 2025 Inflow review — billing reputation / refund complaints pattern

---

## Flags

### Red Flags

- **KC4 (D30 retention) is the only truly EXISTENTIAL kill** — the others are recoverable with intervention. KC4 is structural: if the product doesn't retain ADHD users beyond Day 30, no marketing channel, pricing tier, or feature add saves it
- **KC7 (founder commitment) is high probability** given the 3-startup comparison context — this is not a hypothetical risk, this is the explicit framing of the project. The founder must be especially honest with themselves at Day 30
- **KC2 (WWDC) is binary and uncontrollable** — 11 days from now we know. Version C readiness must be locked in writing before June 8, not improvised on June 9
- **No single advisor / accountability partner identified** to enforce kill criteria — founder is judge, jury, and executioner. Recommend nominating one external person (mentor, founder peer, partner) before launch

### Yellow Flags

- **Time-based gates (Day 30/60/90) require founder discipline** to honor without "just one more month" rationalization. The Pre-Commit Statement above is the mitigation, but it's not enforceable
- **Refund + CAC + retention often compound** — multi-metric failure more likely than single-metric. A 3-metric soft warning may equal a 1-metric hard trigger; founder should not wait for the loudest signal
- **D30 retention threshold of 5% is best-guess** — no ADHD-specific public cohort data exists. Real threshold could be 4% (productivity baseline) or 7% (mid-point of mental-health + productivity). Recommend re-calibrating after M2 data
- **Hard kill is psychologically expensive** — solo founder, $1,500 sunk, US trip planned around launch, public ADHD disclosure already made. The criteria above must be honored regardless of these sunk costs
- **Pivot options (V1 Working Parents, AuDHD, Coach B2B) are themselves untested** — pivoting to a new persona doesn't guarantee that persona is more validated than Maya was. Pivot is not a magic word; new pivot = new Phase 4-7 lightweight
- **30-day "wait and verify" period within KC processes** means a slow kill in some scenarios (e.g., retention <5% at M3 + 1 month verify = M4 final call) — founder must accept that this is a feature not a bug
