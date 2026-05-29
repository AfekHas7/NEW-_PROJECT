# MVP Definition — Planny

**Phase:** Phase 6 — Product (MVP)
**Project:** startup-validation (Planny)
**Date:** 2026-05-28
**Confidence:** Medium-High — היקף הפיצ'רים מבוסס ישירות על pain hierarchy מ-`target-audience.md` ועל wedge analysis מ-`competitor-landscape.md`; הערכות הבנייה הן indicative (תלוי בכיסוי ה-90% של ה-UI שהמייסד טוען); הסיכון הגדול ביותר — F3 Google OAuth review timeline (2-4 שבועות review מצד Google) ו-WWDC (June 8) שעלול לשנות את ה-platform calculus תוך 11 ימים.

---

## תקציר MVP

ה-MVP של Planny צריך להוכיח דבר אחד בלבד תוך 90 ימים: **late-diagnosed US women 25-40 ישלמו $5-10/mo עבור voice brain-dump → AI weekly plan עם two-way Google + Apple Calendar sync, אם המוצר מכבד אותן (no streaks, refund נדיב, 2-tap cancel).** ה-MVP הוא 10 פיצ'רים שמכסים את 5 ה-pains המובילים מ-`target-audience.md` (setup overwhelm, time blindness, task initiation paralysis, object permanence, calendar fragmentation) + 3 brand promises נון-נגושיות (no shame, refund, founder access). כל מה שמעבר ל-10 הפיצ'רים — partner mode, energy-aware, Focusmate, Hebrew RTL, Android — נדחה ל-v1.1 או v2.0 כדי לעמוד בחלון השיגור של 5-7 שבועות. ה-launch window הוא **June 22 - July 1, 2026** (1-2 שבועות אחרי WWDC June 8), והבדיקה הקריטית: האם 100-300 משלמים בשלושת החודשים הראשונים, עם Day-30 retention ≥15% (כפול ב-3.7x מ-productivity category benchmark של 4.1%) ו-refund rate <15%.

---

## Core Hypothesis the MVP Tests

**Primary hypothesis:** Late-diagnosed US women 25-40 with ADHD will pay **$5-10/mo** for an app that lets them voice their week in <90 seconds and syncs both ways with Google Calendar — *if* the app respects them (no streaks, no shame, easy refund).

**Sub-hypotheses to be validated:**

1. **Voice-first brain dump** achieves Day-7 activation (≥35% return) — מבוסס על ה-Aha Moment ב-`target-audience.md` ("voice in, week out") ועל ה-Sub-90s onboarding promise ב-`value-proposition.md`.
2. **Two-way Google Calendar OAuth** is the moat that drives switch-from-Tiimo — מבוסס על `competitor-landscape.md` (Tiimo Nolt #1 feature request פומבי) ועל positioning wedge #2 ב-`positioning.md`.
3. **30-day refund + 2-tap cancel** does NOT cause >15% refund rate — מבוסס על trust-wedge נגד Inflow ב-`positioning.md` ועל RevenueCat refund benchmarks (3-8% רגיל ב-productivity).
4. **Anti-shame UX** (no streaks, no red overdue) materially improves Day-30 retention vs category benchmarks (4.1% → 15%+) — מבוסס על pain #6 + #9 ב-`target-audience.md` ("Streaks shame" + "App graveyard") ועל emotional jobs ב-`value-proposition.md`.

**Falsification conditions:** אם Day-7 retention <20%, ה-voice-first hypothesis לא תקפה. אם refund rate >25%, או model trust-promise קורסות, או pricing לא תואם פרסונה. אם Day-30 <8%, ה-anti-shame UX לא material differentiator vs category baseline.

---

## Must-Have Features (v1.0 — Launch)

### F1: Voice Brain-Dump → AI Weekly Plan

**What it does:** המשתמשת לוחצת ומחזיקה על כפתור מיקרופון במסך הראשון. מדברת חופשי 30-90 שניות על השבוע ("יש לי dentist ביום רביעי, צריך להתקשר לאמא, שלוש פגישות ביום חמישי, להגיש Q3 deck עד שישי"). AI מתמלל + מסדר את התוכן ל-weekly view עם slots מציאותיים, buffers ו-confidence-based parsing.

**Why must-have:** **This IS the product.** Pain #1 ב-`target-audience.md` הוא "setup overwhelm — downloaded 30 apps, abandoned 28". ה-Aha Moment ב-`target-audience.md` הוא בדיוק זה: "voice in, week out, <90 שניות, מאפס הגדרות". Tiimo Co-planner הוא partial text+voice — אף אחד לא מאחד voice → AI → weekly view במסך אחד. **בלי זה, אין wedge, אין מוצר, אין Aha.**

**Success metric:**
- ≥70% של installs משלימים first voice brain-dump ב-session ראשון
- Median time-to-first-plan ≤75 שניות (internal SLA, ה-promise החיצוני "60 sec")
- Transcription accuracy ≥90% עבור US English (test diverse beta cohort כולל AAVE / accented English)

**Build estimate:** **Medium-Large (M-L)** — 10-14 ימי עבודה
- iOS Speech Recognition API (native, free) או Whisper API (paid, multi-lingual) — החלטה תלויה ב-Hebrew RTL question למייסד
- LLM API integration (OpenAI GPT-4o-mini @ ~$0.15/1M tokens or Anthropic Haiku @ ~$0.25/1M tokens) — eval שניהם ב-week 1
- Prompt engineering ל-"extract structured schedule from messy ADHD voice" — דורש 20-30 iterations עם sample data
- Confidence-based parsing: high-confidence items go in plan; low-confidence surface as "did you mean?" cards
- Text fallback always one tap away (per `value-proposition.md` yellow flag — voice cannot be only path)

**Dependency:** LLM API account (OpenAI or Anthropic) + iOS Speech permission flow

---

### F2: Weekly Calendar View (Mobile-First)

**What it does:** Visual week view, Mon-Sun או Sun-Sat (user choice בהגדרות). Tap day to see hour-by-hour. Drag/tap to add/edit/remove items. Always-visible "now" indicator. Buffer time visible by default (15-min gaps). אין color-coding decisions ב-onboarding — ברירת מחדל מינימליסטית (sage / cream / muted indigo per `positioning.md` brand voice).

**Why must-have:** It's a planner — חייב weekly view. `positioning.md` קובע weekly cadence כ-Y axis differentiator (לא daily ritual שנשרף, לא single-fire task). `value-proposition.md` gain #11 ו-#19 דורשים את זה ישירות. **בלי weekly view אין positioning של "weekly planner".**

**Success metric:**
- User views weekly screen ≥3 times/week (active users)
- Time-to-render <1 second after open
- Zero "blank state" rendering — אם אין events, מציג onboarding prompt ל-voice brain-dump

**Build estimate:** **Medium (M)** — 5-7 ימי עבודה (בהנחת UI 90% מוכן, integration + state management בלבד)

**Dependency:** Local DB (Supabase free tier / Firebase / native CoreData) — החלטה תלויה ב-cross-platform plan

---

### F3: Two-Way Google Calendar OAuth Sync

**What it does:** המשתמשת מחברת Google Calendar via OAuth (calendar.events scope only — minimum scope per `value-proposition.md` privacy gain). Planny קוראת events קיימים + כותבת events חדשים. Bidirectional updates within 5 minutes. Conflict resolution: last-write-wins עם undo. Recurring events, all-day events, time zones — מטופלים נכון.

**Why must-have:** **#1 wedge טכני נגד Tiimo** (per `competitor-landscape.md` — Tiimo one-way sync = #1 feature request ב-tiimo.nolt.io, public for 2+ years). Pain #7 ב-`value-proposition.md` (calendar fragmentation) ו-must-have gain #1 בלי זה, Maya חוזרת ל-Apple Reminders + Google Calendar manual. בלי זה, Planny הוא Tiimo עם voice — לא "the only one with two-way sync".

**Success metric:**
- ≥60% של paying users מחברים calendar ב-7 ימים ראשונים
- Sync latency p95 <5 minutes
- Sync error rate <2% של write operations
- Zero duplicate events created (idempotency critical)

**Build estimate:** **Large (L)** — 15-20 ימי עבודה (כולל Google review queue)
- Google Cloud Project setup + OAuth consent screen verification (Google sensitive scope review: **2-4 שבועות review**, חייב להתחיל day 1)
- Read API integration (3-4 ימים)
- Write API integration + conflict resolution (4-5 ימים)
- Edge cases: recurring events, all-day events, time zones, RSVP, attachments (4-5 ימים)
- Testing matrix: Google Workspace accounts + personal Gmail + multi-calendar accounts (2-3 ימים)

**Dependency:** **CRITICAL — Google Cloud Project + OAuth consent screen approval. זה ה-bottleneck של תאריך השיגור.** אם Google review מתעכב, השיגור מתעכב.

---

### F4: Apple Calendar Sync (EventKit)

**What it does:** Read + write to Apple Calendar via native EventKit. iOS only. Two-way: add event in Apple Calendar → appears in Planny within seconds; plan in Planny → writes to Apple Calendar עם proper buffers. אין iCloud bridge (זה מה ש-Tiimo / Akiflow נכשלות שם — per `value-proposition.md` red flag).

**Why must-have:** Maya משתמשת ב-Google Calendar בעבודה (Workspace) ו-Apple Calendar באישי (per `positioning.md` target customer). בלי שני הצדדים, "calendar fragmentation" pain reliever לא עובד. גם — iOS-first launch = EventKit הוא ה-fast-path השני אחרי Google. **EventKit שהציפיות עליו טובות יותר מ-Google (no review queue).**

**Success metric:**
- Apple sync users have ≥10% גבוה יותר Day-30 retention than Google-only users (validation של "both calendars" hypothesis)
- ≥50% של paying users מחברים Apple Calendar (לעומת ה-60% של Google)
- Zero sync failures dropped to user (silent retry + visible error if persistent)

**Build estimate:** **Small-Medium (S-M)** — 3-5 ימי עבודה (EventKit well-documented; iOS permissions straightforward)

**Dependency:** iOS permissions (NSCalendarsUsageDescription) + Apple Privacy Manifest (iOS 17+ requirement)

---

### F5: Gentle Push Notifications (No Streaks, No Red)

**What it does:** Customizable push reminders for tasks/events. Tone informative, not punitive. **אסור streaks. אסור "you missed!" alerts. אסור red badges.** Per-task customization: silent / push / sound. Time-bracketed (quiet hours respected). Default sparse, not chatty — אופציה ל-"reduce notifications" ב-onboarding.

**Why must-have:** Anti-shame UX הוא **brand promise פומבי** (per `positioning.md`). Pain #9 ב-`target-audience.md` ("Streaks shame / red overdue") ו-pain #12 ("Notification blindness") שניהם מטופלים פה. Object permanence (pain #4) — בלי push, "Planny is buried on page 3 of her phone" (AFFiNE quote). **בלי F5, ה-brand voice סותר את עצמו ב-day 1.**

**Success metric:**
- ≥80% של users שומרים notifications מופעלות (לא משבתים ב-iOS settings)
- Zero "I deleted because of notifications" feedback ב-90 ימים ראשונים
- Notification opt-out rate per task type ≤10%

**Build estimate:** **Small (S)** — 2-3 ימי עבודה
- OneSignal free tier (≤10K subscribers) או native APNs ישיר
- Quiet hours engine
- Per-task notification preferences UI

**Dependency:** Push notification provider (OneSignal free tier מספיק ל-MVP) + iOS notification permission flow

---

### F6: Voice-Driven Quick Add

**What it does:** Tap mic anywhere באפליקציה (FAB or shortcut) ל-add single task/event by voice. "Add dentist tomorrow at 10." → AI parses + writes לתאריך הנכון. Confirmation card עם undo.

**Why must-have:** Voice-first הוא brand spine — לא רק brain-dump חד-פעמי. `value-proposition.md` gain #9 ("voice input because typing is friction at brain-dump moment") — חייב להיות זמין בכל מקום, לא רק במסך onboarding. **בלי F6, voice = onboarding gimmick, לא product DNA.**

**Success metric:**
- ≥40% של new tasks מתווספים via voice (לא typed)
- Voice quick-add success rate ≥85% (AI parses correctly first try)
- Time-to-task-added <5 שניות מ-tap to confirmation

**Build estimate:** **Small (S)** — 2 ימי עבודה (reuse F1 voice infrastructure + simpler prompt for single-task parsing)

**Dependency:** F1 voice infrastructure shipped first

---

### F7: 30-Day Refund + 2-Tap Cancel

**What it does:** In-app cancellation in 2 taps (Settings → Subscription → Cancel → confirm). Refund button visible לכל active subscription. Email confirmation upon cancel + upon refund. Refund processed <48hr (subject to Apple/Google IAP constraints; founder owns supplementary refund if platform delays).

**Why must-have:** **Brand promise פומבי + #1 trust wedge נגד Inflow** (per `competitor-landscape.md` — "$95 charge + takedown emails" Trustpilot pattern). Pain #5 ב-`value-proposition.md` (subscription guilt / ADHD tax) חייב פתרון מבני. **זה ה-cost-on-purpose שמייצר ה-trust signal — בלי F7, ה-positioning של "we know the ADHD tax" הוא ריק.**

**Success metric:**
- Cancellation flow time <30 שניות median
- Refund rate <15% (target 5-10% per `value-proposition.md` model)
- Refund processing time <48hr p95
- Zero "I couldn't cancel" complaints על r/ADHDWomen ב-90 ימים ראשונים

**Build estimate:** **Small (S)** — 2-3 ימי עבודה
- Apple StoreKit 2 integration (subscription management)
- Google Billing integration (אם Android in scope)
- Refund webhook listener (Server2Server notifications מ-Apple/Google)
- Founder email notification on every refund (founder learning loop, not retention call)

**Dependency:** Apple Developer account + App Store Connect subscription configured + Google Play Console (אם Android)

---

### F8: Onboarding (<90 Seconds to First Plan)

**What it does:** Welcome screen עם founder voice/photo + verifiable ADHD disclosure ("Hi, I'm [Founder]. I have ADHD and built Planny because Tiimo broke my brain. Tap the mic and tell me about your week."). Voice prompt עם דוגמה מודלקת. Show generated plan within 90 שניות. אין taxonomy decisions, אין color-coding choices, אין categories setup.

**Why must-have:** Setup overwhelm = pain #1. <90s = ה-kill metric שמבדיל את Planny מ-Tiimo. Founder credential = #1 sniff test ב-r/ADHDWomen ("is the founder ADHD?"). **בלי F8, ה-Aha Moment לא קורה ב-session ראשון = 70%+ churn risk.**

**Success metric:**
- Median time מ-install ל-first plan ≤90 שניות
- 80% completion rate (install → first plan)
- ≥50% של users שראו את ה-first plan ממשיכים ל-day 2

**Build estimate:** **Small-Medium (S-M)** — 3-4 ימי עבודה (UI design קיים; כתיבת copy + voice recording + timing optimization)

**Dependency:** F1 voice infrastructure shipped + founder voice/video recording

---

### F9: Privacy Policy + MHMDA Health Data Policy

**What it does:** Two-policy structure: general Privacy Policy + separate Health Data Policy (per Washington State MHMDA + similar state laws). Clear consent flows ב-onboarding. אין third-party tracking pixels בדפי landing שמזכירים ADHD. Data deletion path מ-Settings בתוך App. Data export request flow.

**Why must-have:** **Regulatory floor.** Mental-health adjacent app חייב לעמוד ב-MHMDA (Washington), CCPA (California), GDPR-lite (Apple Privacy Manifest iOS 17+). App Store rejection risk אם חסר. `value-proposition.md` gain #3 (privacy must-have) ו-pain associated.

**Success metric:**
- App Store approval ב-pass ראשון או שני
- Zero privacy complaints ב-90 ימים ראשונים
- Privacy Policy + Health Data Policy ב-2 קליקים מ-home screen

**Build estimate:** **Small (S)** — 1-2 ימי עבודה
- Legal counsel review או template מהימן ($500-2,000 מתוך ה-$1,500 budget — נמצא ב-tension עם marketing budget; שקול pro-bono כיוון אם קיים)
- App-side: settings screen + consent flow + data deletion endpoint

**Dependency:** Legal review (TOS + Privacy + Health Data) — recommend Termly או iubenda templates ($50-200) + 1-hour attorney review ($300-500)

---

### F10: Basic Settings + Account Management

**What it does:** Email/notification preferences, calendar disconnect, account deletion (one-tap), support email link, founder DM link (TikTok), version info, sign out. אין "delete account requires email verification 5 days" friction — must be immediate per Apple guidelines.

**Why must-have:** **Standard + App Store requirement** (data deletion path required לכל apps שמאחסנים user data, per Apple Guideline 5.1.1(v)). Pain #5 ב-`value-proposition.md` (cancellation predatory pattern) — settings החייבים להיות clean.

**Success metric:**
- Account deletion completes ב-<60 שניות
- Zero "I couldn't delete my account" complaints
- Settings screen load <500ms

**Build estimate:** **Small (S)** — 2 ימי עבודה

**Dependency:** Backend account management endpoint + email service (SendGrid free tier / Resend free tier)

---

## Total MVP Build Estimate (v1.0)

| # | Feature | Estimate (days) | Cumulative |
|---|---------|-----------------|------------|
| F1 | Voice brain-dump → AI weekly plan | M-L (10-14) | 14 |
| F2 | Weekly view (mobile-first) | M (5-7) | 21 |
| F3 | Google OAuth (incl. 2-4wk Google review parallel) | L (15-20 build + 14-28 review) | 41 |
| F4 | Apple EventKit two-way | S-M (3-5) | 46 |
| F5 | Gentle notifications | S (2-3) | 49 |
| F6 | Voice quick-add | S (2) | 51 |
| F7 | 30-day refund + 2-tap cancel | S (2-3) | 54 |
| F8 | Onboarding <90s | S-M (3-4) | 58 |
| F9 | Privacy + MHMDA | S (1-2) | 60 |
| F10 | Settings + account mgmt | S (2) | 62 |

**Total estimated working days solo full-time: ~62 ימי עבודה**

**Critical path adjustment:** F3 (Google OAuth) has 2-4 שבוע Google review queue **שיכול לרוץ במקביל לעבודה על F1, F2, F4-F10**. אם המייסד מתחיל את Google verification ב-day 1, ה-review מסתיים בערך ב-day 21-28 — בזמן ש-F1+F2 כבר מוכנים לאינטגרציה. **Realistic full-time timeline: ~30-40 ימי עבודה assuming F3 review starts day 1.**

**Founder constraint:** ~25-30 שעות/שבוע part-time (vibe coder, less native experience, ADHD founder energy ניהול) = effective ~12-15 שעות אפקטיביות, נניח שווי ל-~2-2.5 ימים מלאים/שבוע → real timeline **5-7 שבועות ל-launch-ready** (התואם ל-launch target June 22 - July 1, 2026, ~4-5 שבועות מ-today + WWDC week buffer June 8-15).

**Cost estimate ל-v1.0 (excluding founder time):**
- LLM API (testing + first 1K users): ~$50-150
- Google Cloud (OAuth + minimal infra): $0-50
- Apple Developer: $99/yr (already required)
- Supabase/Firebase: $0 (free tier)
- OneSignal: $0 (free tier)
- Legal templates + 1hr attorney: $400-700
- Domain + landing page: $20-50
- **Total infra/legal: ~$500-1,000** (mostly legal — שאר $500-1,000 ל-marketing per `competitor-landscape.md` budget allocation)

---

## Nice-to-Have Features (v1.1 — Months 2-3)

| Feature | Why deferred (anchor to research) | Priority |
|---------|------------------------------------|----------|
| **Energy-aware mode** (low/med/high day check-in + 1-tap reshuffle) | Pain #10 + gain #13 — important but not critical for trial conversion; Flint stoplight is comparable, not differentiator alone | **High** |
| **Partner mode** (read-only shared week view + shared errands) | Pain #8 (partner friction); gain #14; **whitespace currently uncontested** per `competitor-landscape.md`; 2-3 weeks build with auth/sharing layer | **High** |
| **Focusmate integration** (body-double from any task) | `value-proposition.md` gain #15; narrative bonus; OAuth integration ~3 days | Medium |
| **Weekly review prompt** (Sunday/Friday voice check-in journal) | `value-proposition.md` gain #22; emotional ritual; retention booster | Medium |
| **Mid-week re-plan flow** ("today fell apart, redo next 48hr") | `value-proposition.md` gain #19; Sunsama/Tiimo killer; needs more product polish | **High** |
| **"Just one thing" home-screen CTA** | Pain #3 (task initiation); gain #17; low moat (Goblin Tools comparable) but high emotional impact | Medium |
| **Lock-screen widget + home widget** | Pain #4 (object permanence); gain #18; iOS 17+ WidgetKit ~3-4 days | **High** |
| **Recovery flow** ("this week was hard, let's just look at tomorrow") | `value-proposition.md` gain #25; differentiating emotional moment; needs trigger logic | Medium |
| **Proactive day-14 pause email** | `value-proposition.md` gain #24; brand asset; needs email infrastructure + dormancy detection | Medium |
| **Kind notes** (opt-in periodic affirmations) | `value-proposition.md` gain #23; replicable but tipping-point moment | Low-Medium |
| **First-week visible win** ("you reclaimed X hours") | `value-proposition.md` gain #26; concrete value receipt before trial-end | Medium |
| **Apple Watch companion** | Premium signal; small persona ROI in v1; ~1 week build | Low |
| **Custom notification schedules** (power-user mode) | Power-user; v1 default is sparse, custom is overkill | Low |
| **Dark mode toggle** | Many ADHD adults prefer; iOS auto-supports if implemented properly | Low (auto) |
| **Multi-account Google calendars** (3+ accounts) | Edge case; defer | Low |
| **Recurring task UI** (visual repetition editor) | Defer to v1.1 | Medium |
| **Sub-tasks / nesting** | Defer; v1 keeps flat task model | Low |
| **Import from Tiimo / Sunsama / Notion** | Migration accelerator; v1.1-1.2 | Medium |

---

## Explicitly Out of Scope (v1.0 — and Why)

| Feature | Why not (anchor) |
|---------|-------------------|
| **Streaks / habits tracking** | **Anti-value. Never.** Word-banned per `target-audience.md`. "Toxic לקהל הזה." |
| **Gamification (badges, points, leaderboards)** | Anti-shame violation; Numo plays this lane and is documented weak. Per `positioning.md`. |
| **Social features (sharing, leaderboards, comparison)** | Comparison shame trigger; out of beachhead scope |
| **In-app coaching content / advice** | Regulatory line (FDA SaMD); per `value-proposition.md` "Planny is a planner, not therapy" |
| **Therapy-grade emotional regulation** | Anti-target; comorbidity expectation gap risk per `value-proposition.md` |
| **Multi-user / team / family plan** | Out of beachhead (Motion territory). Family-mode = v1.2 |
| **Hebrew RTL UI** | Israel launch deferred to Month 6+ per `value-proposition.md` US-first focus |
| **Android version** | iOS-first per `positioning.md` (US women 25-40 = iPhone-heavy); Android in Month 2-3 |
| **Web app / desktop** | Mobile-first per anti-Sunsama wedge; web in Year 2 |
| **Health metric tracking (sleep, mood, HRV)** | Out of scope; regulatory risk; not in JTBD |
| **AI chat / "Ask Planny" mode** | Scope creep into Saner.AI territory; defer |
| **Multi-language voice (non-English)** | English-only for v1.0; Hebrew + Spanish wave 2 |
| **Multiple Google accounts (3+)** | Edge case; defer to v1.2 |
| **Recurring task management UI** | Defer to v1.1 (basic recurrence supported via Google/Apple sync) |
| **Sub-tasks / nesting** | Defer to v1.1 |
| **Tagging / categories** | Defer to v1.2 — direct violation of "no taxonomy decisions" onboarding principle |
| **File / image attachments** | Out of scope |
| **Time tracking** | Toggl territory; not in JTBD |
| **Integration with Notion / Todoist / Things / Linear** | Defer to v2.0 (post-PMF) |
| **Apple Reminders import** | Wishlist; defer — bridge via Apple Calendar sync (Reminders calendar) |
| **In-app community / forum** | Anti-value (comparison shame trigger); founder DM is the proxy |
| **Referral program** | Defer to v1.2 (post-PMF); per `competitor-landscape.md` whitespace but premature to invest |
| **Outlook integration** | Microsoft Copilot territory; persona is Google Workspace + Apple, not Outlook |
| **Voice in onboarding for non-English** | English-only v1.0 (Whisper supports Hebrew but adds cost; revisit post-PMF) |
| **B2B / coach dashboard** | Tertiary persona (coaches); v2.0 if signals |
| **Apple Watch standalone app** | iOS companion in v1.1; standalone v2.0 |
| **iPad-optimized layout** | iPhone-first; iPad scales but not optimized in v1 |

---

## Success Criteria for MVP (Day 90 Post-Launch — by ~Sept 22, 2026)

### Quantitative

| Metric | Target (base case) | Stretch | Floor (kill consideration) |
|--------|-------------------|---------|----------------------------|
| **Paying users** | 100-300 | 500+ | <15 |
| **MRR** | $500-1,500 | $2,500+ | <$100 |
| **Day-7 retention** | ≥35% | ≥50% | <20% |
| **Day-30 retention** | ≥15% (vs 4.1% productivity benchmark) | ≥25% | <8% |
| **Trial-to-paid conversion** | ≥20% (vs 38% RevenueCat median) | ≥30% | <10% |
| **Refund rate** | <15% | <8% | >25% |
| **Voice brain-dump completion** (first session) | ≥70% | ≥85% | <50% |
| **Calendar connection rate** (first 7 days) | ≥60% | ≥80% | <30% |
| **Median onboarding time** | ≤90 seconds | ≤60 seconds | >180 seconds |

### Qualitative

- **≥10 unsolicited testimonials** מ-real users (TikTok, App Store reviews ≥4-star, DM screenshots)
- **≥1 mention** ב-ADDitude / Tracy Otsuka podcast / How to ADHD / other ADHD media (paid or earned)
- **≥5 organic Reddit r/ADHDWomen mentions** (not founder-posted)
- **≥1 viral TikTok** (>50K views) — מ-founder או מ-creator seeding pool
- **≥3 founder DMs/week** מ-real users (signal of accessibility working)
- **Refund tone:** ≥80% של refund emails are gracious ("not for me" / "wrong time"), not angry ("scam" / "bait and switch")

### Validation Hypothesis Results

| Hypothesis | GO condition | KILL condition |
|-----------|--------------|----------------|
| **Maya will pay $5-10/mo** | ≥100 paying users at <15% refund rate | <30 paying users OR >25% refund |
| **Two-way OAuth is the switch driver from Tiimo** | ≥30% of paying users cite "Google sync" or "Apple sync" in NPS/feedback OR ≥40% connect both calendars | <10% cite sync; sync usage uncorrelated with retention |
| **Anti-shame UX → retention lift** | Day-30 ≥10% (well above 4.1% baseline) | Day-30 ≤6% (no material lift) |
| **Voice-first is the wedge (not text-first)** | ≥40% of all tasks added via voice; voice users have ≥15% higher Day-30 than text-only users | <20% voice usage; voice doesn't differentiate retention |
| **Founder ADHD disclosure is trust signal** | ≥50% of new sign-ups cite founder/built-by-ADHD in survey OR ≥20% come from founder TikTok | No correlation between founder visibility and conversion |

---

## Failure Criteria (Kill Switches)

### Hard Kill — Stop, Evaluate Pivot, or Stop Entirely

- **<15 paying users by Day 90** — market signal absent
- **Day-30 retention <3%** — below mental health benchmark; product doesn't retain
- **Refund rate >25%** — unit economics break; trust positioning damaged
- **CAC >$40 עם אין path ל-<$20** — even at high LTV, $1,500 budget can't sustain
- **Critical bug ב-calendar sync שגורם ל-data loss** — brand-killer; recall scenario
- **App Store rejection** שאי אפשר לתקן ב-2-3 cycles — distribution blocked

### Soft Kill — Pivot Within Brand

- **15-50 paying users + retention 5-10%** → pivot persona ל-V1 Working Parents או V1 ADHD Men 30-40
- **ADHD audience explicitly rejects voice-first** (text usage >voice in active users) → consider text-first variant; voice as power-user feature
- **Two-way sync usage <20%** → reposition wedge (voice + AI weekly without sync hype)
- **Founder TikTok doesn't gain traction** (organic <1K followers ב-90 ימים) → shift channel mix ל-podcast-heavy + creator gifting only

### Yellow Warnings (Adjust, Don't Kill)

- Trial-to-paid 10-20% → improve trial Aha moment; longer trial?
- Refund rate 15-25% → review refund reasons; tighten onboarding fit
- Day-7 retention 20-35% → improve day 1-7 hooks (notifications, re-engagement email)

---

## ADHD-Specific Adaptations the Founder Already Knows He Needs

> **Note:** המייסד ציין ב-Phase 4 confirmation "יש התאמות שצריך לעשות לADHD". להלן המלצות agent־הן מבוססות `target-audience.md` ו-`value-proposition.md`; המייסד צריך להוסיף / לתקן בהתאם ל-UI שכבר תכנן.

1. **No streaks of any kind** — anywhere in product. אסור counter, אסור chain, אסור "X days in a row".
2. **No red color for overdue / missed** — use amber/yellow if needed; never red. Red = anxiety trigger ב-ADHD per `target-audience.md`.
3. **Soft animations only** — no aggressive bounces / shakes / pulsing alerts. iOS standard easing curves; subtle fades.
4. **Sound design subtle** — no loud chimes; soft chimes או none by default. Notifications silent by default; user opts in to sound.
5. **Reduce text density** — short sentences, 12-18 words max per copy block. Generous whitespace per `positioning.md` brand voice.
6. **High contrast for AuDHD users** — toggleable accessibility mode. Respects iOS Dynamic Type.
7. **Optional dark mode** — many ADHD adults prefer less stimulation; auto-follow iOS system setting.
8. **Reduced motion option** — respects iOS accessibility setting (UIAccessibility.isReduceMotionEnabled).
9. **Buffer time auto-insertion** — between meetings, default 15 min. Per `value-proposition.md` Pain Reliever #2.
10. **No timer countdowns** — anxiety trigger. Use elapsed time or simple "due X" framing.
11. **Tap targets ≥44pt** — finger-fatigue / fine-motor variability ב-ADHD population.
12. **One-thumb operation** — primary actions reachable ב-thumb zone (bottom 2/3 של screen).
13. **Voice button always accessible** — FAB on every primary screen, not buried.
14. **"Carry to tomorrow?" instead of "missed"** — language matters; per `value-proposition.md` gain #10.
15. **Confirmation copy never punitive** — "Got it" / "Done" / "Saved" — never "Finally!" / "About time!".

> Recommend founder review and add specific UX nuances he's planned that may differ.

---

## Founder Input Requested

מספר פתוחים שאשמח לתשובה לפני סגירת Phase 6:

1. **כמה מ-90% של ה-UI שכבר מוכן מכסה את F1-F10?** האם יש פיצ'רים שכבר עשית ולא כללתי ב-MVP? האם יש פיצ'רים ב-MVP שאתה לא רוצה לבנות?
2. **Apple Speech Recognition vs OpenAI Whisper vs Anthropic?** — Apple Speech חינמי אבל English בלבד; Whisper תומך Hebrew ו-50+ שפות אבל עולה ~$0.006/דקה; GPT-4o-mini + Apple Speech hybrid (Apple transcribes, GPT structures) הוא ה-cost-optimal. **המלצה: Apple Speech + GPT-4o-mini ל-v1.0 (English only).**
3. **האם אתה מסכים ש-Hebrew RTL נדחה ל-Month 6+?** — או שאתה רוצה לעשות bilingual מ-day 1 (יוסיף ~2-3 שבועות + Whisper costs)?
4. **F3 (Google OAuth) — כבר התחלת את ה-verification process?** אם לא, זה ה-bottleneck של תאריך השיגור. **חייב להתחיל היום או מחר.**
5. **iOS-only launch או iOS + Android במקביל?** — Android מאריך 2-3 שבועות לכל הפיצ'רים (F1-F10) + שונות EventKit (אין equivalent ל-Apple Calendar; Google Calendar רק) + Play Console review queue.
6. **WWDC June 8 war-room plan** — מי בודק את ה-announcements? איזה 3 scenarios מוכנים מראש (Apple ships heavy / light / delays)? אני יכול לעזור עם content rapid-response.
7. **Legal counsel ל-Privacy + MHMDA + TOS** — יש לך מישהו? אם לא, ממליץ Termly או iubenda template + 1-hour attorney review ($400-700 מתוך ה-$1,500 budget). זה in-tension עם marketing budget — נדרשת החלטה.
8. **Founder ADHD disclosure plan** — האם אתה מוכן לציבוריות מלאה (TikTok build-in-public, in-app "Talk to founder" button, ADDitude/podcast appearances)? זה ה-#1 trust wedge — חייב להיות אותנטי ועקבי.

---

## Strategic Connections

- ראה `feature-prioritization.md` (TBD) ל-RICE scoring מפורט של F1-F10 + v1.1 backlog
- ראה `user-journey.md` (TBD) ל-end-to-end UX flow מ-discover ל-Day 30
- ראה `02-strategy/positioning.md` ל-onliness components שה-MVP מקיים
- ראה `02-strategy/value-proposition.md` ל-pain relievers + gain creators mapping ל-F1-F10
- ראה `01-discovery/target-audience.md` ל-pain hierarchy שמשם נגזרו ה-must-haves
- ראה `01-discovery/competitor-landscape.md` ל-wedge analysis (two-way sync vs Tiimo, refund vs Inflow, mobile-first vs Sunsama)
- ראה `02-strategy/go-to-market.md` (TBD) ל-launch timeline integration עם WWDC June 8 ו-Tracy Otsuka window

---

## Sources

### Phase 3 (Discovery)
- `/home/user/NEW-_PROJECT/startup-validation/01-discovery/target-audience.md` — pain hierarchy (10 ranked pains), Maya persona, JTBD, language map
- `/home/user/NEW-_PROJECT/startup-validation/01-discovery/competitor-landscape.md` — Tiimo Nolt feature gap, Inflow billing reputation, Sunsama mobile gap, platform absorption risk

### Phase 4 (Strategy)
- `/home/user/NEW-_PROJECT/startup-validation/02-strategy/value-proposition.md` — 15 pain relievers + 27 gain creators mapped to features
- `/home/user/NEW-_PROJECT/startup-validation/02-strategy/positioning.md` — Onliness components, category claim, target customer, anti-targets

### External benchmarks
- RevenueCat State of Subscription Apps 2026 (refund rates, trial conversion benchmarks, Day-30 retention by category)
- Adapty State of In-App Subscriptions 2026 (US productivity average $15.20/mo)
- Apple Developer Documentation (EventKit, StoreKit 2, Privacy Manifest iOS 17+)
- Google Calendar API documentation (OAuth scopes, sensitive scope verification process)
- Washington State MHMDA (Health Data Privacy Act) compliance requirements

---

## Flags

### Red Flags

- **F3 Google OAuth review timeline = binary risk to launch date.** Google sensitive scope verification = 2-4 שבועות סטנדרטי, יכול להגיע ל-6-8 אם application מסומן ל-manual security review. **Mitigation:** start verification day 1; have F1, F2, F4-F10 ready by week 3-4 so F3 integration completes immediately upon approval. אם review >5 שבועות, ship v0.9 ללא Google sync (Apple-only + manual export) ושחרר F3 ב-update תוך 2 שבועות.

- **62 working days solo full-time = 5-7 שבועות part-time** — tight against WWDC June 8 + summer launch window (June 22 - July 1). **Slippage of 1 week = launch מתחיל לתחרות עם Apple Intelligence iOS 27 announcement noise.** Mitigation: ruthless scope discipline (F1-F10 only); kill scope creep aggressively; v1.1 backlog ready to absorb "but we should also add..." impulses.

- **Founder's "90% of UI done" claim unvalidated.** Actual completion rate may be 60-75% when accounting for state management, edge cases, accessibility, dark mode. **Mitigation:** week 1 audit of UI completion (founder demos every screen ל-agent / advisor / co-founder); adjust estimates if gap surfaces.

- **WWDC June 8 platform risk.** Apple Intelligence + EventKit changes + Siri 2.0 calendar features may commoditize F1 (voice) and/or F4 (EventKit). **Mitigation:** war-room June 8-15; positioning shift ready ("ADHD-specific layer on top of Apple Intelligence"); cross-platform readiness reduces single-platform dependency.

- **LLM cost at scale unknown.** $0.10-0.30/user/mo estimated, but heavy brain-dump users (3-5x/week) at 60-90 שניות each could push toward $0.50-1.00/user/mo — material on $9.99 ARPU. **Mitigation:** monitor cost/user weekly; switch to Apple Speech + cheaper LLM (Haiku) if costs spike; cache common patterns.

- **iOS-only launch excludes ~40% of US Maya-persona** (Android users; Black/Latina women over-indexed on Android per `value-proposition.md`). Equity + TAM risk. **Mitigation:** Android v1.0 within 8-12 weeks of iOS launch; communicate timeline publicly.

- **Voice transcription accuracy for non-white-American-English speakers untested.** Aha moment may fail differentially across demographics. **Mitigation:** beta test with diverse cohort (3-5 AAVE / accented English speakers) before launch; always-visible text fallback.

### Yellow Flags

- **LLM API single-vendor risk.** OpenAI outage = product outage. **Mitigation:** abstract LLM behind interface; have fallback provider (Anthropic) configured + tested.

- **Voice-first UX assumes user environment allows speaking.** Quiet office / public transit / late-night-partner-sleeping edge cases. **Mitigation:** text fallback always one tap away; voice volume detection + "use text instead" prompt if ambient noise high.

- **Apple Speech requires iOS 10+**; older devices won't work. **Mitigation:** minimum iOS 16 target reasonable (94%+ of US iPhone users as of May 2026); communicate device requirements clearly.

- **30-day refund operationally costly** if rate >10%. Apple/Google IAP refund processing has constraints — founder may need to issue supplementary manual refunds. **Mitigation:** Stripe-style merchant of record consideration (RevenueCat handles); founder commits to never fight a refund.

- **Tiimo may ship two-way sync** before Planny launches (per `competitor-landscape.md` — public Nolt request). **Mitigation:** monitor Tiimo release notes weekly; if Tiimo ships first, sync wedge shifts to "free, included, well-designed" vs Tiimo's likely paid-tier rollout.

- **Indy by Shimmer free tier comparison** will surface in App Store reviews ("why pay when Indy is free?"). **Mitigation:** prepared answer in onboarding + landing page (per `positioning.md`): "We're not a coaching funnel. Two-way sync, voice depth, partner mode coming."

- **Tracy Otsuka podcast window closing** if competitor sponsors first. **Mitigation:** lock Tracy sponsorship within 30 days of launch ($800-1,500 from $1,500 budget).

- **Founder DM channel doesn't scale.** Works at 100 users; breaks at 5,000. **Mitigation:** graduated response model — personal DMs for first 500 users; office hours + community manager thereafter; never silent.

- **Apple Privacy Manifest iOS 17+ requirement** ל-third-party SDKs (OneSignal, Firebase, etc.). **Mitigation:** verify all dependencies have privacy manifests; switch to alternatives if missing.

- **Cross-platform decision (iOS-only vs iOS + Android)** changes total scope by 30-40%. **Decision required week 1.**
