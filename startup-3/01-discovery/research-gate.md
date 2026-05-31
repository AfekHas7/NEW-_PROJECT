# Research Gate — AuditPilot (Phase 3.5 Go/No-Go)

**Phase:** Phase 3.5 — Research Gate
**Project:** startup-3
**Date:** 2026-05-31
**Baselines:** Planny YELLOW 6.5 (gate) → 6.4 (scorecard) · startup-2 YELLOW-RED ~4.5 (gate) → 4.3 (scorecard)

---

## "הנה מה שהמחקר מצא"

**גודל שוק:** Global services TAM ~$5-6B/yr (Tier 1 cert counts). **SAM ישראלי קטן ~$5-7M/yr** (~2,000 certs, +1.4%/שנה, SMB מתכווץ) — beachhead לאימות, **לא venture-scale**; Y1 SOM ~$130-270K. תקרת ה-SAM לא-מחייבת ל-$300K, מחייבת ל-$1M → חובה הרחבה (IMS cross-sell + UK).

**תחרות:** ISO 9001 הוא **whitespace** — כל ה-incumbents הממומנים (Vanta $4.15B, Drata, Delve $32M) ממקדים SOC2/27001 ומתעלמים מ-9001; **אפס יועצי 9001 ישראלים משתמשים ב-AI**. אבל **אין moat טכני** — המודל הוא YC pattern copyable; AuditsReady (US) כבר עושה את ה-thesis (mfg/docs-only), ו-Scytale (Israeli AI GRC) צעד אחד מהרעיון. **window רך 12-18 ח'.**

**ביקוש:** MEDIUM-STRONG. WTP מאומת (תחזוקה STRONG); AI-compliance buying מוכח באדג'נסי (Vanta $300M ARR). trigger-driven (מכרזים/יצוא). אבל 9001 חסר את ה-triggers הדחופים שנותנים ל-Vanta pricing power, ויש trust gap מול AI vendor.

**רגולציה (ה-existential):** **לא killed.** אין כלל נגד מסמכי AI/צד-שלישי. הקו הקשה = impartiality (preparer≠certifier). **הסיכון האמיתי = documentation-vs-implementation:** הערך חייב להיות "ניהול יישום שמייצר ראיות אמיתיות", לא "ייצור מסמכים" (שהוא קומודיטי שנכשל במבדק).

**תזמון:** עכשיו. רוויזיית ISO 9001 ספט' 2026 (transition wave) + labor vacuum + incumbents שמתעלמים מ-9001.

**FMF:** Moderate-plus. האב כשותף-אקוויטי-מומחה = נכס אמיתי (≠ startup-2), אבל ה-domain expertise **שאול** (לא של המייסד) ו-single-point-of-dependency.

---

## Reasoning Through the Verdict

זה הרעיון **החזק ביותר משלושת הסטארטאפים על מספר צירים אובייקטיביים**, ובו-זמנית בעל **שתי חולשות מבניות אמיתיות** שלא היו ל-Planny:

**מה שחזק (חזק יותר מ-Planny בכמה ממדים):**
- **Business model clarity גבוה** — B2B, ACVs מתועדים ($6-8K first-time, $1-3K/yr maintenance), WTP מאומת, **אנונת recert/surveillance מובנית שמתקנת את חולשת ה-LTV של שני הקודמים** (5yr LTV ~$10,700/logo). זה הציון שבו startup-3 מנצח את שניהם.
- **Whitespace + on-brand thesis** — ISO 9001 מוזנח ע"י כל הכסף החכם; ה-thesis הוא בדיוק מה ש-YC ביקש.
- **Existential cleared** — בשונה מ-startup-2 (unit economics שליליים), כאן הרגולציה והכלכלה *יכולות* לעבוד.

**מה שחלש (חלש יותר מ-Planny):**
- **אין moat טכני** — המודל copyable, window רך 12-18 ח', Scytale/AuditsReady צעד אחד. ל-Planny היה לפחות two-way OAuth wedge; כאן ה-defensibility היא execution+distribution בלבד.
- **FMF שאול** — האב הוא הנכס, לא המייסד. ל-Planny ה-ADHD היה non-replicable של *המייסד*. כאן יש single-point-of-dependency.

**ההכרעה לא ממוצעת — היא משוקללת:** הכוח של ה-business model + whitespace + regulatory-clearance עולה על החולשות, **כל עוד** ההנחה הכלכלית המרכזית (מנוף מומחה 8-15h/לקוח) מחזיקה. אם הפיקוח מתברר ככבד (25-40h, כמו יועץ) — ה-thesis קורס בדיוק כמו startup-2. זה ה-make-or-break היחיד.

---

## Verdict: 🟡🟢 YELLOW-GREEN (preliminary ~6.0-6.5/10)

**מעל startup-2 (4.3) בבירור, ובטווח של Planny (6.4) — כנראה צמוד.** ה-scorecard הסופי (Phase 8) יחדד אחרי ש-Phase 7 יבחן את ה-unit economics לעומק.

**המלצה: להמשיך לכל ה-phases** — (א) כי המייסד ביקש validation מלאה apples-to-apples; (ב) כי שלא כמו red-light, אין כאן fatal flaw — יש thesis בר-קיימא עם 3 הנחות לאימות זול; (ג) כי ה-Phase 4-7 יכריעו אם זה 6+ (proceed) או 5 (concerns).

### 3 ההנחות שחייבות להיבדק (זול, לפני בנייה רצינית)
1. **מנוף המומחה** — POC: בנה QMS אמיתי עם האב כ-reviewer, מדוד שעות פיקוח/לקוח. אם >20h → ה-thesis בסכנה.
2. **WTP + trust ישראלי** — 5-10 ראיונות מנהלי תפעול (persona "רונן") + 3-5 ראיונות lead auditors (SII/IQC) על קבילות AI-native.
3. **אנונת recert** — האם לקוח יישאר על מנוי תחזוקה או "יעשה לבד" אחרי שנה 1.

---

## Strategic Connections
- ה-positioning ב-Phase 4 חייב להישען על "ניהול יישום" (regulatory) + distribution moat ישראלי (לא AI) — ראה `competitor-landscape.md` + `industry-trends.md`.
- ה-business-model ב-Phase 4 + financial ב-Phase 7 חייבים לטפל במנוף המומחה כ-assumption מפורש (ראה `verification-report.md`).
- ה-validation ב-Phase 8 חייב לכלול את 3 ההנחות לעיל.

## Flags
**Red Flags:** אין moat טכני (window רך); מנוף מומחה לא-מאומת (existential כלכלי); FMF שאול (single-point-of-dependency).
**Yellow Flags:** SAM ישראלי קטן; 9001 חסר triggers דחופים; trust gap; commitment מחולק (3 סטארטאפים).
