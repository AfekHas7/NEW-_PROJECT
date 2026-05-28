# Industry Trends — Planny

**Phase:** Phase 3 Synthesis
**Project:** startup-validation (Planny)
**Date:** 2026-05-28
**Confidence:** Medium-High (Tier-1 sources מאשרים את ה-macro story — CDC על ADHD, Gartner על AI agents, Rock Health על funding, Apple על Tiimo. Tier-2/3 חלוקים על גודל שוק ה-ADHD apps. WWDC 2026 ב-10 ימים — חלק מהתחזיות עוד יתחדדו)

---

## תקציר עיתוי

עכשיו זה הרגע — אבל החלון לחוץ. ב-2025-2026 הצטלבו ארבעה גלים בלתי-תלויים: ה-CDC הוציא ב-Dec 2025 את העדכון הראשון מזה 20 שנה על שכיחות ADHD במבוגרים (6% מהמבוגרים בארה"ב, **+123% עליה באבחנות מבוגרים** מול +26% בילדים); Apple הכתירה את Tiimo כ-iPhone App of the Year 2025 — endorsement של קטגוריית neurodivergent planners; on-device LLMs (Apple Foundation Models, Gemini Nano) הפכו ל-API נגיש שמאפשר ל-solo founder לבנות AI native ב-$1,500 במקום $10M; ו-Dropbox רכשה את Reclaim.ai ב-$40.2M (יולי 2024) — comp ישיר ש-AI scheduling מייצרת exit ב-8 ספרות גם בלי קנה מידה ענק. ה-tailwinds מאומתים Tier-1 וברמת הסיכוי הכי גבוהה שהקטגוריה ראתה. ה-headwinds: WWDC ב-June 8 2026 (בעוד ~10 ימים) צפוי להציג Apple Intelligence scheduling מבוסס רכישת Mayday Labs; Gemini Spark כבר חי מ-May 2026 עם MCP integrations; Tiimo עם 500K משתמשים ו-halo של Apple; Motion עם $60M ו-$550M valuation; Inflow עם $11M war chest. חלון הפעולה לקטגוריה אנכית ADHD-specific: **9-12 חודש להקמת moat טכני, 24-48 חודש לפני שגנריקה גוברת על ADHD-UX**. נטו: עיתוי טוב, בלחץ זמן, חובה wedge חד.

## מגמות מאקרו

### עליית מודעות וגילוי ADHD
- **CDC Data Brief #543 (Dec 2025):** 6% מהמבוגרים בארה"ב מאובחנים — ~15.5M אנשים. עדכון ראשון מזה 20 שנה.
- **+123% עליה באבחנות מבוגרים** מול +26% בילדים — אבחנות מבוגרים גדלות פי 4.6.
- **55.9% מהמבוגרים עם ADHD לא אובחנו עד גיל 18** — קוהורט late-diagnosed ענק שמחפש פתרונות באופן אקטיבי.
- חיפושי "ADHD" גלובלית: **+270.5% (YouGov 2019-2023, 20 מדינות)**.
- "late diagnosed ADHD" = breakout term; adult-women referrals +344% (2007-2016, מאיץ).
- Stage: Growing → Peak awareness
- Impact: **tailwind כבד** — Planny לא צריך ליצור ביקוש, רק לתפוס אותו.

### Mainstreaming של ADHD ב-Social
- TikTok: Top-100 #ADHD videos = **~500M צפיות מצטברות**, ממוצע 5.47M לסרטון (PLOS One 2025, UBC).
- #ADHD = ההאשטאג הבריאותי ה-7 בפופולריות ב-TikTok.
- **62% מקהל ה-ADHD אונליין הוא נשי** (YouGov) — late-diagnosed women הוא הסגמנט הדינמי ביותר.
- "ADHD-late-diagnosed-mom" identity מתפוצצת — NYT, The Atlantic, TikTok ADHD parent content.
- אבל: <50% מטענות בסרטוני TikTok תואמות לקריטריונים אבחנתיים → קהל עם demand גבוה ל-coping tools גם בלי אבחנה רשמית.
- Stage: peak culture moment 2024-2026.
- Impact: **tailwind לטווח קצר-בינוני**; headwind ארוך-טווח אפשרי (backlash על "ADHD as identity badge", רגולציה על misinformation).

## טכנולוגיה — מגמות מפתחות

### AI Personal Assistants — מעבר מ-Chatbot ל-Agent
- **Gartner Aug 2025:** AI agents יקפצו מ-<5% מ-enterprise apps (2025) ל-**40% (סוף 2026)**.
- Counter-signal: **>40% מ-agentic AI projects יבוטלו עד 2027** (Gartner Jun 2025) — אזהרת hype trough.
- Voice-first interactions גדלו ב-340% ב-2025; חיזוי >50% מ-consumer AI interactions voice-initiated עד 2027.
- Stage: Early-growing → Peak hype 2026.
- Impact ל-Planny: **opportunity** — משתמשי ADHD הם early adopters לטרנד (brain-dump באמצעות קול = ADHD-perfect modality); **threat** — bar של "AI-powered" עולה מהר, GPT-wrapper לא יבדל.

### Mobile-First, AI-Native, On-Device
- Apple Intelligence runs on-device לדגמי iPhone של 2024+ → >60% מ-iPhone install base בארה"ב באמצע 2026.
- Personal AI assistant market CAGR **41.9%** — privacy הוא הדרייבר הראשי.
- LLM costs ירדו דרסטית 2024-2026 (Hostinger / Goldman Sachs).
- iOS 27 (June 2026 expected): Extensions framework + Gemini/Claude/etc plug-ins.
- Stage: Growing fast → Mainstream on iOS 18+.
- Impact: **tailwind ל-solo founder** — בניית מוצר AI-native ב-$1,500 ריאלי; ADHD users רגישים ל-"איפה ה-mental-health data שלי" → on-device = trust signal חזק.

### Calendar APIs ו-MCP Standard
- **Google Calendar API:** יציב, רחב, OAuth — direct integration זמין ב-3-4 שבועות פיתוח.
- **Apple EventKit:** מוגבל ל-iCloud sync — **לא יכול לכתוב ל-Google/Outlook**. מי שמסתמך על EventKit נחתך מהחתיכה הגדולה של הקהל.
- **Microsoft Graph:** enterprise focus, פחות רלוונטי ל-B2C ADHD.
- **Model Context Protocol (MCP):** Google Gemini Spark שלח May 2026 עם MCP ל-Canva/OpenTable/Instacart/Adobe/Spotify/GitHub/Notion/Slack. Apple מחבר Gemini/Claude דרך iOS 27 Extensions.
- Stage: Mature אבל פרגמנטרי; protocol war underway.
- Impact: **moat טכני ל-Planny** — direct Google OAuth זה מה שמתחרים רבים נכשלים בו (Tiimo, Routinery נשארים EventKit-only). זה ההזדמנות הטכנית הכי גדולה בחבילה.

### Burnout-Aware / Context-Aware Scheduling
- Morgen, Sunsama, Motion, Skedpal מתחילים לשלב emotional well-being, work patterns, energy windows.
- Stage: Growing ב-"thoughtful productivity" niche; עדיין נדיר ב-mainstream.
- Impact: מתיישר ישירות עם צורך ADHD ל-energy-aware planning (low-dopamine days, hyperfocus windows). מעטים מבצעים את זה טוב ל-ADHD ספציפית.

## השקעות ו-M&A — איפה הכסף

### Categories Hot ב-2025-2026
- **Digital health funding 2025: $14.2B (+35% YoY מ-$10.5B)** — Rock Health Year-End 2025.
- AI-central startups: **$34.4M avg per round** מול $18.8M ל-non-AI = AI premium ברור.
- Mental health = אחת מ-2 קטגוריות "concentrated capital" של 2025.
- Trend direction: מאיץ ב-megadeal end; flat-to-modest ב-seed.

### Notable Deals (ADHD-adjacent + AI Scheduling)
| Company | Stage | Amount | Date | Significance |
|---|---|---|---|---|
| **Reclaim.ai → Dropbox** | Acquired | **$40.2M** | Jul 26, 2024 | ה-comp הכי קרוב ל-Planny. 320K משתמשים → $125/user EV. validates exit possible במספרי משתמשים צנועים. |
| **Apple → Mayday Labs** | Acquired (IP) | undisclosed | Apr 2024 | IP של AI scheduling. סימן מובהק לכיוון Apple Intelligence + Calendar. **Trigger ל-threat clock של WWDC**. |
| Motion | Series C | $60M ($550M val) | Sep 2025 | פיבוט ל-B2B agentic — **עזב את consumer ADHD lane** = opportunity ל-Planny. |
| Inflow | Series A | $11M | 2023 | ADHD CBT app. Octopus Ventures. ~$22.49/mo. War chest על paid social → CAC לא ריאלי לבוטסטרפ. |
| Tiimo | ADHD-native | $4.8M cumulative | 2020-2023 | iPhone App of the Year 2025. 500K users, 50k paying subs (~$3-6M ARR estimate). |
| Talkiatry | Series D | $210M | 2025 | Telepsychiatry megadeal — mental health concentrated capital validation. |
| Grow Therapy | Late | $150M | 2025 | Hybrid mental health. |
| Neurode | Pre-seed | $5.2M | 2024 | ADHD medtech headband. Khosla + PsyMed. |
| Rule | Pre-seed | £800k | 2025 | ADHD-tax fintech. |

### Implications
- VC הוכיחה ש-ADHD scheduling יכול לצאת ב-$40M acquisition.
- Acquirers exist בעלי $125/user EV → solo bootstrap עם 20K משתמשים = exit פוטנציאלי $2.5M+.
- אבל: השוק מתממן מהר → Planny לא יכול לחכות. כל רבעון שעובר מצמצם whitespace.

## Behavioral Shifts בקהל היעד

### Gen Z + Millennials עם ADHD
- **Millennials = 45% מכל in-app spending**.
- **42% מ-Gen Z כרגע בטיפול** (+22pp מ-2022) — משלמים בפועל על mental health.
- 73% productivity-tool usage בקוהורט ADHD בוגר.
- Health & wellness = **23% מ-subscription consumer spend** (RevenueCat 2025).
- Subscription app ARPU benchmark: **$8.41/mo** (טווח $3-9/mo).
- **Productivity LTV = $46.97 — הכי גבוה מבין כל ה-app categories** (RevenueCat 2026).
- US monthly productivity avg = **$15.20** (Adapty 2026), +12.5% YoY.
- **Weekly plans = 66% מהכנסות productivity** (RevenueCat 2026) — Planny's wedge הוא בדיוק שם.

### Subscription Fatigue + "ADHD Tax" Discourse
- שיח "ADHD tax" ב-Reddit/TikTok: ADHD users impulse-buy productivity tools ואז זונחים — guilt cycle.
- Subscription guilt = recurring r/ADHD theme; קישור recurring charge → "personal failure" כשלא בשימוש.
- Privacy-conscious post-Cambridge Analytica + BetterHelp/Cerebral scandals → חוסר אמון ב-corporates גדולים, רצון לאינדי.
- **Implication ל-Planny:** pricing power קיים ($8-15/mo); הגרסה האנטי-guilt (annual upfront, no surprise charges) היא יתרון תחרותי.

### Late Diagnosis Wave
- **61% מהנשים עם ADHD מאובחנות בבגרות** (מול 40% מהגברים).
- Postpartum diagnoses → triggered בגיל 28-35.
- "ADHD-late-diagnosed-mom" identity מתבססת כקטגוריה ברורה.
- TikTok #ADHDinWomen מתפוצץ — אחת מקטגוריות ה-content הצומחות ביותר ב-2024-2026.

## Expert Predictions

| Prediction | Source | Confidence |
|---|---|---|
| 40% מ-enterprise apps עם task-specific AI agents עד סוף 2026 | Gartner | High |
| >40% מ-agentic AI projects יבוטלו עד 2027 (cost, unclear value) | Gartner | High — counter-signal חשוב |
| Personal AI agents = "default interface" עד 2026 | Goldman Sachs / Salesforce | Medium-High |
| >50% מ-consumer AI interactions voice-initiated עד 2027 | Salesforce / aggregations | Medium |
| Mental wellness apps יגיעו ל-~$13B globally עד 2027 (Mental Health Apps Market: $8.4B 2025 → $18.81B 2031) | MarketsandMarkets / SNS | Medium |
| ADHD apps market: $2.78B (2026) → $3.22B (2027) → $4.3B (2030); CAGR 12-15% | Multiple analysts (variance רחבה) | Low-Medium |
| AI agents handle 30-40% מ-knowledge work עד 2027-2028 | McKinsey / Gartner | Medium |
| ADHD vertical יישאר fastest-growing mobile niche עד 2028 | Sensor Tower-style aggregations | Medium |

## Regulatory Trajectory

### Direction of Travel
- **Apple App Store (March 26, 2026):** סגירה חזקה יותר — health/medical category triggers regulated medical device declaration. **Productivity remains safe harbor** ל-Planny.
- **Google Play (Jan 2026 + Apr 2026):** mandatory disclaimer "not a medical device" בפסקה הראשונה של description; Organization Account verification; ban על שימוש ב-health data ל-employment/insurance.
- **FDA General Wellness (Jan 6, 2026 update):** deregulatory shift — favorable ל-Planny אם copy נשמר ב-"wellness/organization/executive-function support" ולא "treats ADHD."
- **FTC:** אכיפה אגרסיבית של ad pixel violations — BetterHelp $7.8M (2023), Cerebral $7M (2024), GoodRx $1.5M (2023). **Common pattern:** כל אכיפה הייתה על data sharing עם ad networks, לא טענות טיפוליות.
- **WA MHMDA:** $7,500/violation + **private right of action** = plaintiffs' firms trolling אקטיבית. Treble damages עד $25K.
- **CA CPRA SPI:** mental health = sensitive personal information; rights to limit + cybersecurity audits פאזה 2027-2028.
- **Israel Amendment 13 (אוג 2025):** mandatory DPO, ISS handling, fines עד NIS 100K לאדם בלי הוכחת נזק.
- **EU AI Act:** transparency obligations יחולו על AI scheduling אם משיק ב-EU.

### Implications ל-Planny
- מותר לפעול ב-General Wellness Category 1 — "stress management, mental acuity, self-esteem, sleep management" כלולים ב-safe harbor.
- אסור: "מטפל ב-ADHD", "משפר ריכוז", "מפחית תסמינים", "alternative to Adderall", "clinically proven", "doctor-recommended".
- מותר: "Designed for adults with ADHD", "ADHD-friendly planning", "helps organize your week".
- חובה: Privacy Policy נפרדת ל-health data + separate consent ל-collection וsharing (MHMDA).
- **אסור Meta/TikTok pixels בכל דף שמזכיר ADHD** — זה ה-tripwire של BetterHelp/Cerebral/GoodRx.
- Apple App Store categorization: **Productivity primary**, לא Health & Fitness.
- Compliance budget: **$8-19K launch (US-only)**; $15-35K (+ Israel + EU).

## איום קומודיטיזציה

### Timing Clock — האירועים הקרובים
- **WWDC 2026 — June 8 (~10 ימים):** סבירות גבוהה ל-Apple Intelligence + scheduling features מבוסס רכישת Mayday Labs (Apr 2024). על ה-IP של Mayday — AI scheduling — Apple לא הוציאה דבר עדיין; WWDC הוא ה-natural reveal point. **High-impact event לכל ה-AI scheduling lane.**
- **Google Gemini Spark (May 2026, כבר חי):** calendar reschedule + Daily Brief + MCP integrations. Gated $100/mo enterprise — לא ישיר ל-consumer ADHD עדיין.
- **iOS 27 (יוני 2026 expected):** Siri-Gemini hybrid; Extensions framework לחיבור third-party AI models. **Calendar layer יכול להפוך לcommodity.**
- **Microsoft Copilot agentic (April 27, 2026, כבר חי):** enterprise focus, פחות רלוונטי.
- **ChatGPT Scheduled Tasks + Gemini Scheduled Actions (Nov 2025):** כבר רצים. Tom's Guide/TechRadar מאשרים — gen AI עושה recurring reminders + summaries מעל Gmail/Calendar.

### חלון הזדמנות לקטגוריה ADHD
- **9-12 חודש** עד שהשכבה הבסיסית של AI scheduling מקומודיטיזציה (basic task triage, recurring reminders).
- **24-48 חודש** עד שתחווית ADHD-specific (transitions, buffers, gentle re-planning, non-judgmental tone, body-doubling) מקומודיטיזציה — Apple/Google לא יבנו את זה מעצמם.
- **Defensible long-term moats ל-Planny:** (a) ADHD-specific data + RLHF preference data על re-planning שמרגיש טוב מול shaming, (b) brand trust בקטגוריה רגישה, (c) integrations עם ADHD coaching content / therapy, (d) couples/partner features, (e) optional clinical reimbursement path.

## Timing Scorecard

### Tailwinds (אפשרויות)
1. **+270% חיפושי ADHD גלובלית** (2019-2023, 20 מדינות)
2. **+123% עליה באבחנות מבוגרים** (CDC Dec 2025)
3. **62% נשי = beachhead מאומת** — late-diagnosed women 25-40
4. **TikTok #ADHD: 500M+ צפיות**, 7th בריאותי
5. **Productivity LTV $46.97 — הכי גבוה מכל ה-app categories** (RevenueCat 2026)
6. **Weekly plans = 66% מהכנסות productivity** — exactly Planny's wedge
7. **Motion עזב את consumer ADHD lane** (Series C, $550M val, B2B pivot)
8. **AI costs ירדו → solo founder יכול לבנות ב-$1,500**
9. **Reclaim → Dropbox $40.2M** — exit comp ברור
10. **CDC + Apple endorsement (Tiimo App of the Year)** = peak cultural moment

### Headwinds (סיכונים)
1. **WWDC June 8 — Apple Intelligence + Mayday Labs IP** → רעידת אדמה צפויה
2. **Tiimo iPhone App of Year 2025** → editorial moat + 500K users
3. **Saner.AI** Product Hunt #1 ADHD app — 389 upvotes, ADHD-AI positioning
4. **Indy by Shimmer (Jan 2026, 205 upvotes #6 daily)** — direct competitor, seed-funded
5. **Inflow $11M paid social war chest** → CAC לא ריאלי לבוטסטרפ
6. **Mental health retention 3.3% day-30** (4.1% productivity)
7. **Subscription guilt + "ADHD tax" reputation** בקטגוריה
8. **40% מ-agentic AI projects יבוטלו (Gartner 2027)** — hype trough warning
9. **Gemini Spark + ChatGPT Scheduled Tasks כבר חיים** — commodity layer מתחיל
10. **MHMDA private right of action** — plaintiffs' firms trolling

### ציון עיתוי כולל
**Tailwinds 7/10, Headwinds 4/10. נטו: עיתוי טוב, אבל לחוץ.**

חלון פעולה אופטימלי: **השקה soft בתוך 60-90 ימים, סגירת moat טכני (direct Google Calendar OAuth) ב-30 ימים, סגירת partnership ראשון עם ADHD creator (Tracy Otsuka / Jessica McCabe alt) ב-45 ימים, MHMDA-compliant privacy stack מ-day 1, ולא להשיק את אותו השבוע של WWDC (Jun 8)**.

## מה זה אומר ל-Planny

1. **WWDC June 8 הוא נקודת רעידת אדמה — תכנן סביבה, לא נגדה.**
   - אל תשיק רשמית באותו שבוע. הכן war-room עם תוכן תגובתי תוך 24 שעות מההכרזה.
   - אם Apple מציגה Intelligence scheduling: ה-positioning של Planny הופך ל-"ADHD-native, weekly cadence, gentle re-planning" — לא "AI calendar" (שיהפוך לcommodity).
   - אם Apple לא מציגה: window הופך רחב יותר ב-3-6 חודש.

2. **Direct Google Calendar OAuth = ה-moat הטכני, לא Apple EventKit.**
   - 3-4 שבועות פיתוח, חובה לסגור ב-30 ימים.
   - זה מה ש-Tiimo ו-Routinery לא עושות → מאפשר ל-Planny להיכנס לסטאק של משתמשי Google מבלי לאלץ אותם להעביר נתונים ל-iCloud.
   - גם moat נגד גרסת iOS Calendar רק של Apple Intelligence — Planny עובד cross-platform.

3. **Productivity LTV $46.97 + weekly plans 66% מהכנסות = ה-zone של Planny.**
   - תמחור $8.99/mo monthly, $69-79/yr annual ($5.83-$6.67/mo effective) מתיישר מדויק.
   - שקול גם weekly plan ($3.99-$4.99/wk) — 66% מהכנסות productivity מגיעות משם, ו-ADHD impulse-conversion גבוה.
   - Trial רק על annual/6mo — מקטין subscription guilt, גם valid אסטרטגית.

4. **Partnership עם late-diagnosed-women creator תוך 45 ימים.**
   - Sunsama כבר נעלה את Jessica McCabe (How to ADHD). Tracy Otsuka (ADHD for Smart Ass Women podcast) הוא target טבעי.
   - 62% נשי בקהל ADHD → creator-led GTM זול וממוקד מול $11M paid social של Inflow.

5. **ה-headwind הכי גדול הוא retention, לא acquisition.**
   - Day-30: 4.1% productivity, 3.3% mental health (RevenueCat benchmarks).
   - תכנון retention מ-day 1, לא retrofit: weekly review ritual, compassionate re-engagement (לא shaming), structured day-30/day-90/day-180 cliffs.
   - "ADHD-cohort churn" מובנה (8-12% monthly) → annual/6mo מ-day 1, לא afterthought.

6. **Marketing language policy לפני הדולר הראשון של growth.**
   - "Designed for adults with ADHD" כן; "treats ADHD" / "improves focus" לא.
   - Zero pixels בכל דף שמזכיר ADHD — server-side conversion only.
   - $0 שליטה שמונעת חשיפת $7.8M כמו BetterHelp.

## פערי נתונים אגרגטיביים על מגמות

1. **WWDC 2026 (Jun 8) eedge יכול לשנות הכל** — 10 ימים מהמסמך. נדרש re-evaluation מיידי אחרי ההכרזה.
2. **Tiimo/Numo/Inflow ARR מדויק** — Tiimo "50K paying subs" הוא ה-figure הקונקרטי היחיד. ARR estimates ($3-6M ל-Tiimo) לא מאומתים.
3. **Direct Google Trends RSV numbers** — לא נשלפו ערכים מדויקים 0-100; כל המגמות directional ולא absolute.
4. **Direct Reddit thread data** — WTP sentiment סינתזה מ-secondary, לא ציטוטים ישירים.
5. **Indy by Shimmer pricing** (launched Jan 2026) — לא פומבי. אם מתחת ל-$8/mo, whitespace מצטמצם.
6. **CAC benchmarks ל-ADHD-specific apps** — לא קיימים פומבית. Mental health כללי $30-80, ADHD ככל הנראה זול יותר דרך TikTok organic.
7. **Apple iOS 27 + Gemini-Siri scope** — rumor-stage עד WWDC. Critical re-check ב-30 ימים.
8. **2025-2026 funding rounds ל-ADHD-labeled apps** מעבר ל-Rule/Neurode — לא נמצאו. או deals quiet או VC moment עוד לא בשיא.

---

## Sources

- [CDC Data Brief #543 (Dec 2025) — Adult ADHD prevalence](https://www.cdc.gov/nchs/products/databriefs/db543.htm)
- [ADDitude — Adult ADHD Diagnosis Growing More Common (CDC)](https://www.additudemag.com/adult-adhd-diagnosis-cdc-report/)
- [PLOS One — A double-edged hashtag: #ADHD on TikTok (2025)](https://journals.plos.org/plosone/article?id=10.1371%2Fjournal.pone.0319335)
- [UBC News — ADHD misinformation on TikTok](https://news.ubc.ca/2025/03/adhd-misinformation-on-tiktok/)
- [Gartner — 40% of enterprise apps will feature task-specific AI agents by 2026](https://www.gartner.com/en/newsroom/press-releases/2025-08-26-gartner-predicts-40-percent-of-enterprise-apps-will-feature-task-specific-ai-agents-by-2026-up-from-less-than-5-percent-in-2025)
- [Gartner — Over 40% of agentic AI projects will be cancelled by 2027](https://www.gartner.com/en/newsroom/press-releases/2025-06-25-gartner-predicts-over-40-percent-of-agentic-ai-projects-will-be-canceled-by-end-of-2027)
- [Goldman Sachs — What to expect from AI in 2026](https://www.goldmansachs.com/insights/articles/what-to-expect-from-ai-in-2026-personal-agents-mega-alliances)
- [Rock Health — 2025 year-end digital health funding](https://rockhealth.com/insights/2025-year-end-digital-health-funding-overview-a-tale-of-two-markets/)
- [TechCrunch — Dropbox acquires Reclaim.ai (Aug 2024)](https://techcrunch.com/2024/08/22/dropbox-acquires-index-ventures-backed-ai-scheduling-tool-reclaim-ai/)
- [MarketScreener — Dropbox acquired Reclaim.ai for $40.2M](https://www.marketscreener.com/quote/stock/DROPBOX-INC-45013534/news/Dropbox-Inc-acquired-Reclaim-ai-Inc-for-40-2-million-47716890/)
- [Built In SF — Motion secures $60M Series C](https://www.builtinsf.com/articles/motion-raises-60m-funding-20250909)
- [TechCrunch — Inflow raises $11M Series A (Jan 2023)](https://techcrunch.com/2023/01/11/inflow-a-platform-for-managing-adhd-through-cbt-raises-11m/)
- [Daring Fireball — 2025 App Store Award Winners (Tiimo)](https://daringfireball.net/2025/12/2025_app_store_award_winners)
- [Tiimo — Winner of iPhone App of the Year 2025](https://www.tiimoapp.com/resource-hub/tiimo-winner-2025-app-store-awards)
- [TechTimes — Gemini Spark launch (May 2026)](https://www.techtimes.com/articles/317144/20260525/gemini-spark-googles-24-7-cloud-ai-agent-now-executes-tasks-third-party-apps.htm)
- [RevenueCat — State of Subscription Apps 2025](https://www.revenuecat.com/state-of-subscription-apps-2025/)
- [FDA — General Wellness: Policy for Low Risk Devices (2026)](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/general-wellness-policy-low-risk-devices)
- [FTC — Updated Health Breach Notification Rule (Apr 2024)](https://www.ftc.gov/business-guidance/blog/2024/04/updated-ftc-health-breach-notification-rule-puts-new-provisions-place-protect-users-health-apps)
- [Apple Developer — App Review Guidelines](https://developer.apple.com/app-store/review/guidelines/)
- [WA RCW 19.373 — My Health My Data Act](https://app.leg.wa.gov/RCW/default.aspx?cite=19.373&full=true)
- [IAPP — Israel Amendment 13 Reform](https://iapp.org/news/a/israel-marks-a-new-era-in-privacy-law-amendment-13-ushers-in-sweeping-reform)
- [McKinsey — Future of wellness trends](https://www.mckinsey.com/industries/consumer-packaged-goods/our-insights/future-of-wellness-trends)
- [Harmony HIT — State of Gen Z Mental Health 2025](https://www.harmonyhit.com/state-of-gen-z-mental-health/)

## Flags

**Red Flags:**
- **WWDC June 8 — Apple Intelligence + Mayday Labs IP reveal** הוא ה-binary event הגדול ביותר. Apple רכשה IP של AI scheduling לפני שנתיים בדיוק מתאים ל-iOS 27 timeline. אסור להשיק את אותו השבוע. נדרש war-room + תוכן תגובתי.
- **Tiimo iPhone App of the Year 2025 (Dec 2025)** = halo + 500K users + Apple editorial moat. כל positioning שלא בורח חד מ-Tiimo הוא dead on arrival. Planny חייב "weekly OS, not daily visual" framing.
- **MHMDA private right of action** — plaintiffs' firms trolling. חובה separate health-data consent + Health Data Privacy Policy ב-day 1, לא אחרי. אם פולין רגולטורי, $7,500-25,000 per user מצטבר.
- **Mental-health app retention crisis** — 30% נטישה ב-90 ימים, day-30 3.3%. זה ה-#1 failure mode בקטגוריה. אם Planny לא out-designs retention, כל ה-tailwinds לא יצילו unit economics.
- **Marketing copy drift = automatic FDA/FTC risk.** מספיק שמפרסם / מקדם / influencer יגיד "treats ADHD" כדי לפתוח חזית. חובה Marketing Language Policy לפני הדולר הראשון של growth.
- **Ad pixels (Meta/TikTok/Google) על דפי ADHD = BetterHelp/Cerebral/GoodRx fact pattern.** Default position: zero pixels, server-side conversion עם hashed IDs + explicit consent.

**Yellow Flags:**
- **ADHD app market size variance** ($0.5B – $7.7B by various Tier-3 sources) — directional (12-15% CAGR) אמין, absolute numbers לא. אסור להשתמש במספרים specific בdeck של משקיעים.
- **Indy by Shimmer (launched Jan 2026, $11M seed funding precedent)** — pricing לא פומבי. אם מתחת ל-$8/mo, whitespace של Planny מצטמצם. Monitor monthly.
- **Saner.AI launch decay (389→60→6 upvotes על 3 launches)** — Product Hunt ADHD audience saturated. Planny לא צריך PH-led GTM; TikTok / influencer / podcast sponsorship.
- **40% מ-agentic AI projects יבוטלו עד 2027 (Gartner)** — hype trough מתקרב. Planny לא צריך להיתלות ב"AI scheduling" framing; חייב ADHD-native framing שמחזיק גם אם ה-AI hype נשבר.
- **TikTok ADHD content מכיל <50% תוכן מדויק** — risk שpremium platforms (TikTok, Meta) ירסנו או יאסרו את ה-tag ב-2-3 שנים. Diversify channels.
- **Tiimo + Numo + Inflow + Saner + Indy + Routinery + Habi = 7+ competitors בקטגוריה** — Planny חייב wedge חד (weekly cadence + late-diagnosed-women + gentle re-planning + Google OAuth) ולא לחזור על "AI scheduler for ADHD".
- **Israel Amendment 13 + DPO threshold creep** — ברגע ש-Planny עובר ~10K Israeli users, חובה fractional DPO + PPA registration. Trigger אוטומטי בדשבורד.
