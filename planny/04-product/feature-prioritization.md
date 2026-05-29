# Feature Prioritization — Planny

**Phase:** Phase 6 — Product (RICE)
**Project:** startup-validation (Planny)
**Date:** 2026-05-28
**Confidence:** Medium-High — ה-Reach מבוסס על TAM beachhead מתועד ב-`target-audience.md` (Maya persona, US late-dx women 25-40); ה-Impact מבוסס על דירוג pains/gains ב-`value-proposition.md` (Strongest Fit = Impact 3, Important Fit = Impact 2, Differentiating = Impact 1.5, Delighters = Impact 1); ה-Effort מבוסס על אומדן solo vibe-coder עם 90% UI כבר בנוי; ה-Confidence מבוסס על מידת ה-validation ב-customer-voice + competitor-landscape (data-backed = 100%, persona-narrow validated = 80%, gut/speculative = 50%/30%). סיכון עיקרי: WWDC ב-10 ימים יכול לערער את אומדני ה-Effort של F3/F4 ואת ה-Reach של F1 אם Apple Intelligence Calendar שולחת voice-to-schedule native.

---

## תקציר

ה-RICE prioritization של Planny לוקח 30 פיצ'רים (v1.0 must-haves, v1.1 nice-to-haves, v1.2 deferred, v2.0 expansion) ומדרג אותם ב-(Reach × Impact × Confidence) / Effort כדי לקבל **build order** שמשרת שני יעדים בו-זמנית: (א) הגעה ל-launch ב-9 ביוני (post-WWDC) עם MVP שמכבד את ה-three wedges שאומתו ב-`value-proposition.md` — two-way calendar sync (anti-Tiimo), 60-second voice brain-dump (Aha moment), ו-refund/trust UX (anti-Inflow); (ב) שמירה על runway של פאונדר סולו כך שהבחירה היא לא "מה הכי חשוב" אלא **"מה הכי חשוב חלקי כמה זמן זה לוקח."**

הציון מודיע על ה-leverage היחסי של כל פיצ'ר. הניצחונות הגדולים ביותר הם פיצ'רים עם **Effort נמוך מאוד + Reach גבוה + Confidence גבוה** — F7 (refund + 2-tap cancel, RICE 11,429), F5 (gentle push, RICE 10,000), F6 (voice quick-add, RICE 9,143). אלה לא הפיצ'רים ה"סקסיים" — F1 (voice brain-dump → AI plan) הוא ה-wedge אבל ה-Effort גבוה יותר. ההמלצה האסטרטגית: לבנות את ה-quick wins (notifications, refund, cancel) **לפני** ה-glamour features כי הם משחררים זמן ל-debugging של F1+F3 שהם ה-hard parts.

ה-build order הוא כפי שהוא משלוש סיבות: (1) **F9 (Privacy + MHMDA) ראשון** כי הוא חוסם את Google OAuth review (ש-Google לוקחת 4-8 שבועות); (2) **F3 (Google OAuth) מתחיל את התהליך בשבוע 1 גם אם הקוד עוד לא מוכן** כי ה-Google review הוא ה-critical path היחיד שהפאונדר לא שולט בו; (3) **F1 (Voice brain-dump) ו-F2 (Weekly view) ב-Sprint 1** כי בלעדיהם אין מוצר בכלל. v1.1 ו-v1.2 מתועדפים אחרי PMF signals כדי לא לבזבז זמן על פיצ'רים שלא מבקשים, ו-v2.0 (Android, Hebrew RTL, Web) דחוי ל-6-12 חודשים פוסט-launch כי כל אחד מהם הוא effort של 0.5-2 person-months שיהרוס את ה-iOS quality bar.

---

## RICE Methodology Reminder

- **Reach:** users affected per quarter
- **Impact:** 3 = massive, 2 = high, 1 = medium, 0.5 = low, 0.25 = minimal
- **Confidence:** 100% / 80% / 50% (data-backed / medium / gut)
- **Effort:** person-months
- **Formula:** RICE = (R × I × C) / E

---

## RICE Scoring Table (Full Roster)

| ID | Feature | Reach | Impact | Confidence | Effort (mo) | RICE | Notes |
|----|---------|-------|--------|------------|-------------|------|-------|
| F1 | Voice brain-dump → AI plan | 500 | 3 | 80% | 0.5 | 2,400 | Core wedge — Aha moment |
| F2 | Weekly view UI | 500 | 2 | 100% | 0.3 | 3,333 | Required core canvas |
| F3 | Google Calendar OAuth two-way | 400 | 3 | 80% | 1.0 | 960 | Tech moat; Google review timeline |
| F4 | Apple Calendar EventKit two-way | 400 | 2 | 100% | 0.15 | 5,333 | Cheap + critical wedge |
| F5 | Gentle push notifications | 500 | 2 | 100% | 0.1 | 10,000 | Lowest effort highest impact |
| F6 | Voice quick-add | 400 | 2 | 80% | 0.07 | 9,143 | Reuse F1 voice infrastructure |
| F7 | Refund + 2-tap cancel | 500 | 2 | 80% | 0.07 | 11,429 | Brand promise — anti-Inflow |
| F8 | Onboarding <90s | 500 | 3 | 100% | 0.2 | 7,500 | Highest leverage UX backbone |
| F9 | Privacy + MHMDA policies | 500 | 1 (regulatory floor) | 100% | 0.07 | 7,143 | Required — blocks Google review |
| F10 | Settings + account | 500 | 1 | 100% | 0.07 | 7,143 | Required infrastructure |
| --- | **v1.1 features** | | | | | | |
| F11 | Energy-aware mode | 300 | 2 | 50% | 0.3 | 1,000 | Differentiation; Flint overlap |
| F12 | Partner mode (shared read view) | 200 | 3 | 50% | 0.5 | 600 | Distribution multiplier; uncontested whitespace |
| F13 | Focusmate integration | 100 | 2 | 80% | 0.2 | 800 | Narrative + audience overlap |
| F14 | Weekly review prompt (Sunday) | 300 | 2 | 80% | 0.1 | 4,800 | Retention engine |
| F15 | Custom notification schedules | 200 | 1.5 | 80% | 0.1 | 2,400 | Power user retention |
| F16 | iOS widget (home screen) | 300 | 2 | 80% | 0.15 | 3,200 | Object permanence; engagement |
| F17 | Apple Watch companion | 100 | 1 | 50% | 0.5 | 100 | Defer — low signal |
| --- | **v1.2 features** | | | | | | |
| F18 | Recurring task UI | 300 | 1.5 | 80% | 0.2 | 1,800 | Workflow completeness |
| F19 | Sub-tasks / nesting | 200 | 1 | 50% | 0.2 | 500 | Optional — Goblin Tools overlap |
| F20 | Tags / categories | 200 | 1 | 50% | 0.15 | 667 | Optional; taxonomy = ADHD anti-pattern |
| F21 | Multiple Google accounts (3+) | 100 | 1 | 80% | 0.1 | 800 | Edge case (work+personal Google) |
| F22 | Light/Dark mode (manual) | 500 | 0.5 | 100% | 0.05 | 5,000 | Auto-supported by iOS — quick win |
| F23 | Referral program | 300 | 2 | 50% | 0.2 | 1,500 | After PMF; zero-competitor whitespace |
| --- | **v2.0 features** | | | | | | |
| F24 | Android version | 500 | 3 | 80% | 2.0 | 600 | Major rebuild; ~40% US TAM unlock |
| F25 | Web app | 200 | 1 | 50% | 1.5 | 67 | Defer — anti-mobile-first wedge |
| F26 | Hebrew RTL UI | 200 | 2 | 80% | 0.5 | 640 | Israel launch — founder market |
| F27 | Apple Reminders import | 200 | 1 | 80% | 0.15 | 1,067 | Migration aid from status quo |
| F28 | Notion / Todoist integration | 100 | 1 | 50% | 0.3 | 167 | Power user — scope creep risk |
| F29 | AuDHD-specific UX variant | 100 | 3 | 30% | 0.5 | 180 | Speculative; survey r/AuDHD first |
| F30 | In-app voice journaling (separate from planning) | 200 | 1 | 50% | 0.4 | 250 | Scope creep — Saner.AI territory |

---

## Prioritized Build Order

### Sprint 0 (Week 1, May 28 – June 3) — Foundation
1. **F9 Privacy + MHMDA policies** (RICE 7,143) — regulatory unblock; **must finish day 1-2** to start Google OAuth verification submission
2. **F8 Onboarding <90s** (RICE 7,500) — UX backbone; the load-bearing promise of the entire value-prop
3. **F3 Google OAuth APPLICATION START** — submit verification request to Google **even before code is final** (Google review = 4-8 weeks, this is the binary critical path)

### Sprint 1 (Week 2, June 4 – June 10) — Core Engine (spans WWDC week)
4. **F1 Voice brain-dump → AI plan** (RICE 2,400) — the core wedge; Aha moment in <60s
5. **F2 Weekly view UI** (RICE 3,333) — the canvas the plan renders into
6. **F6 Voice quick-add** (RICE 9,143) — reuse F1 voice infrastructure; near-zero marginal effort
7. **WWDC War-Room (June 8-10)** — monitor Apple Intelligence Calendar announcements; prepare positioning response within 48hr per `value-proposition.md` mitigation plan

### Sprint 2 (Week 3-4, June 11 – June 24) — Sync + Trust
8. **F4 Apple Calendar EventKit two-way** (RICE 5,333) — ship before F3 because EventKit is local API (no review queue); the "Tiimo wedge" half
9. **F3 Google Calendar OAuth two-way** (RICE 960) — finish integration once Google approval lands; full "Tiimo wedge" complete
10. **F5 Gentle push notifications** (RICE 10,000) — highest RICE in entire roster; ship before beta
11. **F7 Refund + 2-tap cancel** (RICE 11,429) — brand promise; must be in-app before App Store submission
12. **F10 Settings + account** (RICE 7,143) — account management, billing transparency line

### Sprint 3 (Week 5, June 25 – July 1) — Polish + Beta
- **TestFlight closed beta to 50-100 waitlist members** (per `customer-voice.md` recruitment)
- Bug fixing — focus on F4 EventKit edge cases (the #1 vulnerability if shipped buggy, per value-prop Red Flag)
- **Voice transcription diversity testing** — accented English / AAVE / code-switching (mitigates value-prop Red Flag)
- App Store submission (allow 1-2 week Apple review)
- **Public launch target: post-WWDC + ~3 weeks = June 29 – July 6**

### v1.1 (Months 2-3 post-launch, ~July-August 2026)
13. **F14 Weekly review prompt** (RICE 4,800) — Sunday voice journal; retention engine + emotional ritual
14. **F16 iOS widget** (RICE 3,200) — object permanence fix; cited explicitly as gain #18 in value-prop
15. **F15 Custom notification schedules** (RICE 2,400) — power user retention + notification blindness pain reliever
16. **F11 Energy-aware mode** (RICE 1,000) — branded differentiation; combine with 1-tap reshuffle so it's distinct from Flint stoplight
17. **F13 Focusmate integration** (RICE 800) — adjacent audience body-doubling
18. **F12 Partner mode** (RICE 600) — distribution multiplier; uncontested whitespace per competitor-landscape

### v1.2 (Months 4-6, ~September-November 2026)
19. **F22 Light/Dark mode manual** (RICE 5,000) — quick win; nearly free if iOS auto-supports
20. **F18 Recurring task UI** (RICE 1,800) — workflow completeness
21. **F23 Referral program** (RICE 1,500) — after PMF signal confirmed; zero-competitor whitespace per competitor-landscape
22. **F21 Multiple Google accounts** (RICE 800) — work+personal Google edge case
23. **F27 Apple Reminders import** (RICE 1,067) — migration aid from status quo (the biggest "competitor" per competitor-landscape)
24. **F20 Tags / categories** (RICE 667) — only if user signal; taxonomy is ADHD anti-pattern per `value-proposition.md`

### v2.0 (Months 6-12, ~December 2026 – May 2027)
25. **F26 Hebrew RTL UI** (RICE 640) — Israel launch; founder home market
26. **F24 Android version** (RICE 600) — major effort; unlocks ~40% US TAM (equity + Black/Latina under-representation in late-dx data)
27. **F19 Sub-tasks** (RICE 500) — workflow

### Cut / Defer Indefinitely (revisit only on signal)
- **F25 Web app** (RICE 67) — directly contradicts mobile-first wedge
- **F28 Notion / Todoist integration** (RICE 167) — scope creep; small audience
- **F29 AuDHD variant** (RICE 180) — pursue only if r/AuDHD survey shows signal
- **F30 Voice journaling** (RICE 250) — scope creep into Saner.AI territory
- **F17 Apple Watch** (RICE 100) — defer until Day 90+ user request signal

---

## Dependencies Map

```
F9 (Privacy + MHMDA policies)
   ↓ blocks
F3 (Google OAuth) — Google requires privacy policy URL + Health Data Policy at submission
   ↓ depends on (external)
Google verification review (4-8 weeks, binary risk)
   ↓ blocks
Sprint 2 launch readiness (calendar sync = #1 functional gain)

F1 (Voice brain-dump → AI plan)
   ↓ blocks
F6 (Voice quick-add) — shares iOS Speech Recognition + LLM pipeline
F14 (Weekly review prompt) — reuses voice infrastructure
   ↓ depends on
LLM API account (OpenAI/Anthropic) + iOS Speech permission + cost monitoring

F2 (Weekly view UI)
   ↓ blocks
F1 rendering (plan needs canvas to render into)
F4, F3 (calendar events need a view)
F16 (widget reads from same data model)

F4 (Apple Calendar EventKit two-way)
   ↓ blocks
F11 (Energy-aware reshuffle — writes new events back to calendar)
F18 (Recurring tasks — uses EKRecurrenceRule)
   ↓ depends on
iOS Calendar permission prompt + Apple Privacy Manifest declarations

F8 (Onboarding <90s)
   ↓ blocks
TestFlight beta (Sprint 3) — load-bearing promise tested with 20+ Maya users
   ↓ depends on
F1 + F2 + F4 functional (the 90s flow IS voice → plan → calendar write)

F7 (Refund + 2-tap cancel)
   ↓ blocks
App Store submission — Apple requires functional in-app subscription management
   ↓ depends on
RevenueCat or StoreKit2 integration + ops process for <48hr refund SLA

F10 (Settings + account)
   ↓ blocks
F7 (cancel button lives in settings)
F15 (notification schedule customization lives in settings)
F21 (multiple Google accounts management)

F12 (Partner mode)
   ↓ blocks
F23 (Referral program — reuses user-to-user invite infrastructure)
   ↓ depends on
Backend user-to-user data model + invite flow + shared-state sync

F24 (Android version)
   ↓ depends on
PMF signal on iOS first (retention >25% Day-30) + revenue to justify 2.0 person-months

F26 (Hebrew RTL UI)
   ↓ depends on
SwiftUI layout audit + Hebrew copy translation + RTL EventKit edge cases
```

---

## Effort Estimates Summary

| Phase | Total Effort | Cumulative Calendar | Launch Milestone |
|-------|--------------|---------------------|------------------|
| v1.0 (must-haves, F1-F10) | 2.55 person-months | 5-7 weeks part-time | App Store launch July 2026 |
| v1.1 (months 2-3, F11-F16 minus F17) | 1.35 person-months | + 4-5 weeks part-time | Retention layer Aug-Sep 2026 |
| v1.2 (months 4-6, F18+F20-F23) | 0.8 person-months | + 2-3 weeks | Power user + referral Nov 2026 |
| v2.0 (months 6-12, F24+F26+F27) | 2.65 person-months | + significant; Android dominant | Cross-platform 2027 |

**v1.0 total = 2.55 mo.** Solo vibe-coder at ~50% capacity (founder also doing GTM, support, content) = **~5 calendar months full effort, OR ~5-7 weeks if 90% UI already done means most of F2 is "wire it up" not "build it."** Original 90% UI claim is the bet — if that holds, the 2.55 mo collapses toward 1.5-1.8 mo and the July launch is achievable.

---

## Risk-Weighted Adjustments

For features with Confidence <80%, recommend pre-build validation:

| Feature | Confidence | Pre-build validation |
|---------|------------|----------------------|
| F11 Energy-aware mode | 50% | Test with TestFlight beta — would users use 3-tap morning check-in? Or is reshuffle button alone enough? |
| F12 Partner mode | 50% | Survey 10 paying users at Day 30 — would partner sub-share? Validate distribution-multiplier hypothesis. |
| F17 Apple Watch | 50% | Defer until Day 90+ user request signal in support inbox. |
| F19 Sub-tasks | 50% | Watch for "I wish I could nest" support tickets; otherwise resist (taxonomy anti-pattern). |
| F20 Tags / categories | 50% | Same as F19 — actively anti-ADHD. Build only if 5+ paying users explicitly request. |
| F25 Web app | 50% | Validate via "do you want a web companion?" survey at Day 60. Likely answer: no. |
| F28 Notion / Todoist | 50% | Only if 3+ paying users at Day 60 ask explicitly. |
| F29 AuDHD variant | 30% | Survey r/AuDHD (50K+ members) for interest before any build. |
| F30 Voice journaling | 50% | Watch for "I use Planny voice for non-planning thoughts" signals first. |

---

## Validation Loop for v1.1+

Before building each v1.1 feature, ask:

1. **Is it requested by 3+ paying users?** (not waitlist; paying = signal that survives the trial-to-paid threshold)
2. **Does retention data show a gap this feature fills?** (Day-7 / Day-30 cohort analysis vs. feature use)
3. **Does the founder's time budget allow without hurting v1.0 quality?** (especially F4 EventKit bug rate must stay <2% per `value-proposition.md` Red Flag)
4. **Does it strengthen one of the three wedges (sync trust / voice Aha / refund trust)** OR open a new validated wedge (partner whitespace)?

If <3 of 4 = defer.

---

## Strategic Connections
- ראה `mvp-definition.md` (forthcoming in this directory) ל-feature spec details + acceptance criteria
- ראה `user-journey.md` (forthcoming) ל-flow integration ובמיוחד ל-Sprint 1 onboarding flow
- ראה `02-strategy/go-to-market.md` (forthcoming) ל-launch sequencing סביב WWDC + ADHD Awareness Month (October)
- ראה `01-discovery/competitor-landscape.md` ל-wedges שמצדיקים את ה-Impact scores (Tiimo one-way sync = F3+F4 critical; Inflow billing = F7 critical)
- ראה `02-strategy/value-proposition.md` ל-jobs-to-be-done שמצדיקים את ה-Reach (Maya = 500 per quarter MVP-stage estimate)
- ראה `01-discovery/target-audience.md` ל-Maya persona שמצדיקה את ה-iOS-first + late-dx-women focus

---

## Sources

### Internal:
- `/home/user/NEW-_PROJECT/startup-validation/01-discovery/competitor-landscape.md` — wedges (Tiimo two-way sync, Inflow billing, Sunsama mobile)
- `/home/user/NEW-_PROJECT/startup-validation/02-strategy/value-proposition.md` — pains/gains hierarchy informing Impact scores
- `/home/user/NEW-_PROJECT/startup-validation/01-discovery/target-audience.md` — Maya persona informing Reach
- `/home/user/NEW-_PROJECT/startup-validation/01-discovery/raw/customer-voice.md` — verbatim quotes confirming pain priorities

### External benchmarks:
- RevenueCat State of Subscription Apps 2026 — trial-to-paid conversion benchmarks informing F7 Effort/Impact
- Google OAuth verification timeline (4-8 weeks) — informing F3 critical-path sequencing
- Apple App Store Review Guidelines (subscription cancellation = §3.1.2) — informing F7 must-ship-before-submission
- WWDC 2026 schedule (June 8, T-10 days) — informing Sprint 1 war-room timing

### RICE methodology:
- Intercom RICE prioritization framework (Sean McBride, 2017) — formula and Impact scale definitions

---

## Flags

**Red Flags:**

- **F3 (Google OAuth) Google review timeline is binary risk.** If Google rejects verification (possible reasons: incomplete privacy policy, missing Health Data Policy if voice data classified, broad scopes), Planny must reapply OR ship with **manual calendar-import fallback** (paste .ics, copy/paste meetings). This breaks the "two-way sync" wedge externally. **Mitigation:** apply Day 1 of Sprint 0; have manual-import fallback designed in parallel.

- **F1 (Voice brain-dump) LLM API costs at scale need monitoring vs MRR.** At $9.99/mo and ~$0.05-0.20 per voice-to-plan call, even 5 brain-dumps/week = $1-4/mo per user = 10-40% margin hit. **Mitigation:** instrument cost-per-user from Day 1 of beta; consider on-device transcription + cheaper LLM for parsing; cap at N free dumps/day with paid-tier unlock if needed.

- **F4 (Apple Calendar EventKit) sync quality is the #1 vulnerability** if shipped buggy — exact wedge claimed externally. Per `value-proposition.md` Red Flag, ship one-way write-back to Apple before claiming two-way externally if buggy. **Mitigation:** Sprint 3 bug-bash focuses here; do not externally claim "two-way" until <2% bug rate in beta.

- **F8 (Onboarding <90s) is load-bearing.** If actual onboarding ≥ 2 min in production, the entire value-prop falls apart in trial → Reddit screenshots → brand damage. **Mitigation:** internal SLA = under 75s median, tested with 20+ Maya-persona beta users before App Store submission.

- **F7 (Refund) operational gap.** Apple IAP refund processing has delays; if refund SLA <48hr is missed, the brand promise becomes a lie. **Mitigation:** founder manually issues supplementary refunds via Stripe/PayPal when Apple delays.

**Yellow Flags:**

- **F22 (Dark mode manual) is essentially free** — auto-supported by iOS SwiftUI but founder should test on all screens (some custom colors may not auto-invert correctly). 0.05 mo Effort estimate may even be high.

- **F26 (Hebrew RTL) deferred 6+ months** — Israel beachhead must wait until US Maya PMF confirmed. Founder is Israeli; emotional pull to ship Hebrew early must be resisted.

- **F24 (Android) is 2.0 feature; iOS-only at launch deferring ~40% of potential US Maya TAM.** Equity risk (Black/Latina women over-indexed on Android in some segments). **Mitigation:** publish Android timeline publicly to maintain trust; commit to within 6 months of iOS launch in any public communication.

- **F11 (Energy-aware mode) Confidence 50%** because overlaps with Sunsama capacity-aware + Flint stoplight check-in. Combine with mid-week 1-tap reshuffle (which neither does) to differentiate.

- **F12 (Partner mode) is named in value-prop but ships v1.1.** Risk: Maya churns to Cozi or Tiimo before partner mode ships. **Mitigation:** public roadmap with target date; ship within 6 months of v1.0.

- **F14 (Weekly review prompt) Sunday timing risk** — may trigger "Sunday scaries" instead of relieving them. **Mitigation:** test Sunday vs Friday-evening timing with beta; allow user to choose.

- **WWDC June 8 may invalidate F1 Reach assumption.** If Apple Intelligence Calendar ships heavy voice-to-schedule in iOS 27, F1's Impact may drop from 3 to 1.5 (still important but no longer differentiating wedge). **Mitigation:** war-room week of June 8-15; if Apple ships heavy, re-score F1 and pivot positioning to "ADHD-specific layer on top of Apple Intelligence" within 7 days.

- **Saner.AI Series Seed risk** — if Saner closes Q3 2026 and claims "voice your week" wedge first, F1's Confidence drops to 50%. **Mitigation:** ship F1 in Sprint 1 (June, before Saner can plausibly close + market) and lock late-dx-women persona publicly.

- **F23 (Referral) zero-competitor whitespace per competitor-landscape** — easy differentiator but mobile referral mechanics can be clunky. Test before over-investing.
