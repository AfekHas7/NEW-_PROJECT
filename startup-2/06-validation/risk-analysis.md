# Risk Analysis — startup-2 (RSVP-AI)

**Phase:** Phase 8 — Validation
**Project:** startup-2
**Date:** 2026-05-29
**Confidence:** Medium-High (סיכונים מבוססי Phase 3)

> Risk matrix: Likelihood (H>60% / M 20-60% / L<20%) × Impact (Critical/Major/Moderate/Minor).

---

## Risk Matrix

| # | סיכון | סוג | Likelihood | Impact | עדיפות |
|---|---|---|---|---|---|
| R1 | אולם לא ישלם (WTP נכשל) | Market | M-H | Critical | 🔴 מיידי |
| R2 | אין חפיר — מתחרה מוסיף AI / Lunsoul פונה ל-B2B | Business | **H** | Critical | 🔴 מיידי |
| R3 | רגולציה — תביעת ספאם / באן WhatsApp | Market/Legal | M | Critical | 🔴 מיידי |
| R4 | COGS חורג (voice) → מרווח שלילי | Financial | M | Major | 🔴 מיידי |
| R5 | סנטימנט שלילי ל-voice מבריח אורחים → דיוק נופל | Product | M-H | Major | 🟡 |
| R6 | תפעול מרחוק (ארה"ב) נכשל באירוע קריטי | Team/Ops | M | Major | 🟡 |
| R7 | פער מימוני (חוו"ד ₪15-40K >> seed) | Financial | H | Major | 🟡 |
| R8 | commitment מחולק (3 סטארטאפים) | Team | M | Major | 🟡 |
| R9 | עונתיות → תזרים לא אחיד | Financial | H | Moderate | 🟢 מנוהל ע"י retainer |
| R10 | שוק קטן — תקרת ARR נמוכה | Market | H | Moderate | 🟢 מקובל אם bootstrap |

---

## High-Priority Risks — מיטיגציה ואותות מקדימים

### R1 — אולם לא ישלם (WTP)
- **מיטיגציה:** E2 (ראיונות) לפני בנייה; "מנה מובטחת" כבר מגינה על אולם → ייתכן שהכאב לא חזק → לבדוק אם הכאב הוא של האולם או של הזוג.
- **אות מקדים:** <3/10 אולמות מביעים WTP.

### R2 — אין חפיר 🔴 (הסיכון הכי גבוה-סבירות)
- **מיטיגציה:** distribution moat — לנעול יחסי אולמות + מותג מהר (חלון 6-12 ח'). אבל זה moat נבנה, לא מובנה.
- **אות מקדים:** Lunsoul/מתחרה משיק B2B white-label; ספק voice (Wonderful) נכנס לאירועים.
- **[Opinion]** זה הסיכון שהכי קשה למתן — הוא מבני. גם אם הכל יעבוד, הקלות שבה מעתיקים אותך מגבילה את הערך לטווח ארוך.

### R3 — רגולציה
- **מיטיגציה:** E1 (ייעוץ) → חוו"ד מלאה; ארכיטקטורה הגנתית (תוכן לוגיסטי, opt-out, opt-in דרך מארח, תיעוד).
- **אות מקדים:** עו"ד אומר "סיכון גבוה"; תלונת אורח; ירידת דירוג WhatsApp.

### R4 — COGS חורג
- **מיטיגציה:** E3 (POC) מודד דקות אמיתיות; rate-limit על voice; retainer מכסה.
- **אות מקדים:** דקות voice בפועל > הנחה ב-POC.

---

## Flags
**Red Flags:** 4 סיכונים Critical (R1-R4), אחד מהם (R2, היעדר חפיר) בעל סבירות גבוהה וקשה-מאוד-למתן.
**Yellow Flags:** פער מימוני (R7); תפעול מרחוק (R6); commitment מחולק (R8).

## Sources
- כל Phase 3 + research-gate.md + frameworks.md (risk matrix)
