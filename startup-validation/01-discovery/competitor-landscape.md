# Competitor Landscape — Planny

**Phase:** Phase 3 Synthesis
**Project:** startup-validation (Planny)
**Date:** 2026-05-28
**Confidence:** Medium-High (תמחור, מימון ופיצ'רים מאומתים היטב; נתחי שוק, CAC ו-retention משוערים מבנצ'מרקים קטגוריאליים; פלטפורמות פוסט-WWDC = High-uncertainty)

---

## תקציר תחרותי

קטגוריית ה-AI scheduling ל-ADHD נמצאת ברגע של **bifurcation**. בתחתית מתרחבת שכבת אינדי + סולו-פאונדרים (Flint, Lately, NoPlex, neurolist, MyADHD) שמייצרת fragmentation ב-App Store search results אבל ללא איום נקודתי. באמצע יושבים ה-incumbents המאומנים: Tiimo (האייקון של ADHD-native, Apple iPhone App of Year 2025), Inflow (14% נתח שוק על גב $11M Series A ב-paid social), Sunsama (bootstrapped $1.5M ARR עם הצבא הכי טוב של creators), ו-Motion (שמתפנה מהזירה הצרכנית ל-B2B agentic ב-$50M ARR / $550M val). בראש העץ — **Saner.AI**, המתחרה החדש והמסוכן ביותר: Techstars + Google Accelerator, מדורגת #1 ברוב רשימות 2026, Product Hunt launch הכי חזק שהיה לקטגוריה (389 upvotes / 682 comments), broader scope של "Jarvis ל-ADHD" שיכול לבלוע את ה-wedge של Planny אם לא ננוע מהר. במקביל, **Indy by Shimmer** (שוגרה 15 ינואר 2026) מציגה את האיום האסטרטגי הכבד ביותר — חינמית כ-top-of-funnel ל-coaching של $200+/mo, עם $3.5M raise מאחורי הכיסוי.

המתחרה האמיתי הגדול ביותר הוא לא Tiimo או Saner — אלא **inertia + Apple Reminders + Google Calendar**. ADHD adults לא מחפשים אפליקציה — הם נכנעים לסטטוס קוו של נייר + sticky notes + ChatGPT + תזכורת אפל בודדת. ומעל הכל מרחפים שלושה גורמי פלטפורמה: **Apple Intelligence iOS 27** (WWDC ב-10 ימים, post-Mayday Labs acquisition = מנוע scheduling AI שכבר 2+ שנים בפיתוח), **Google Gemini Spark** (השיק במאי 2026, עם reschedule + Daily Brief), ו-**Microsoft Copilot Outlook agentic** (אפריל 2026, אבל אנטרפרייז-skewed). אלו לא מתחרים — הם **commoditization risk**.

ה-positioning ש-Planny צריך לנקוט הוא ברור: **לא להתחרות באקדמיות פיצ'ר נגד ענקים**, אלא לנעול את **late-diagnosed US women 25-40 כ-persona ייעודית** שאף אחד לא תובע בשמה — שילוב של הקול של Numo ("cringe-free"), אמינות קלינית של Inflow (מינוס בעיית ה-billing שלו), קצב ה-capacity-aware ritual של Sunsama (מינוס mobile read-only), וכל זה ב-$9.99/mo שמתחת ל-Tiimo iOS ($12), Motion ($19), Sunsama ($25), Inflow ($22+). ה-wedge הטכני הוא **two-way Apple + Google Calendar sync** (Tiimo's #1 פגיעות), ה-wedge החוויתי הוא **voice brain-dump → AI weekly plan ב-30 שניות** (אף מתחרה לא מאחד את שלושת השכבות), וה-wedge האתי הוא **billing transparency + no-shame UX** במונחים שבהם Inflow ו-Numo נכשלים פומבית ב-Trustpilot ו-Reddit.

---

## מפת ריכוז שוק

- **Tier 1 (Threat HIGH):** Tiimo, Saner.AI, Indy by Shimmer
- **Tier 2 (Threat MED-HIGH):** Inflow, Motion (פיבוט B2B), Sunsama, Flint (חדש, אותו wedge)
- **Tier 3 (Threat MED):** Routinery, Numo, Akiflow, neurolist, MyADHD (TestFlight)
- **Tier 4 (Threat LOW):** Lately, NoPlex, Unloop, Ramble, Amie, Trevor AI, MyADHD assessment, neurolist UK, ChatGPT custom GPTs
- **Substitutes (Status Quo):** Apple Reminders + Calendar, Google Calendar manual, Notion + templates, Todoist, Things 3, paper Hobonichi / bullet journals, whiteboards, ADHD coaching ($170-225/session, Shimmer $140-345/mo), virtual assistants ($549-5,190/mo), "nothing — I just survive"
- **Platform absorption risk:** Apple Intelligence iOS 27 (post-Mayday Labs acquisition, WWDC June 8 2026), Google Gemini Spark ($100/mo Ultra) + Daily Brief, Microsoft Copilot Outlook agentic, OpenAI ChatGPT (Scheduled Actions + Memory + future calendar connectors)

**ריכוז:** Fragmented but bifurcating. אף שחקן בודד לא מחזיק >15% משוק ADHD apps; Inflow מוביל ב-14% (T3), Tiimo מוביל במותג עם 500K active / 50K paying. אין דומיננטיות אמיתית — מה שמשאיר window אבל גם אומר שהקטגוריה עוד לא הוכיחה ש-winner-takes-most אפשרי.

---

## טבלת השוואת פיצ'רים (synthesized final)

| Feature | Planny (planned) | Tiimo | Motion | Reclaim | Sunsama | Inflow | Routinery | Numo | Saner.AI | Indy |
|---------|------------------|-------|--------|---------|---------|--------|-----------|------|----------|------|
| Weekly plan generation | ✅ | ✅ partial (Co-planner) | ✅ auto | partial (habits) | ✅ ritual | ❌ | ❌ | ❌ | ✅ | ✅ |
| Constraint-based reschedule | ✅ | ❌ | ✅ | ✅ | partial (H2'25) | ❌ | ❌ | ❌ | ✅ | ? |
| Two-way Google Calendar sync | ✅ wedge | ❌ one-way | ✅ | ✅ | ✅ | ❌ | ❌ | ❌ | ? | ? |
| Two-way Apple Calendar sync | ✅ wedge | ❌ one-way | partial | limited | partial | ❌ | ❌ | ❌ | ? | ? |
| ADHD-native UX | ✅ | ✅ core | ❌ | ❌ | partial (capacity) | ✅ core | ADHD-friendly | ✅ core | ✅ | ✅ |
| Partner / shared mode | ✅ planned | ❌ profile-sharing only | team only | team only | team only | community only | ❌ | squad social | ❌ | ? |
| Voice brain-dump → plan | ✅ planned | partial (Co-planner) | limited | ❌ | ❌ | Quinn chat | voice guidance (out) | ❌ | partial | ? |
| Free tier | ❌ (14-day trial) | trial only | trial only | ✅ Lite forever | trial only | trial only | ✅ limited | trial only | ? | ✅ |
| Mobile native iOS+Android | ✅ | iOS-strong, Android beta | web-first, mobile companion | web-only | mobile read-only | ✅ | ✅ | ✅ | partial | ✅ |
| Monthly $ | $9.99 | $12 iOS / $10 web | $19+ | $0 / $8-18 | $20-25 | $22.49 / $47.99 w/coach | $3.99 | $7.99-15.99 | TBD ($8-12 est) | Free |
| Annual $ | $59.99 | $54-79.99 / $42 web | $228+ | $0-216 | $240 | $95.99-199.99 | $27.49 | $59.99 | TBD | Free |
| ADHD founding team | ✅ | partial (Azari ND) | ❌ | ❌ | ❌ | partial (clinician) | ❌ | ✅ | ? | ✅ (coaching DNA) |

---

## ניתוח מתחרים מובילים — Deep Dive

### Tiimo — האיום הקיומי

- 500K active users / 50K משלמים, 3M+ downloads, 1M+ claimed users
- **Apple iPhone App of the Year 2025** (6,600+ testimonials, Daring Fireball)
- $4.8M גוייסו (pre-Series A; Crowberry, People Ventures, Divergent Investments)
- Copenhagen-based, 25-30 בצוות, Azari היא ND בעצמה
- Pricing iOS $12/mo / $54-79.99/yr; web $10/mo / $42/yr; family $119.99/yr
- **חוזקות:** מותג חזק ביותר ב-ADHD-native, Apple endorsement (moat ל-12-24 חודשים), עיצוב ויזואלי משלהם, AI Co-planner שוגר
- **חולשות (פגיעויות):**
  - **One-way calendar sync** ל-Apple/Google/Outlook — לא כותב חזרה. **זה ה-#1 wedge ל-Planny.**
  - אין partner mode אמיתי (family = profile sharing, לא קואורדינציה)
  - Setup overwhelm — תלונה חוזרת (Reddit + reviews)
  - Buggy timer, slow support, cancellation friction
  - Android חלש/late
  - בקשת פיצ'ר פומבית ל-two-way sync ב-**tiimo.nolt.io** — אם Tiimo משחרר ראשון, ה-wedge נסגר
- **משמעות:** Tiimo הוא ה-#1 incumbent ב-positioning של Planny. אבל ניתן לתקוף אותו על שני צירים נקודתיים (two-way sync + partner mode) ש-Planny יכולה לסגור ב-9-12 חודשים. **דרישה: לא לנסות לנצח אותו על visual design — לנצח על calendar trust ו-mobile UX.**

### Saner.AI — האיום החדש שלא היה ב-Wave 1

- Techstars + Google Accelerator + Value Create Ventures
- מדורגת **#1 ברוב רשימות "best ADHD app 2026"** (Morgen, Rivva, OnePageCRM)
- Product Hunt launch: 389 upvotes / 682 comments — ההשקה הכי חזקה אי-פעם של אפליקציית ADHD
- ~$120K disclosed ב-Crunchbase (כנראה undercount), מקושרת ל-Asian/SEA fund
- AI-native assistant ל-notes + email + calendar + chat — **broader scope מ-Planny**
- **חוזקה:** content marketing הכי רעשני בקטגוריה, brand momentum מהיר, Google credits + accelerator distribution
- **חולשה אפשרית:**
  - **Scope creep** — "Jarvis ל-ADHD" יכול להיות חולשת focus
  - אין mobile-first ברור, נראה כ-knowledge-worker-leaning
  - אין positioning של "women 25-40 / late-diagnosed" — הם רחבים
  - Pricing לא פומבי = signal של חוסר ביטחון
- **משמעות:** **זה האיום החדש מספר 1.** Saner.AI היה צריך להיות ב-Wave 1 — זה process flag. נדרש Planny להגיב מהר עם persona-narrow positioning ש-Saner לא יכול לתבוע.

### Motion — פינוי הזירה הקונסיומרית

- $50M ARR (Aug 2025), $550M val, $102M raised, Series C ספטמבר 2025 ($38M)
- **פיבוט ל-B2B agentic** — Motion AI Employees (מאי 2025), Team Pro/Business AI tiers, $19-69/seat
- Harry Qi (CEO) הוא founder-led PLG ב-LinkedIn/Twitter — אבל הפוקוס הוא SMB
- **חוזקה:** המנוע הכי בוגר ל-auto-scheduling, war chest, brand
- **חולשה ל-Planny:**
  - **ADHD-hostile by design** — "constant re-prioritization" = חרדה ל-ADHD brain (Reddit)
  - Steep learning curve, Mobile companion only, $228+/yr יקר מדי
  - "Got auto-charged" complaints על trial flow (dark pattern)
- **משמעות ל-Planny:** **Motion עוזב את הקונסיומר ADHD.** מתחרה אחד פחות בנישה הצרכנית. הסיכון היחיד: רכישה של ADHD brand (Tiimo? Numo?) לצורך consumer entry.

### Reclaim.ai — סטטוס Dropbox

- נרכשה אוגוסט 2024 ב-**$40.2M** ע"י Dropbox (SEC 8-K)
- 22 איש הצטרפו ל-Dropbox; 43K companies / 320K users pre-acquisition
- **Lite חינמי-תמיד tier** — היחיד מתוך ה-incumbents שיש לו free forever
- **אין mobile native** — web/desktop only
- post-acquisition: cross-sell בלבד, marketing visibility ירד
- **משמעות ל-Planny:**
  - הסיכון העיקרי = אם Dropbox משחרר Reclaim Mobile + מוסיף ADHD framing, Planny מולה competitor חינמי + Dropbox distribution
  - אבל ההסתברות לזה ב-12 חודשים נמוכה — Reclaim מוטמעת כ-team productivity tool ב-Dropbox, לא ADHD play
  - **Watch closely:** mobile launch + ADHD pivot signals

### Inflow — האיום + ההזדמנות (Trust Wedge)

- **14% נתח שוק ADHD apps** (T3 marketgrowthreports)
- $16.7M גוייסו, Series A $11M ינואר 2023 (Octopus Ventures led)
- **TikTok @inflow: 296.6K followers, 16.2M likes** — הדומיננטית בקטגוריה
- Quiz funnel (Noom-style) = primary CTA
- Co-founders: Levi Epstein, Seb Isaacs, Dr. George Sachs (clinician credibility)
- Pricing: $22.49/mo / $95.99/yr (no coach); $47.99/mo / $199.99/yr (with coach)
- **חוזקות:** CBT-grounded, best-funded ADHD-native, community + coaching layer
- **חולשות (פגיעויות):**
  - **בעיית מוניטין billing/cancellation ב-Trustpilot ו-Reddit** — multiple users דיווחו על charges אחרי cancel, slow refund response. **זה moat אתי ל-Planny.**
  - לא planner — task management secondary
  - Engagement drops sharply אחרי onboarding (mental-health app pattern)
- **משמעות ל-Planny:**
  - **אסור להתחרות בערוצי paid social** עם הקהל ADHD שלהם — ה-$11M שלהם יבד את ה-CAC
  - **חייבים לעבור על billing transparency** כ-brand promise פומבית
  - Possible partnership opportunity — Inflow = education, Planny = planning (use cases לא חופפים מלא)

### Sunsama — ה-Template ל-GTM של Planny

- bootstrapped $1.5M ARR, profitable מ-2022
- mobile **read-only** (תסכול ידוע ב-Reddit + comparison blogs)
- **600+ creator ambassador program** (SARAL-managed) — out-competed VC rivals
- שותפות עם **Jessica McCabe / How to ADHD** (1.7M+ subs) — דפי dedicated `/for-adhd`, `/a/howtoadhd`, `/a/adhd-doers`
- $20-25/mo, 14-day trial **no CC required**
- **חוזקה:** capacity-aware planning (anti-overload) = ADHD-helpful, brand voice ערכי
- **חולשה ל-Planny:**
  - Mobile read-only = פתח ענק ל-ADHD users שמתכננים on-the-go
  - $240/yr יקר ל-consumer
  - לא ADHD-explicit — user חייב לזהות עצמית
  - Jessica McCabe **נעולה** — אסור לכוון לשם
- **משמעות:** **ה-GTM template ל-Planny.** ה-600+ creator model הוא בדיוק מה ש-$1,500 budget יכול להעתיק בקנה מידה קטן ב-12-18 חודשים.

### Indy by Shimmer — האיום האסטרטגי הכבד

- שוגרה **15 ינואר 2026** (The Vibe With Ky)
- founder: Christal Wang (Shimmer, YC-backed)
- **חינמית, no paywall** — top-of-funnel ל-Shimmer coaching ($140-345/mo)
- Shimmer total raised: **$3.5M** (YC, Worklife, Seed to B, Aglaé, Koa Labs, Gaingels)
- **חוזקה:** free distribution + well-funded parent + defensible cross-sell economics
- **חולשה:** product עוד צעיר, pricing/feature breadth לא ברור, scope מוגבל אם זה רק funnel
- **משמעות ל-Planny:** **התשובה ל-"why pay when Indy is free" חייבת להיות מוכנה לפני launch.** ההתשובה: (1) Planny לא מנסה למכור coaching, אז אין conflict-of-interest motivation; (2) feature depth (two-way sync, partner mode, voice brain-dump) ש-funnel-app לא תבנה; (3) brand voice של late-diagnosed women.

### Saner.AI vs Indy vs Tiimo — מי האיום הראשי לקטגוריה של Planny?

**תשובה: Saner.AI > Tiimo > Indy.**

- **Saner.AI** הוא הסיכון הקרוב ביותר ל-positioning של Planny — same AI-native + ADHD-native pitch, momentum טרי, Techstars + Google credits, ועדיין לא נעל persona. אם הוא יסגור Series Seed ($5-15M) ב-6-12 חודשים הקרובים, marketing surge יקבע את הקטגוריה.
- **Tiimo** הוא הסיכון הגדול ביותר ב-incumbent terms (brand, Apple, install base) — אבל פגיעויותיו (sync, partner mode) נקודתיות וניתנות לתקיפה.
- **Indy** הוא הסיכון האסטרטגי לטווח ארוך (free + funded parent) — אבל היא funnel app שתחנוק קודם כל את Inflow ו-Numo, לא בהכרח את Planny אם Planny מוכיח value-for-pay.

---

## מפת פוזישנינג

Planny ממקם את עצמו ב-3 צירים:

**ציר X (Generic → ADHD-native):** Planny מימין הקיצוני. מצד שמאל יושבים Motion, Reclaim, Akiflow, Sunsama, Notion — אף אחד מהם לא מדבר ADHD פומבית. מצד ימין מצטופפים Tiimo, Inflow, Numo, Routinery, Indy, Saner.AI. **Planny מציב את עצמו לא רק "ADHD-native" אלא "late-diagnosed-women-25-40-native"** — sub-segment ש-Tiimo (neurodivergent רחב), Saner (knowledge workers) ו-Numo (younger cringe-free) לא תובעים.

**ציר Y (כלי בודד → פלטפורמת תפעול שבועית):** Planny ב-top. מתחת יושבים Routinery (routine execution), Lately (be-on-time), Goblin Tools (task decomp), Things 3 (task list), Apple Reminders (single-fire). באמצע יושבים Numo (gamified social), Inflow (coaching), Flint (daily). בראש העץ מצטופפים Sunsama (daily ritual), Motion (auto-schedule), Tiimo (visual planner), Saner.AI (broad assistant). **ה-positioning של Planny: weekly cadence — לא daily, לא single-task — שזה ה-jobs-to-be-done הנכון ל-ADHD planning** (capacity-aware over a week beats daily ritual which ADHD adults abandon).

**ציר Z (סמוי — Pricing fairness + shame-free design):** Planny ב-quadrant של "fair pricing + warm UX". Motion, Akiflow, Sunsama יושבים ב-"premium pricing + cold UX". Inflow, Numo יושבים ב-"premium-with-coaching + billing complaints". Routinery, Trevor AI יושבים ב-"cheap + feature-light". Reclaim Lite, Indy יושבים ב-"free + limited". **רק Planny יושב ב-$9.99-with-no-shame-and-no-billing-tricks** — Brand promise פומבי על 30-day no-questions refund.

---

## ניתוח GTM של מתחרים — מה עובד / מה אסור

### עובד:

- **Sunsama:** 600+ creator ambassadors (SARAL) + Jessica McCabe / How to ADHD partnership → **TEMPLATE ל-Planny.** ניתן להעתיק ב-30 micro-creators + 1 tier-1 podcast ב-$1,500.
- **Inflow:** TikTok daily posts + quiz funnel + paid social — **אבל זה דורש $11M Series A**, לא $1,500.
- **Tiimo:** affiliate codes ל-TikTok creators (30% הנחה) + App Store featuring (App of Year 2025) + ND-affirming brand voice → earned media moat
- **Routinery:** ASO + App Store featuring (Editor's Choice May 2024, App of Day 2026) + aggressive low price = 5M+ downloads ב-minimal spend. 70% מההכנסות מארה"ב למרות 30% מהמשתמשים — **US ADHD audience = high-LTV.**

### אסור ל-Planny:

- **Meta paid social** (Inflow מתמחר אותך החוצה — $30-80 CAC iOS ADHD)
- **TikTok paid social** (אותה סיבה — Inflow השקיע מיליונים שם)
- **Google Search Ads "ADHD planner"** (saturated — Motion, Tiimo, Reclaim bid)
- **Generic productivity SEO** ("best AI calendar") — Motion, Sunsama, Reclaim dominated
- **Competing for App Store featuring על basic "ADHD app"** — Tiimo Apple-locked ל-12 חודשים. **המסלול:** ADHD Awareness Month (October 2026) + Women's History Month (March 2027) — נושאים שלא Tiimo locked.

### לא מנוצל (Planny's white space):

- **Tracy Otsuka — ADHD for Smart Ass Women** (8M downloads, women 25-40, 160 countries) — exact persona, אפס app sponsors. Single highest-leverage spend.
- **ADDitude "Women with ADHD" newsletter** (subset of 750K opt-in, 40% open rate) — אין app advertisers בולטים.
- **r/ADHDWomen** (700K members) — **אפס competitor presence.** Founder-led organic over 60-90 days.
- **Pinterest "ADHD planner"** — TAM גדולה, אפס מתחרה.
- **Katy Weber — Women & ADHD podcast**, **MissUnderstood** (Understood.org).
- **Referral programs** — אף אחד מ-6 המתחרים הראשיים לא הריץ אחד. give-a-month/get-a-month easy differentiator.

### Budget allocation ($1,500):

- $800 — Tracy Otsuka podcast sponsorship (single episode)
- $500 — ADDitude Women with ADHD newsletter sponsorship
- $200 — Apple Search Ads test על "ADHD weekly planner" long-tail (kill ב-CAC >$40)
- $0 — Creator gifting (30 ADHD micro-creators @ free annual sub)
- $0 — Reddit/SEO/TikTok founder-led organic

---

## הערכת סיכון פלטפורמה

### Apple (Severe risk)

- **רכישת Mayday Labs (April 2024)** — sunset May 2024. Mayday's tech: "AI-Schedule Tasks" + "Ideal Time Scheduling Engine" = **בדיוק ה-feature set של Motion/Reclaim/Planny**, כבר 2+ שנים בפיתוח פנים-Apple.
- **WWDC June 8, 2026 (~10 ימים מהיום)** — Siri 2.0 overhaul הוא ה-headline feature. Personal context (private on-device knowledge graph). Calendar app gets Apple Intelligence. iOS 27 ships ספטמבר 2026.
- iPhone heavy = ה-beachhead של Planny (US women 25-40 = iPhone-heavy).
- **תוכנית תגובה:**
  - **War-room ב-WWDC (June 8-15)** — תוכן תגובתי מוכן מראש בשלושה תרחישים:
    - (a) Apple ships heavy AI calendar → pivot ל-"ADHD-specific layer on top of Apple Intelligence"
    - (b) Apple ships light → double down "Apple won't build this for ADHD adults specifically"
    - (c) Apple דוחה Siri 2.0 שוב (Apple דחתה Personalized Siri ב-March 2025 — credibility deficit) → "promised, undelivered"
  - **Own the ADHD-native UX layer** ש-Apple לא תבנה (horizontal vs vertical)
  - **Use Apple Intelligence as infrastructure** — EventKit, Shortcuts, on-device LLM, "Hey Siri, ask Planny to reschedule"
  - **Cross-platform from day 1** — US Android 40%+, אסור לבטוח ב-iOS exclusivity

### Google (Moderate-High)

- **Gemini Spark** (גוייס במאי 2026) — agent persistent בענן, accesses Gmail/Calendar/Docs, reschedules meetings, finds slots. **$100/mo Ultra gate = הסיכון מתון מהפרסונה של Planny (cost-sensitive).**
- **Daily Brief** (ב-tiers זולים יותר $20 AI Pro) — morning digest מ-Gmail/Calendar/Tasks. **זה האיום הקרוב יותר** ל-Planny's morning planning use case.
- **תוכנית תגובה:**
  - Integrate ב-Google Calendar **כ-source לא כ-competitor** (read-only sync, Planny adds ADHD layer)
  - Position: "Spark does 100 things. Planny does one — your week, your way."
  - Watch Daily Brief expansion ל-free tier (= reevaluation moment)

### Microsoft (Lower)

- **Copilot in Outlook agentic (April 2026)** — triage, reschedule conflicts, focus blocks, "Calendar Instructions". **אבל enterprise-skewed** — Planny's persona היא personal mobile, לא Outlook desktop.
- **תוכנית תגובה:** Don't optimize for Outlook; partner via Microsoft Graph read-only sync if persona-relevant.

### OpenAI / ChatGPT (Rising)

- Custom GPTs ל-ADHD planning הם **organic trend ב-Reddit ו-ADDitude** — אפס marketing, awareness גובהה.
- Scheduled Actions + persistent Memory + (future) App Connectors ל-calendar = איום בינוני שעולה.
- **תוכנית תגובה:**
  - Acknowledge ChatGPT users פומבית במרקטינג: "if you already plan with ChatGPT, here's what Planny adds: persistence, notifications, calendar."
  - "Import from ChatGPT" onboarding flow (paste daily plan → Planny converts to blocks)
  - השתמש ב-OpenAI/Anthropic APIs מאחורי הקלעים — אל תתחרה על LLM quality raw

---

## ניתוח switching costs

### למה ADHD users נתקעים על הסטטוס קוו?

- **Already-paid sunk cost** — Hobonichi planner מינואר, Notion templates, Todoist Premium annual
- **Shared calendars עם partner/family** — Google Calendar קשה לעזוב
- **Work-mandated** — Outlook במשרד
- **"I tried 10 apps, none stuck"** — defensive, exhausted user (Reddit pattern)
- **Onboarding tax** — data entry friction = abandonment קלאסי ל-ADHD
- **Trust in fragile crutch** — switching = risking שנים של coping

### מי שעל Tiimo (פגיע ביותר):

- 75% מתסכלים מ-setup overwhelm
- One-way sync = users עוברים בין Tiimo ל-Apple Cal ידנית
- אין partner mode → couples עם ADHD partner נשארים עם conflict
- **Planny migration:** import calendar in one tap + auto-detect existing Tiimo patterns

### מי שעל Sunsama:

- Mobile read-only = תכנון פיזית רק ליד מחשב = friction יומיומי ל-ADHD
- $240/yr = sticker shock ל-consumer
- **Planny migration:** "Sunsama for ADHD, mobile-first, half the price"

### מי שעל Inflow:

- Billing reputation (Trustpilot, Reddit)
- לא planner — coaching אפליקציה. Users שמחפשים schedule הולכים לאיבוד.
- **Planny migration:** trust-led positioning, 30-day no-questions refund as brand promise

### מי שעל Apple Reminders + Calendar:

- ADHD-hostile design: red badges, single-fire notifications, no graduated reminders, no rescheduling on miss
- "out of sight, out of mind" object permanence problem
- **Planny migration:** graduated notifications + always-visible widget + lock-screen weekly view

### Onboarding requirement:

- **Sub-90-second setup** — connect Apple/Google Calendar in one tap, auto-detect existing patterns
- **First-week visible win** — "you reclaimed X hours" or "completed Y blocks"
- **Two brain-dumps שבועיים = ערך מצטבר** → 14-day trial הוא הנכון (לא 7-day; RevenueCat 2025: 84% של 3-day ו-64% של 7-day cancel נופלים יום 0-1)

---

## ניתוח פגיעות — איזה מתחרה הכי פגיע?

**Ranking של פגיעות (highest → lowest):**

1. **Tiimo — HIGHEST.** One-way sync + setup overwhelm + no partner mode + Android-late. **Planny תוקף שלוש פגיעויות אלה ישירות.** ה-Apple Award קונה לו 12-24 חודשים, אבל ה-feature gaps שלו מתועדים פומבית ב-tiimo.nolt.io.
2. **Inflow — HIGH.** Billing reputation שאינה ברת-תיקון בלי הודאה פומבית. Trust-led positioning של Planny מנצל את זה ישירות. Inflow לא ייאלץ להגיב כי הם לא planner.
3. **Sunsama — MEDIUM-HIGH.** Mobile read-only הוא feature gap שהם מודעים אליו אבל לא משחררים. "Timeboxing 2.0" שובש (היה אמור H2 2025, May 2026 unconfirmed).
4. **Numo — MEDIUM.** Crashes, glitches, cancellation friction (App Store reviews). Brand voice טוב, product weak.
5. **Saner.AI — MEDIUM (rising).** Pricing לא פומבי, scope broad, אין persona narrow. אם Planny ינעל persona מהר, Saner יהיה מעט פחות איום.

**Planny תוקף 3 נקודות כאב במקביל:**
- Tiimo's sync + partner gap
- Inflow's billing reputation
- Sunsama's mobile gap

---

## המלצות אסטרטגיות

1. **Wedge טכני — Two-way calendar sync:** EventKit ישיר ל-Apple + Google Calendar OAuth ישיר, **לא דרך iCloud sync** (זו הסיבה שמתחרים נכשלים). יציאה ראשונה לפני Tiimo משחרר את ה-Nolt feature היא קריטית — חלון של 6-12 חודשים. **Apple WWDC ב-10 ימים = פעולה דחופה: לבדוק אילו EventKit APIs מתעדכנים, להתאים architecture.**

2. **Wedge חוויתי — 30-second start עם voice brain-dump:** Tiimo's Co-planner הוא text+voice young; אף מתחרה לא מאחד voice-capture → AI-schedule → ADHD context → calendar write. **זה ה-wow moment** של ההדגמה הראשונה ב-TikTok וב-podcast ads.

3. **Wedge אתי — 30-day no-questions-asked refund + transparent cancel:** מפורסם כ-brand promise פומבי. Inflow ו-Numo נכשלים פומבית בזה. **זה הניצחון הזול ביותר ב-trust** ב-late-diagnosed women persona (skeptical, burned-before).

4. **Wedge פוזישני — "By an ADHD adult, for ADHD adults — late-diagnosed women, no shame, no streaks":** Persona narrow ש-Tiimo (neurodivergent רחב), Saner (knowledge workers), Motion (B2B) לא תובעים. **כל copy, כל TikTok, כל podcast ad חייב להחזיק את ה-line הזה.**

5. **Wedge GTM — Sunsama playbook ב-1/100 התקציב:** 30 ADHD micro-creators @ gifted annual sub + Tracy Otsuka podcast + ADDitude newsletter + r/ADHDWomen 90-day founder-led organic. **אסור לגעת ב-Meta/TikTok paid.**

6. **Partnerships ל-leverage:**
   - **Tracy Otsuka** (ADHD for Smart Ass Women, 8M downloads) — single episode sponsorship $800-1500
   - **Focusmate** integration (body-doubling) — adjacent product, audience overlap
   - **ADHD coaches** (B2B2C "your coach's homework, automated") — Shimmer competitive but smaller coaches receptive
   - **AVOID:** Jessica McCabe (Sunsama locked), Inflow (paid social conflict)

7. **Acceleration signal:** Saner.AI Series Seed (6-12 חודשים) = marketing surge. **תהדק launch ל-9-12 חודשים** במקום 12-18 (Wave 1 baseline), עם waitlist + community נופתים ב-60 הימים הבאים כדי ללכוד mindshare לפני.

---

## פערי נתונים תחרותיים אגרגטיביים

- **Saner.AI pricing** — לא פומבי. חוסר חיוני ל-competitive positioning.
- **Saner.AI founders + LinkedIn backgrounds** — לא חשף בחיפושים. נדרש direct LinkedIn pass.
- **Indy by Shimmer pricing tiers** (post-beta) — TBD.
- **CAC verified figures** לכל המתחרים — כולם משוערים מ-category benchmarks (Apple Ads $3-10 CPI; Meta health $30-80).
- **Trial-to-paid conversion rates** ספציפיים ל-Tiimo, Inflow, Sunsama — רק category medians (~12% hard paywall, 18-25% opt-in trial, 49-60% opt-out trial).
- **Numo, Akiflow, Amie, Trevor AI:** exact ARR / paying users / team sizes — DATA GAP בכולם.
- **Tiimo Android maturity** — claims of beta/limited; parity status unconfirmed.
- **Sunsama Timeboxing 2.0** — היה אמור H2 2025; status May 2026 unconfirmed.
- **App Store / Play Store install counts** — אף אחד מהאינדים (Flint, Lately, neurolist, MyADHD) לא חשף verifiable numbers; נדרש Sensor Tower paid query.
- **YC W25/S25/W26 ADHD-specific entries** — חיפושים החזירו aggregate batch info; נדרש direct yc.com search על industry:health + tags:adhd.
- **Israel-market emerging competitors** — Wave 2 pass היה US-centric; pass יעודי נדרש.
- **Reddit r/ADHD ו-r/ADHDWomen verbatim quotes** — WebSearch returned summaries only; manual scraping needed.
- **WWDC 2026 actual scheduling features** — Inference based on Mayday acquisition + code leaks; **definitive on June 8, 2026** (10 ימים).
- **Gemini Spark adoption curve** — שוגרה May 2026, רק AI Ultra subs ($100/mo) — early adopters לא נמדדו.

---

## Sources

### Tier 1 (highest):
- SEC 8-K filing (Dropbox acquisition of Reclaim.ai, $40.2M, Aug 2024)
- Pricing pages: tiimoapp.com, usemotion.com, reclaim.ai, sunsama.com, akiflow.com, routinery.app, numo.ai, inflow/getinflow.io, trevor.ai
- Google blog (I/O 2026 announcements): https://blog.google/innovation-and-ai/technology/ai/google-io-2026-all-our-announcements/
- gemini.google/overview/agent/spark/
- Saner.AI homepage + PitchBook + Crunchbase + Tracxn profiles
- YC company directories (Inflow, Shimmer)

### Tier 2:
- TechCrunch (Inflow Series A $11M Jan 2023; Shimmer $2.2M Jan 2024; Dropbox-Reclaim acquisition; Lately gamified launch Apr 2025)
- Crunchbase, Tracxn, Latka, ARR Club (Motion $50M ARR Aug 2025)
- Daring Fireball (Apple iPhone App of the Year 2025; Apple Siri delay March 2025)
- Sifted (Tiimo profile, downloads, B2B plans)
- SARAL case study (Sunsama 600+ creators, How to ADHD partnership)
- Octopus Ventures blog (Inflow channel mix)
- MacRumors / 9to5Mac / AppleInsider (Mayday acquisition Apr 2024; iOS 27 calendar AI; WWDC 2026 June 8 preview)
- Bloomberg (iOS 27 model swap)
- Engadget / 9to5Google / Tom's Guide / Techlicious (Gemini Spark May 2026)
- Microsoft Tech Community blog (Copilot Outlook agentic Apr 2026)
- Macworld, eWeek, Business Standard, BusinessToday (WWDC 2026)
- Cantech Letter (Flint launch, North Vancouver dad), Philly Mag (NoPlex), Femtech Insider (Shimmer)
- RevenueCat State of Subscription Apps 2025
- AppTweak Apple Ads Benchmarks 2025
- ADDitude advertising page (750K subscribers, 40% open rate)
- Tracy Otsuka — ADHD for Smart Ass Women podcast

### Tier 3:
- App Store / Google Play listings (neurolist, MyADHD TestFlight, Flint, Lately, Numo)
- Reddit summaries (r/ADHD, r/ADHDWomen) — sentiment directional only
- Comparison blogs: Morgen, Rivva, OnePageCRM, alfred_, Temporal — sponsor-adjacent
- Pretty Progress blog (Apple Reminders ADHD critique)
- Motley Bloom (Hobonichi-ADHD)
- Coaching Executive Function, New Frontiers, Shimmer.care (coaching pricing)
- Trustpilot review aggregation (Inflow billing complaints)
- Wishup, Oceanstalent, Wing (VA pricing aggregators)
- The Vibe With Ky (Indy review, Jan 15 2026)
- Product Hunt (Unloop Dec 2025, Saner.AI launch)
- SocialCat (ADHD influencer roundup)
- Tiimo Nolt feature request board (tiimo.nolt.io — two-way sync public request)
- ADHD Flow State Accelerator alumni signals

---

## Flags

### Red Flags:

- **Apple Mayday acquisition (Apr 2024) + iOS 27 calendar AI** = Apple בונה את ה-feature core של Planny. WWDC ב-June 8 = severe sherlocking risk ב-Planny's beachhead device. **Mitigation: own ADHD-specific UX vertical, cross-platform day 1, war-room week.**
- **Saner.AI היה צריך להיות ב-Wave 1.** Process flag — אם Saner נופל בפער, מה עוד פספסנו? **Mitigation: Wave 1 audit לפני B5.**
- **Indy by Shimmer (חינמית) + Shimmer $3.5M funded parent** = free competitor שמסבסד מ-coaching upsell. **Pricing strategy של Planny חייב לענות על זה לפני launch.** אם Planny עולה $9.99/mo ו-Indy חינמית, conversion יהיה אכזרי.
- **Capital מתקשה סביב ADHD-tech.** $2.7B global digital-health mental-health funding 2024 (+38% YoY); 65+ ADHD app funding rounds. **חלון 12-18 חודשים אמיתי אבל נסגר בפעולה.**
- **Tiimo Apple App of the Year 2025 + AI Co-planner** = brand + product momentum, לא paper threat.
- **Inflow billing/cancellation reputation** = reputation risk לכל הקטגוריה — Planny נכנס לתוך users skeptical.
- **Motion $550M val + $50M ARR + B2B pivot** = capacity לרכוש ADHD brand (Tiimo? Numo?) consumer entry.
- **Reclaim free forever + Dropbox distribution** = אם Dropbox משחרר Reclaim Mobile + ADHD framing, free competitor + Dropbox install base.
- **Gemini Spark shipping (May 2026) + Daily Brief** = Google מ-"rumor" ל-"shipping" ב-2 שבועות.
- **OpenAI ChatGPT custom GPTs ל-ADHD** organic Reddit traction + memory + (future) calendar connectors = near-zero CAC alternative.
- **ADHD coaching (Shimmer) $140-345/mo** = squeezing Planny מלמעלה ב-willingness-to-pay.
- **ADHD app retention brutal** (Wave 1: 3-4% Day-30 baseline). Planny must solve retention before scaling CAC.

### Yellow Flags:

- **WWDC 2026 (June 8, 10 ימים)** — platform tailwind או commoditization risk. Apple AI ship delays historically (Personalized Siri delayed Mar 2025) = 6-12 חודשי runway אפשרי.
- **Tiimo two-way sync feature request פומבי ב-Nolt** — אם Tiimo משחרר ראשון, calendar-write moat של Planny נסגר. **Move fast.**
- **Sunsama Timeboxing 2.0** אם יוצא יפה = absorbs late-dx adults שמתסכלים היום.
- **Notion + Notion Calendar** = decision אחד מ-"AI ADHD Planner templates."
- **Solo-founder indie launches clustering** (Flint, Lately, NoPlex 2025-2026) — קולקטיבי fragment App Store search, individually low-threat.
- **Techstars שתי השקעות ADHD-adjacent בשנתיים** (Saner.AI, Neurotype) = pattern, לא anomaly.
- **"Stoplight capacity check-in" (Flint) + "magic subtasks + voice playlist" (neurolist)** = strong ADHD-native UX innovations Planny doesn't have. Feature-gap risk.
- **Open-source ADHD tooling** (ADHDExec, Leantime) shallow but exists — well-funded fork = credible competitor.
- **ADHD Flow State Accelerator** = future-competitor generator. Monitor each cohort.
- **TikTok ADHD content misinformation risk** — 2022 CJP found 52% of top ADHD TikToks misleading. Clinical advisor endorsement חיוני ל-credibility ו-PR defense.
- **App Store featuring** דורש submitted nominations + Apple relationships — plan 4 חודשים מראש ל-ADHD Awareness Month (October), Women's History Month (March).
- **No ADHD app has visible referral program** — easy differentiator, test before over-investing (mobile referral mechanics יכולים להיות clunky).
- **Trial length:** 84% of 3-day, 64% of 7-day cancellations יום 0-1 (RevenueCat 2025). **14-day no-CC trial (Sunsama choice)** הוא הנכון.
