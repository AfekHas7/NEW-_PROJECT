# Scorecard — Planny Final Assessment

**Phase:** Phase 8 — Validation (Scorecard)
**Project:** startup-validation (Planny)
**Date:** 2026-05-28
**Confidence:** Medium-High — הציון מבוסס על 7 dimensions שכל אחת מהן נשענת על Phase 3-7 evidence (Tier 1 + Tier 2 sources). הקרח הדק הוא: אפס validation אקטיבי של customer-paying-intent, retention assumption של D30=12% שהוא 3x מ-productivity benchmark של 4.1% ולא נתון אלא היפותזה, ו-WWDC June 8 (11 ימים מעתה) כ-binary external event שיכול לשנות 2-3 dimensions בו-זמנית.

---

## ה-Verdict הראשי

**Overall Score: 6.4 / 10**
**Recommendation: CONDITIONAL GO**

Planny הוא רעיון טוב מספיק כדי להצדיק את ההשקה — אבל לא רעיון "ברור". יש כאן שלושה דברים שנדירים לראות יחד: founder-market fit אמיתי (לא נרטיב — מצב פסיכיאטרי שאי-אפשר לזייף), wedge טכני מובחן (two-way OAuth ש-Tiimo לא משחררת כבר שנתיים על אף בקשת פיצ'ר פומבית), ותזמון תרבותי שעובד (62% נשי בקהל ADHD, +270% חיפושים, $46.97 productivity LTV הגבוה ביותר בכל הקטגוריות). יש כאן גם שלושה דברים שאסור להתעלם מהם: **תקרת שוק ריאלית של $50K ARR בשנה הראשונה** (לא venture-scale, לא יוצאת לדרכים אם המייסד רוצה $1M+ סלרי), **רטנציה ADHD לא ידועה ציבורית — הכל proxies מקטגוריות אחרות**, ו-**WWDC ב-11 ימים** שעלול להפוך חצי מה-MVP לפיצ'ר Apple חינמי. ה-recommendation היא לא "Go" אלא "Conditional Go" כי אם המייסד לא יעמוד ב-3 התנאים שמופיעים למטה תוך 30 ימים — המסקנה צריכה להיות לעצור, לא לדחוף קדימה. ההבחנה הזו לא סמנטית — היא ההבדל בין סטארטאפ ש-burn $1,500 חכם לבין סטארטאפ ש-burn 6 חודשי founder time על משהו שלא נבדק. הציון 6.4 הוא "להמשיך עם משמעת", לא "להמשיך באושר".

---

## Scorecard Table

| Dimension | Score (1-10) | Rationale |
|-----------|--------------|-----------|
| Problem severity | 8 | Pain hierarchy מתועדת מ-35+ verbatim quotes ב-customer-voice (Setup overwhelm "30 apps, abandoned 28", Time blindness "90% of tasks 4:51pm-4:58pm", Task initiation "paralyzed, unable to start"). 89% comorbidity → ה-pain הוא לא inconvenience אלא clinical anxiety trigger. ADHD search +270% global 2019-2023. **חולשה:** ה-pain מתועד דרך 50% WebFetch failures על Reddit — סינתזה, לא ציטוט ראשוני. |
| Market size | 5 | US ADHD apps TAM $773M (Market Growth Reports 2025, Medium). SAM "Maya late-dx women 25-40" $77-140M (Tier 2 extrapolation). **SOM Y1 ריאלי $15-50K ARR (High confidence) — זה bootstrap, לא venture.** Y1 base case projection 850 paying users / $53K ARR; Y3 projection $384K ARR לפני seed round אופציונלי. Israel TAM ceiling ~$140K — לא revenue engine. **לא רע, אבל לא דרמטי — זה ציון ריאלי, לא pessimistic.** |
| Competitive advantage | 6 | Onliness composite חזק: founder ADHD (Tiimo's Azari ND but operational not narrative; Inflow's Sachs is clinician not patient) + voice brain-dump <90s (Tiimo's Co-planner partial; no one unifies voice→AI→sync) + two-way Google OAuth (Tiimo's #1 Nolt request unresolved 2+ years) + 30-day refund (Inflow billing reputation moat). **חולשה:** Tiimo iPhone App of the Year 2025 = 12-24 months marketing oxygen. Saner.AI Techstars + Google Accelerator rising. Indy by Shimmer free, $3.5M parent. Window 9-18 months לפני שמתחרים סוגרים, או worse — Apple shippa אותו ב-WWDC. |
| Feasibility (Product/Tech) | 6 | 90% UI claimed by founder (unvalidated). MVP scope 10 features (F1-F10) at ~62 working days solo full-time, ~5-7 weeks part-time. Apple EventKit (S-M) + LLM API (mature) + StoreKit2 (mature) — manageable scope. **Red flag:** Google OAuth sensitive scope review = 2-4 weeks external dependency, can extend to 6-8 weeks if manual security review triggered. Solo founder, vibe coder, less native iOS experience. WWDC June 8 in 11 days could force re-architecture. "90% UI" claim is the bet — if it's actually 60-75%, timeline slips into Apple Intelligence shipping window. |
| Business model clarity | 7 | Pricing $9.99/$39.99/$59.99 locked, anchored against Tiimo $54/yr, Numo $59.99/yr (exact match — proven). Whitespace $7-10/mo confirmed across 14 competitors. 94% gross margin post Apple cut. Productivity LTV $46.97 (highest of any category, RevenueCat 2026). Weekly plans = 66% of productivity revenue (RevenueCat). Reinvestment compounding math works in Base scenario (D30 ≥12%). **חולשה:** D30 retention for ADHD audience unknown — entire model rests on hypothesis. Refund rate >15% breaks economics. Inflow's $11M paid spend means paid acquisition impossible → organic-only is mandatory not optional. iOS-only Y1 caps reach ~40%. |
| Founder-market fit | 8 | Founder has ADHD (publicly disclosed per intake סבב 3) — non-replicable trust capital, #1 sniff test in r/ADHDWomen ("is the founder ADHD?"). US trip for several months enables in-person validation (5-10 coffee chats per Experiment 5). Has product/UI/design chops (90% UI ready). Bilingual EN+HE for IL expansion. **חולשה:** Solo founder, no co-founder buffer. Comparing 3 startups — divided commitment risk (Assumption A16 marked CRITICAL existential). Vibe coder, less native iOS experience. No funded runway — depends on personal savings + 100% reinvestment. **Zero customer validation experience** — never run an interview, never gotten a "no" from a paying user. |
| Timing | 6 | Tailwinds genuine: ADHD search +270.5% globally 2019-2023 (YouGov Tier 1), 123% adult diagnosis increase (CDC NCHS Tier 1), 62% female ADHD online audience (YouGov), TikTok #ADHDinWomen 2.6B views (TikTok native Tier 1), Productivity LTV at record high $46.97 (RevenueCat 2026 Tier 1). Motion vacating consumer ADHD lane to B2B (Sep 2025). **Red flag:** **WWDC June 8, 2026 (11 days) is binary external risk.** Apple acquired Mayday Labs (Apr 2024) — 2+ years of AI scheduling tech inside Apple. iOS 27 reveal point. If Apple ships ADHD-aware AI scheduler → Planny's voice wedge + sync wedge commoditized at platform level. Tiimo App of Year 2025 halo (Dec 2025). Saner.AI Series Seed risk (6-12 months). Inflow $11M poisoning paid channels. Window 9-18 months. |
| **Overall** | **6.4 / 10** | **Conditional Go.** Problem severity (8) + Founder-market fit (8) drag the average up; Market size (5) drags it down toward bootstrap-reality, not venture-reality. Competitive advantage (6) + Timing (6) reflect real wedges within a real window — but neither is overwhelming. Business model (7) and Feasibility (6) are operationally viable but rest on unvalidated assumptions (D30 retention, Google OAuth approval, 90% UI claim). The score says: this is worth executing **if** the 3 conditions hold. It does not say "this will definitely work." |

### Scoring Logic
- **8-10:** Strong signal to proceed — compelling evidence
- **6-7:** Conditional proceed — specific conditions to validate first
- **4-5:** Significant concerns — run validation experiments before committing serious resources
- **1-3:** Recommend against proceeding in current form — explain pivots

---

## פירוט מפורט של כל dimension

### Problem Severity: 8 / 10

ה-pain כאן הוא לא inconvenience צרכני. הוא clinical — 89% comorbidity rate (anxiety 73-74%, depression 62-64% per ADDitude survey n=1,500 women). Setup overwhelm + time blindness + task initiation paralysis הם תסמיני executive dysfunction מתועדים. Maya חיה את ה-pain מספר פעמים ביום, כל יום, וכבר ניסתה 5-12 אפליקציות שנכשלו עליה. ה-cancellation pattern של "I felt like the failure" אחרי כל אפליקציה שננטשה הוא לא תיאור drift — הוא תיאור trauma response. הציון לא 9-10 כי **התיעוד הוא 50% snippet-based ולא ציטוט ראשוני**: WebFetch נכשל על Reddit, App Store, Trustpilot, ADDitude ב-50% מהזמן בזמן המחקר. הקול האמיתי של Maya נגיש דרך Medium long-form, planner-coach blogs, ו-snippets — לא דרך 700K המשתמשות של r/ADHDWomen ישירות. למידע הזה יש גבול, ויכול להיות שהשפה בקהילה יותר shame-driven ויותר frustrated מהמדיאן שתפסנו.

**Evidence FOR:**
- 35+ verbatim quotes ב-customer-voice.md (Tier 2-3 sources — Medium, ADDitude, JustUseApp, HuffPost, AFFiNE, JD Psychotherapy)
- 15.5M US ADHD adults (CDC NCHS MMWR Oct-Nov 2023, High confidence) — מסת משתמשים אמיתית
- 89% comorbidity rate (ADDitude survey n=1,500 women, Medium) — pain אינו discretionary
- Day-30 retention 4.1% productivity / 3.3% mental health = structural app-graveyard (RevenueCat / HCPLive Tier 1-2) — אנשים מבקשים תשובה ולא מוצאים אחת
- ADHD search +270% globally 2019-2023 (YouGov Tier 1)
- Tiimo Apple iPhone App of the Year 2025 + Inflow $11M Series A = שוק שמשקיעים מאמתים אותו

**Evidence AGAINST:**
- אפס ראיון לקוח אמיתי לפני התחלת הפיתוח. כל ה-pain מצוטט מ-secondary sources
- ה-pain documented through anglophone Western internet — לא ידוע אם זה נכון לאוכלוסיות אחרות (Black/Latina women under-represented in late-dx data)
- "Pain" אינו "willingness-to-pay" — Maya חיה במציאות של 30+ apps שננטשו. הסקפטיות שלה היא ה-pain עצמה
- WebFetch failed 50% — הקול האמיתי של r/ADHDWomen (700K) לא נכנס למחקר. הציטוטים הם מ-snippets, לא threads

### Market Size: 5 / 10

זה הציון שיכאב למייסד יותר מכל ציון אחר במסמך הזה, ולכן הוא כתוב הכי ישר. **השוק לא ענק. הוא לא הולך להיות ענק.** SOM Y1 ריאלי הוא $15-50K ARR, Y2 base $162K, Y3 base $384K. זה Sunsama-style $1.5M ARR bootstrap exit — לא Inflow $11M Series A path. אם המייסד עושה את החישוב לגבי ה-3 startups שהוא משווה ביניהם — Planny הוא לא הסטארטאפ עם ה-TAM הגדול ביותר. הוא הסטארטאפ עם founder-market fit ה-strongest והכי realistic-to-launch. הציון 5 כי השוק קיים ומתועד היטב ב-Tier 1, אבל הוא bootstrap-scale, לא venture-scale, וזה צריך להיות מובן ברור לפני שמשקיעים זמן.

**Evidence FOR:**
- US ADHD apps TAM **$773M (2025)** (Market Growth Reports Tier 2)
- 15.5M US ADHD adults (CDC NCHS 2023, High confidence)
- $77-140M SAM ADHD-specific late-dx women (Tier 2 extrapolation, Medium)
- Productivity LTV **$46.97** — highest of any category (RevenueCat 2026 Tier 1)
- ADHD apps CAGR 15-16% — double productivity general (8-10%)

**Evidence AGAINST:**
- SOM Y1 only **$15-50K ARR** — niche bootstrap, not VC-scale
- Israel TAM ceiling **~$140K ARR** — strategic anchor, not engine
- Analyst variance on ADHD apps market size: $0.5B to $7.7B (Tier 3) — direction reliable, absolute number not
- Y3 projection $384K ARR before any seed round — comfortable solo founder territory, not "build a company"
- Reclaim → Dropbox $40.2M exit comp at 320K users = $125/user enterprise value. Planny at 5K users Y2 = ~$625K theoretical exit (not realistic without significant growth)

### Competitive Advantage: 6 / 10

ה-Onliness composite אמיתי וברור — founder ADHD + voice-first + two-way OAuth + 30-day refund + persona narrow (late-dx women 25-40) = שילוב שאף מתחרה לא יכול לטעון בלי לשקר או בלי לעבור rebuild שלם. הציון לא גבוה יותר כי **כל wedge בפני עצמו אינו kill-shot**: Tiimo יכולה לשחרר two-way sync בכל רגע (היא יודעת — הבקשה ב-Nolt שלה 2+ שנים), Saner.AI יכולה לטעון voice-first אם תרים Series Seed בקרוב, Inflow יכולה לעבור על billing reputation עם הצהרה (אם תעז). ה-wedge הכי defensible הוא founder ADHD — וזה wedge פסיכולוגי, לא טכני. גם יש 8+ מתחרים ישירים בקטגוריה רוויה. Window 9-18 חודשים אמיתי, וה-clock רץ.

**Evidence FOR:**
- Onliness composite (founder ADHD + voice <90s + two-way OAuth + 30-day refund + no streaks + late-dx women persona narrow)
- Tiimo's documented unaddressed gaps (one-way sync per tiimo.nolt.io public for 2+ years; no partner mode; Android beta; "kid-coded" aesthetic alienates Maya 30+)
- Apple EventKit limitation creates real technical moat (Google OAuth direct, not iCloud bridge)
- Inflow billing reputation creates ethical wedge that competitors can't match without admitting prior behavior
- Tracy Otsuka podcast (8M downloads, 95% women, 25-40 demographic, US-skewed) currently unclaimed by competitors

**Evidence AGAINST:**
- Tiimo iPhone App of Year 2025 + 6,600+ testimonials + Apple editorial moat (12-24 months)
- Saner.AI Techstars + Google Accelerator + #1 in 5+ "best ADHD apps 2026" rankings — broader scope risk
- Indy by Shimmer free entering category (Jan 2026), $3.5M Shimmer parent funding
- WWDC June 8 Apple Mayday Labs absorption risk — Apple has had AI scheduling tech 2+ years internally
- Inflow $11M Series A poisoning Meta/TikTok auctions — paid acquisition unviable for Planny
- "Built by an ADHD adult" is non-renewable trust capital — if founder hides ADHD or contradicts narrative once, moat collapses immediately

### Feasibility (Product/Tech): 6 / 10

ה-claim של "90% UI done" לא אומת. אם נכון, MVP מסתיים ב-5-7 weeks part-time, וה-launch window June 22 - July 1 הוא ריאלי. אם בפועל זה 60-75% (סביר כשמכניסים state management, edge cases, accessibility, dark mode), ה-timeline נדחק ל-8-10 weeks וה-launch נכנס ל-Apple Intelligence announcement noise. ה-Google OAuth review הוא 2-4 weeks external dependency שיכול להגיע ל-6-8 שבועות אם application מסומן ל-manual security review — זה ה-binary critical path היחיד שהמייסד לא שולט בו. הציון לא 4-5 כי המייסד הוא הקהל היעד ויש לו design instinct (90% UI claim is the bet), ה-LLM costs ידועים ויציבים, ו-Apple EventKit + RevenueCat + Supabase כולם mature stacks. הציון לא 8-9 כי solo founder + vibe coder + WWDC dependency + Google review queue = 4 single-points-of-failure ב-execution.

**Evidence FOR:**
- 90% UI done (per founder claim — UNVALIDATED)
- 5-7 weeks part-time build remaining (per mvp-definition.md estimate)
- Google OAuth + voice + sync = manageable scope for solo vibe-coder with AI assist
- LLM costs sustainable at projected scale ($0.10-0.30/active user/mo)
- Apple StoreKit2, EventKit, OneSignal free tier, RevenueCat free tier <$2.5K MTR — all mature
- Apple Small Business Program (15% fee post-approval) achievable

**Evidence AGAINST:**
- Solo founder, vibe coder, less native iOS experience
- Google OAuth review timeline uncertain (2-4 weeks standard, 6-8 weeks possible) — binary critical path
- 90% UI claim unvalidated (likely 60-75% real once edge cases, state management, accessibility, dark mode counted)
- WWDC June 8 (11 days) could force re-architecture (EventKit changes, Siri 2.0 integration, Apple Intelligence Calendar features)
- Voice transcription accuracy for non-white-American-English untested (equity + UX risk)
- LLM cost runaway from heavy users (20+ brain-dumps/mo could push to $1+/user/mo → gross margin compression)

### Business Model Clarity: 7 / 10

זה החלק הכי בריא של המודל. Pricing locked ב-whitespace מאומת ($7-10/mo cluster confirmed across 14 competitors), Numo proves $59.99/yr works, Inflow $96/yr is the trust ceiling, Tiimo $54/yr is the floor. 94% gross margin post Apple cut, 95% post SBP. Productivity LTV $46.97 highest of any category. Reinvestment compounding math works in Base scenario. Refund + 2-tap cancel + 30-day no-Q is a brand asset that competitors can't match without admitting prior dark patterns. הציון לא 8-9 כי **D30 retention for ADHD audience is unknown publicly** — entire model rests on hypothesis (4.1% productivity baseline, 16% best-in-class ceiling, 12% target). אם D30 בפועל <6%, reinvestment compounding מתכווץ במקום להתרחב, runway exhausts תוך 6-9 חודשים, וגם Pessimistic-2 לא יחזיק. אם refund rate >15%, brand promise becomes financial drag. iOS-only Y1 caps reach ל-~60% of US Maya (US Android ~40%, especially Black/Latina women).

**Evidence FOR:**
- Pricing locked in whitespace ($7-10/mo cluster, Numo exact match $59.99/yr)
- Productivity LTV $46.97 — highest of any category (RevenueCat 2026 Tier 1)
- Weekly plans = 66% of productivity revenue (RevenueCat 2026 Tier 1)
- 94% gross margin Y1 / 95.6% Y2 post-SBP
- Reinvestment compounding feasible in Base scenario (D30 ≥12%)
- Apple SBP eligibility automatic <$1M ARR → +21% net revenue per user from Y2

**Evidence AGAINST:**
- D30 retention unknown for ADHD audience — all benchmarks are proxies (productivity 4.1%, mental-health 3.3%)
- Refund rate >15% breaks model — Inflow precedent 5-8% with fuzzy 7-day refund; Planny 30-day generous policy could hit 15-25%
- Inflow's $11M paid spend prices out paid channels — organic mandatory not optional
- iOS-only Y1 caps reach ~60% of US Maya
- 60-day working capital gap (Apple holds 30-45 days + 30-day refund window) — founder needs personal $2,500+ buffer above seed
- Trial-to-paid declining industry-wide (46% → 33% YoY, Recurly)

### Founder-Market Fit: 8 / 10

זה הציון הגבוה ביותר במסמך, ולא במקרה. **המייסד הוא הקהל היעד**, לא בנרטיב — בפסיכיאטריה. אובחן ב-ADHD, חי את ה-pain, ניסה את Tiimo / Sunsama / Motion / Apple Reminders, ננטש על-ידם, ובנה מה שהוא רצה. **ה-#1 sniff test ב-r/ADHDWomen על כל אפליקציה חדשה** הוא "is the founder ADHD?" — ה-answer הוא yes, וזה non-replicable. נסיעת ה-US לכמה חודשים מאפשרת 5-10 in-person interviews בעלות אפסית — ה-highest leverage validation experiment. יש לו design/product chops (90% UI claim is the bet). בילינגוויסטיות EN+HE לקראת IL expansion. הציון לא 9-10 כי **3 הסיכונים החמורים שלא נפתרים בהיותו ADHD**: (1) **solo founder = single point of failure** — אם הוא חולה/burnout/Israeli reservist call-up = product velocity collapses; (2) **comparing 3 startups simultaneously** — divided commitment risk (Assumption A16 marked CRITICAL existential); (3) **zero customer validation experience** — מעולם לא הריץ ראיון, מעולם לא קיבל "no" ממשלם פוטנציאלי. הוא בעל ADHD שבונה ל-ADHDers, אבל אין לו ניסיון עסקי באימות ביקוש.

**Evidence FOR:**
- Founder has ADHD himself — strong unique angle, publicly disclosed per intake סבב 3
- Will be in US for several months — enables in-person validation (Experiment 5, highest-leverage in playbook)
- Can be public face of brand (TikTok / founder content, build-in-public)
- Has UI / design / product chops (90% UI ready claim)
- Bilingual EN+HE for IL expansion
- Will pay ADHD-disclosure premium: every Maya in r/ADHDWomen asks "is the founder ADHD?" first

**Evidence AGAINST:**
- Solo founder, no co-founder buffer
- **Comparing 3 startups → divided commitment risk** (Assumption A16 marked CRITICAL existential in tracker)
- Less native iOS experience (vibe coder, AI-assisted dev)
- No funded runway (depends on personal savings + 100% reinvestment)
- **Zero customer validation experience yet** — never run an interview, never gotten a "no" from a paying user
- Israeli reservist risk (per market-analysis.md flag)
- Founder DM accessibility ("I read every email") works at 100 users, breaks at 5,000

### Timing: 6 / 10

הציון הזה הכי תלוי ב-event יחיד בכל המודל — **WWDC June 8, 2026, בעוד 11 ימים**. ה-tailwinds אמיתיים ומאומתים ב-Tier 1: ADHD search +270%, 62% female audience, 123% adult diagnosis increase (CDC), TikTok #ADHDinWomen 2.6B views, Productivity LTV $46.97 record high, Motion vacating consumer lane. ה-headwinds גם הם אמיתיים: Tiimo iPhone App of Year 2025 halo (12-24 חודשים marketing oxygen), Saner.AI Techstars rising, Indy by Shimmer free, Inflow $11M poisoning paid channels. אבל **ה-binary risk הוא Apple**: 2+ שנים של AI scheduling tech בתוך Apple אחרי רכישת Mayday Labs (April 2024), WWDC הוא ה-natural reveal point. אם Apple shippa heavy AI calendar + Siri 2.0 ADHD-aware — Planny הופך ל-"ADHD layer on top of Apple Intelligence" בטוב, או commodity ברע. הציון לא 7-8 כי ה-binary risk מטה דרסטית. הציון לא 4-5 כי גם אם Apple shippa heavy, יש ADHD-specific UX layer ש-Apple לא יבנה (transitions, buffers, gentle re-planning, partner mode, late-dx women narrative). Window 9-18 חודשים אמיתי, וה-clock רץ.

**Evidence FOR:**
- ADHD search +270.5% globally 2019-2023 (YouGov 20-country Signal Tier 1)
- 62% female ADHD online audience (YouGov)
- 123% adult diagnosis increase CDC NCHS 2023 (vs +26% children, Tier 1)
- TikTok #ADHDinWomen 2.6B views (TikTok native)
- Productivity LTV at record high $46.97 (RevenueCat 2026 Tier 1)
- Motion vacating consumer ADHD lane (Sep 2025, B2B pivot)
- Reclaim → Dropbox $40.2M exit comp (Jul 2024, SEC 8-K Tier 1)
- On-device LLM costs collapsed → solo founder can build AI-native at $1,500

**Evidence AGAINST:**
- **WWDC June 8 (11 days) Apple Intelligence announcement** — binary external risk; Apple acquired Mayday Labs (Apr 2024); iOS 27 reveal
- Tiimo iPhone App of Year 2025 — 12-24 month marketing oxygen + Apple editorial moat
- Saner.AI Techstars + Google Accelerator rising — broader scope competitor
- Indy by Shimmer free (Jan 2026) — $3.5M parent funding
- Inflow's $11M paid spend saturating channels — paid acquisition not viable
- Trial-to-paid declining industry-wide (46% → 33% YoY, Recurly)
- 40% of agentic AI projects to be cancelled by 2027 (Gartner) — hype trough warning

---

## ה-Verdict הברור

### Final Recommendation: CONDITIONAL GO

**זה לא קל לכתוב conditionally בלי להישמע כמו ניסיון להתחמק מהחלטה.** אז בלי להתחמק: Planny הוא רעיון טוב מספיק כדי להצדיק 30-60 ימי השקעה נוספים, אבל לא מספיק טוב כדי לדלג על שלושה תנאים שהמייסד חייב לעמוד בהם. אם הוא לא מסוגל לעמוד בהם — המסקנה צריכה להיות לעצור, לא לדחוף קדימה. ה-3 התנאים לא טקסיים — הם ה-difference between סטארטאפ ש-burn $1,500 חכם לבין סטארטאפ ש-burn 6 חודשי founder time על משהו שלא נבדק.

**הנקודה הכי חשובה במשפט אחד:** Planny מספיק טוב כדי להשיק, אבל ה-real test הוא לא ה-launch — הוא ה-Day 30 retention cohort בחודש 2-3 ואז ה-Day 90 cohort בחודש 3-4. אם D30 retention <6%, המודל הפיננסי נשבר תוך 6-9 חודשים בלי קשר ל-MRR בחודש 1. ה-existential KPI הוא לא acquisition. הוא retention. וזה לא ידוע כרגע.

**מה זה אומר בפועל:** המייסד צריך להשיק את Planny ביוני 22 - יולי 1 (post-WWDC), להפעיל את 3 התנאים, ולקבל החלטה אמיתית בחודש 3 על-בסיס נתוני retention אמיתיים — לא על-בסיס "feeling" של "זה הולך לעבוד". אם בחודש 3 D30 retention <6% — kill the project gracefully (honor refunds, shut infrastructure, free the founder time ל-startup 2 או 3). אם 6-10% — engineer retention features ב-2 שבועות, pause acquisition spend. אם ≥10% — accelerate Tracy network effect, plan Y2 (Android, Hebrew, partner mode), consider seed round optionality.

### If GO / CONDITIONAL GO — The 3 Conditions

1. **In-person interviews in US trip (Experiment 5)** — 5-10 coffee chats with late-diagnosed ADHD women 25-40 in NYC/NJ/Brooklyn/Jersey City. screen by 3 questions in DM (When were you diagnosed? What planner apps have you tried? Age + city). 30-min each, batch in 2 days. Validate ≥6/10 willingness to pay $9.99 + ≥7/10 voice wedge resonance + ≥5/10 say they'd install. **Without this, the Maya persona remains inferred — not validated.** זה ה-highest-leverage experiment בכל ה-playbook.

2. **Defer launch to post-WWDC June 8** — with 3 pre-written launch versions:
   - **Version A (60-70% probability):** Apple doesn't ship AI scheduler → proceed June 22 as planned, positioning unchanged
   - **Version B (20-30%):** Apple ships generic AI scheduler/Siri productivity → delay launch 1 week to July 1, reposition to "ADHD layer on top of Apple Intelligence"
   - **Version C (5-10%):** Apple ships ADHD-aware scheduler → pause launch entirely; pivot evaluate within 48hr (AuDHD niche / Couples mode / B2B coaches / Perimenopausal-ADHD)

3. **Direct Google Calendar OAuth in 3-4 weeks** — submit to Google sensitive scope verification **Day 1** (today). Review timeline 2-4 weeks standard, 6-8 if manual security review triggered. **This is the binary critical path the founder doesn't control.** Have manual `.ics` import fallback designed in parallel — if review extends past 5 weeks, ship v0.9 without Google sync (Apple-only + manual import), release F3 update 2 weeks post-approval.

### If GO — The Path Forward (12 weeks)
- **Week 1-2 (May 29 - Jun 11):** Pre-launch validation — Landing page live (Carrd $50), Twitter poll, Reddit r/ADHDWomen value post (NO promo), Tracy Otsuka outreach email Day 1, 80 micro-creator DMs, Google OAuth verification submitted, Apple SBP application, Privacy Policy + MHMDA drafted
- **Week 3-4 (Jun 12 - Jun 25):** TestFlight closed beta 50-100 from waitlist, WWDC June 8 decision point lock launch version A/B/C, Google OAuth final dev + QA, App Store submission (5-7 day review)
- **Week 5-6 (Jun 26 - Jul 9):** Public launch June 22 or July 1, ProductHunt + HackerNews, daily TikTok posts, Tracy Otsuka episode airs week 6 (if booked), Apple Search Ads test $50/day
- **Week 7-12 (Jul 10 - Aug 20):** Iterate based on user feedback, scale ASA from $50 to $100/day on best-performing keywords, kill <$40 CAC keyword groups, first Day-30 retention measurement (Week 8 cohort), Day 90 validation checkpoint — Green/Soft Kill/Hard Kill decision per kill-criteria

### If STOP — The Honest Path
אם המייסד לא יכול / לא רוצה להתחייב לתנאים, או אם הוא בכלל מבין שהוא צריך להתמקד באחד מה-2 startups האחרים שלו במקום ב-Planny:
- ה-2 startups האחרים שלו ראויים לאותו rigorous validation. ה-methodology של ה-Phase 1-8 plan הזה יחול עליהם כמעט אחד-לאחד (אם הם consumer mobile apps עם beachhead persona)
- ה-Planny work אינו מבוזבז — המתודולוגיה (Lean Canvas, Positioning, Value Proposition, MVP Definition, Financial Projections) חוזרת על עצמה ב-startup 2 ו-3
- אם יש pre-launch waitlist signups — לכבד את ה-expectations (email פרישה כנה: "Hi — Planny is paused. Here's why."), לא ghost
- אם יש early TestFlight users — תודה, לבטל גישה ב-30 day notice, אין refund חובה כי לא נגבה כסף

---

## Comparison Framework (for Founder's 3-Startup Decision)

When the founder applies this same scorecard to Startup 2 and Startup 3:

| Criterion | Planny Score | Startup 2 (RSVP-AI) | Startup 3 |
|-----------|--------------|-----------|-----------|
| Problem severity | 8 | 6 | — |
| Market size | 5 | 4 | — |
| Competitive advantage | 6 | 2 | — |
| Feasibility | 6 | 6 | — |
| Business model | 7 | 4 | — |
| Founder-market fit | 8 | 4 | — |
| Timing | 6 | 5 | — |
| **Overall** | **6.4 / 10** | **4.3 / 10** | **—** |

> **Startup 2 (RSVP-AI) filled 2026-05-29.** ראה `startup-2/06-validation/scorecard.md`. Verdict: NO-GO במתכונת הנוכחית. **Planny מנצח 6.4 מול 4.3, ב-6 מתוך 7 ממדים.** הפער הגדול: Competitive advantage (6 מול 2 — ל-Planny onliness אמיתי, ל-startup-2 אין חפיר) ו-Founder-market fit (8 מול 4 — ADHD non-replicable מול "מפיק לשעבר"). זה מאשר את התחזית שבסעיף האזהרה למטה: FMF הוא ה-amplifier — startup-2 הוא market-driven והמייסד לא חי את הכאב.

**Decision rule:** Pick the highest-scored. If tied: pick the one with highest Founder-market fit + Timing combined. If still tied: pick the one closest to launch (lowest opportunity cost — less founder time at risk).

**אזהרה חשובה:** **Planny מקבל 8/10 ב-Founder-Market Fit חלקית בגלל שמייסד ה-ADHD הוא non-replicable advantage.** אם Startup 2 או 3 גם מבוססים על personal pain של המייסד, יקבלו גם הם 7-8. אם הם opportunistic / market-driven אבל המייסד לא חי את הכאב — הם יקבלו 4-5 ב-FMF, גם אם השאר חזק. **FMF הוא ה-amplifier הכי גדול בציון הסופי לבחירה בין סטארטאפים — לא הציון הגבוה ביותר ולא המודל הכי קל לבנייה.** מייסד שלא חי את הכאב לא יחזיק 12-24 חודשים של slog לפני PMF.

---

## Anti-Pattern Check

האם ה-agent מזהה anti-patterns? (Per Honesty Protocol):

- **🟢 Solution looking for a problem** — NO (Maya pain validated in research; founder lives the pain himself; 35+ verbatim quotes; CDC 15.5M US adults with ADHD; ADHD search +270%; Tiimo+Inflow+Numo proven market exists; Reclaim→Dropbox $40.2M exit comp)
- **🟡 Boiling the ocean** — MITIGATED (Maya beachhead locked: late-dx US women 25-40 NYC/NJ; anti-targets explicitly defined — teens, enterprise, severe-symptom users, neurotypical productivity enthusiasts; persona-discipline value enforced; original intake claim of "for everyone" rejected in Phase 1)
- **🟢 Premature scaling** — NO (Y1 bootstrap, no infrastructure overbuild; iOS-only at launch; Android deferred to Y2 M1; Hebrew RTL deferred to Y2 M6; no hires until $5K MRR threshold; no VC raise planned pre-PMF; Sunsama-style $1.5M ARR bootstrap path)
- **🟢 Vanity metrics** — NO (paying users + retention + refund tracked; not downloads; not waitlist signups as primary signal; D30 retention defined as existential KPI; LTV/CAC tracked; install-to-paid funnel measured; ARR not MAU as north star)
- **🟡 Building in stealth too long** — MEDIUM (founder hasn't done user research; zero customer interviews pre-launch; relying on inferred demand signals — CDC prevalence, market existence, Reddit observation; **mitigated by waitlist landing page Experiment 1 + US trip Experiment 5**; **NOT mitigated:** founder still building before validating willingness-to-pay from real Maya)
- **🟢 Ignoring unit economics** — NO (LTV/CAC analyzed in depth; refund rate sensitivity modeled; LLM cost/user/mo budgeted; Apple SBP eligibility planned; gross margin tracked; reinvestment compounding math documented; pessimistic scenario explicitly named — Pessimistic-2 retention collapse → hard kill)

**Net assessment of anti-pattern profile:** Healthy. 2 yellow flags (Boiling the Ocean — mitigated; Building in Stealth — partial mitigation via Experiment 5). 4 green. **No red anti-pattern flags.** This is unusual — most founders fail 2-3 anti-patterns badly. Planny's documentation shows discipline in scope, persona, metrics, and unit economics. The remaining yellow on stealth/customer research is the #1 thing to fix in next 30 days.

---

## The Single Most Important Thing for the Founder to Know

**ה-test האמיתי של Planny הוא לא ה-launch — הוא ה-Day 30 retention בחודש 2-3.** אם בחודש 2 cohort retention <6% — ה-model נשבר תוך 6-9 חודשים בלי קשר לכמה paying users יש לך בחודש 1, וגם אם Tracy Otsuka מסכימה להעצים, וגם אם ה-WWDC עובר בלי תקיפת Apple. אם בחודש 2 cohort retention ≥10% — יש לך עסק bootstrap-able ל-$300-500K ARR ב-3 שנים, וזה בסדר גמור אם זה מה שאתה רוצה. רטנציה היא משתנה ה-#1 הקיומי. CAC לא ה-#1. תמחור לא ה-#1. פיצ'רים לא ה-#1. **רטנציה.** אתה צריך להתחייב מראש — ל-kill-criteria.md, לעצמך, ולמסמך הזה — שאם D30 בקוהורט חודש 2 <6% — אתה עוצר. בלי "let's try harder". בלי "let's give it 3 more months". אם אתה לא יכול להתחייב לזה — אל תשיק את Planny. תבחר אחד מה-2 startups האחרים שלך, או תחזור לעבודה ותחשוב ברצינות.

---

## Strategic Connections
- ראה כל קבצי Phase 3 — `01-discovery/` (market-analysis.md, target-audience.md, competitor-landscape.md, industry-trends.md, confidence-dashboard.md)
- ראה כל קבצי Phase 4 — `02-strategy/` (lean-canvas.md, positioning.md, value-proposition.md, business-model.md, go-to-market.md)
- ראה כל קבצי Phase 5 — `03-brand/` (mission-vision-values.md, tone-of-voice.md, brand-personality.md)
- ראה כל קבצי Phase 6 — `04-product/` (mvp-definition.md, feature-prioritization.md, user-journey.md)
- ראה כל קבצי Phase 7 — `05-financial/` (revenue-model.md, cost-structure.md, projections.md)
- ראה `validation-playbook.md` ל-13 experiments מסודרים cheapest→most expensive
- ראה `assumptions-tracker.md` ל-25 assumptions עם confidence levels + test plans
- ראה `01-discovery/research-gate.md` ל-Phase 3 verdict (YELLOW LIGHT 6.5/10) — **this scorecard supersedes it (6.4/10, CONDITIONAL GO)**. ה-revised verdict כמעט זהה כי ה-Phase 4-7 documents חיזקו את ה-positioning ו-product clarity אבל גם הוסיפו רבדים של risk (Apple SBP dependency, Google OAuth queue, 60-day working capital gap, retention as #1 existential)

## Sources

**Aggregate Tier counts across Phase 3-8:**
- **Tier 1 (government, analyst, academic, primary regulator):** ~32 unique citations
  - CDC NCHS MMWR 2023, CDC Data Brief #543 Dec 2025
  - RevenueCat State of Subscription Apps 2025 + 2026 (115K+ apps, $16B+ revenue)
  - Adapty State of In-App Subscriptions 2025 + 2026
  - AppTweak 2026 Apple Ads Benchmarks
  - Recurly subscription benchmarks (67M subscribers)
  - Apple Developer official (App Store Connect, Small Business Program, EventKit)
  - Google Play official + Google Calendar API documentation
  - SEC 8-K Dropbox → Reclaim.ai $40.2M acquisition Jul 2024
  - FDA General Wellness 2026 guidance
  - WA RCW 19.373 (MHMDA) + FTC HBNR final rule + IAPP Israel Amendment 13
  - PLOS One 2025 UBC TikTok #ADHD academic study
  - PMC 5-year ADHD search trends study
  - YouGov 20-country Signal Report (+270.5% ADHD search 2019-2023)
  - Gartner Aug 2025 + Jun 2025 (agentic AI predictions)
  - Rock Health 2025 Year-End funding report
  - Apple App Store Awards 2025 (Tiimo iPhone App of the Year)
  - Daring Fireball, AppleInsider, 9to5Mac, MacRumors, Bloomberg (WWDC + iOS 27)
- **Tier 2 (specialized industry, legal advisories):** ~78 unique citations
  - TechCrunch (Inflow Series A $11M, Shimmer $2.2M, Lately launch, Dropbox-Reclaim)
  - Crunchbase, Tracxn, PitchBook (Saner.AI Techstars + Google Accelerator)
  - First Page Sage, ChartMogul (trial conversion 18-25% opt-in, 49-60% opt-out)
  - BusinessDojo, Mapendo (NA ARPU $6.20/mo)
  - HCPLive, Wallace PhD (mental health app retention 3.3% D30)
  - Amraandelma 2025 (productivity D30 4.1%)
  - ChoosingTherapy Inflow review (billing reputation)
  - 42matters (Israel app market statistics)
  - Cooley, IAPP, Wilson Sonsini, Alston & Bird, Faegre Drinker (legal/regulatory)
  - SARAL case study (Sunsama 600+ creators + How to ADHD)
  - Octopus Ventures blog (Inflow channel mix)
  - Tracy Otsuka — ADHD for Smart Ass Women podcast (8M downloads, 150K monthly)
  - ADDitude (1,500-respondent menopause survey, advertising rates)
  - Sifted (Tiimo profile, B2B plans, downloads)
- **Tier 3 (community / reviews, used with skepticism):** ~98 unique citations
  - Medium long-form ADHD-planner writeups
  - JustUseApp Tiimo + Inflow reviews
  - Capterra Sunsama reviews (mobile read-only "Achilles' heel")
  - Trustpilot Inflow snippets (billing complaints)
  - Reddit r/ADHDWomen + r/ADHD via search snippets (50% WebFetch failure rate)
  - ProductiveWithChris (Motion shame UX review)
  - AFFiNE blog (object permanence quotes)
  - HuffPost ADHD tweets roundup (viral 4:51pm-4:58pm)
  - The Vibe With Ky (Indy by Shimmer review, Jan 15 2026)
  - Tiimo Nolt feature request board (tiimo.nolt.io two-way sync request public 2+ years)

**WebFetch success rate:** ~30% (mostly Tier 1 government + Apple/Google official + RevenueCat). **WebFetch failure rate:** ~50% (Reddit, Trustpilot, Capterra, ADDitude, App Store reviews, JustUseApp — i.e., almost every direct customer voice source). **Direct Reddit thread access:** ~5%. **Implication:** The research is research-firm-grade on demographics, regulation, competition, and pricing. It is significantly weaker on raw verbatim voice of the Maya persona. **Pre-launch validation via Experiment 5 (US coffee chats) and Experiment 3 (Reddit value post) is mandatory to close this gap.**

## Flags

**Red Flags:**

1. **WWDC June 8, 2026 (11 days from scorecard) is binary external risk.** Apple acquired Mayday Labs April 2024 — 2+ years of AI scheduling tech inside Apple. iOS 27 natural reveal point. If Apple ships ADHD-aware AI scheduler at WWDC keynote, Planny's voice wedge + sync wedge commoditized at platform level within 90 days. **Mitigation: war-room June 8-15; 3 launch versions pre-written; positioning shift ready to "ADHD layer on top of Apple Intelligence".**

2. **Day-30 retention unknown for ADHD audience — model breaks if <6%.** No public ADHD-specific cohort data. Productivity benchmark 4.1%, mental-health 3.3%. Planny target 12% is hypothesis built on anti-shame UX + voice wedge + weekly cadence + ADHD-native delivery. **First reliable signal is Month 2-3 cohort behavior. Founder must agree pre-launch to hard-kill criteria if D30 <6% — no "let's run it longer" exceptions.**

3. **Zero customer validation pre-launch.** Founder has spoken to zero late-diagnosed Maya women about willingness-to-pay $9.99/mo for Planny. All persona is inferred from research, not validated by paying intent. **Mitigation: Experiment 5 (US coffee chats) is highest-leverage validation in entire playbook. Without it, persona remains inferred.**

4. **3-startup divided commitment risk.** Founder is comparing 3 startups simultaneously. Assumption A16 marked CRITICAL existential in tracker. **Mitigation: this scorecard exists to enable apples-to-apples comparison. Founder must self-evaluate Day 30, 60, 90 — and pivot decisively if Planny is not the clear winner.**

5. **$1,500 budget in saturated category with Inflow $11M paid spend poisoning auctions.** Paid acquisition (Meta, TikTok, Google) unviable for Planny. **Organic-first is not a strategy choice — it's a mathematical necessity. If founder cannot create 3-5 pieces of organic content/week, there is no distribution model.**

6. **Refund rate >15% breaks unit economics.** 30-day no-Q refund is brand promise but financially aggressive. Inflow precedent 5-8% refund/dispute with fuzzy 7-day refund. Planny generous 30-day policy could hit 15-25% if onboarding fit poor. **Mitigation: sessions-gated refund (<10 sessions/30 days); monitor weekly from Month 1.**

7. **Google OAuth sensitive scope verification = binary critical path.** 2-4 week standard review, 6-8 weeks if manual security review triggered. **Mitigation: submit Day 1 (today); ship v0.9 Apple-only + manual import if review extends past 5 weeks.**

8. **Founder DM accessibility ("I read every email") is non-scalable architecture.** Works at 100 users; breaks at 5,000. Trust signal that must transition to graduated response model by $10K MRR.

**Yellow Flags:**

1. **Tiimo iPhone App of the Year 2025** — 12-24 months Apple editorial moat + 6,600+ testimonials + 500K active users. Marketing oxygen unfair to Planny.

2. **Saner.AI Techstars + Google Accelerator + #1 in "best ADHD apps 2026" rankings.** If they close Series Seed ($5-15M) in Q3 2026, marketing surge will define the category before Planny can claim it.

3. **Indy by Shimmer free (Jan 2026)** + $3.5M Shimmer parent funding. "Why pay when Indy is free?" objection on every TikTok comment.

4. **Israel TAM ceiling ~$140K ARR** — strategic anchor, not revenue engine. Don't build projections that depend on IL.

5. **WebFetch 50% failure rate on customer voice sources** (Reddit, Trustpilot, ADDitude, App Store reviews). Persona language map is research-firm-grade synthesis but not verbatim community capture.

6. **iOS-only Y1 launch excludes ~40% of US Maya** (Android users; Black/Latina women over-indexed on Android per equity analysis).

7. **LLM cost runaway risk** — heavy users (20+ brain-dumps/mo) could push to $1+/user/mo → compress gross margin from 95% to ~85%. Soft rate-limit mandatory in v1.

8. **60-day working capital gap** (Apple holds 30-45 days + 30-day refund window). Founder personal runway must cover Months 1-3 OpEx ($1,700+) on top of $1,500 seed deployment. If personal runway exhausted before M7, model collapses regardless of MRR.

9. **Apple Small Business Program (15% fee) eligibility may not be granted immediately** — if denied/delayed, Y1 net revenue per user drops 21%; material to reinvestment compounding speed.

10. **Founder content load (30% of time) impacts product velocity.** Solo founder + ADHD founder energy management + 25-30 hr/week pace for 12 months without burnout = real burnout risk (Assumption A15).

**Green Signals (counterbalancing — not in original Red/Yellow request but worth noting):**

1. Founder ADHD = non-replicable trust capital — verified per intake סבב 3, public disclosure planned
2. 62% female ADHD audience + 270% search growth + 2.6B TikTok views — momentum is real
3. Productivity LTV $46.97 — highest of any category (RevenueCat 2026 Tier 1)
4. Weekly plans = 66% of productivity revenue — Planny's wedge is exactly where the money is
5. Tracy Otsuka podcast (8M downloads, 95% women, 25-40 demographic) currently unclaimed
6. Apple EventKit limitation creates real technical moat (direct Google OAuth defensible 6-12 months)
7. Reclaim → Dropbox $40.2M exit comp validates that bootstrap ADHD scheduling can exit at 8-figure
8. Sunsama bootstrapped to $1.5M ARR without VC — proves path exists
9. Motion vacating consumer ADHD lane to B2B = one less direct competitor in beachhead
10. US trip enables in-person validation at $50-150 cost — Experiment 5 is the highest-leverage data Planny will ever get
