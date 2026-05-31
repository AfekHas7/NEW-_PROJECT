# MVP Definition — AuditPilot

**Phase:** Phase 6 — Product
**Project:** startup-3
**Date:** 2026-05-31
**Confidence:** Medium

---

## Core Hypothesis ש-ה-MVP בודק
**"AI + פיקוח מומחה קל (8-15 שעות/לקוח) יכולים להפיק QMS ל-ISO 9001 שעובר מבדק Stage 2 בפועל — כולל רשומות אמיתיות, לא רק מסמכים."**
זו ההנחה הכלכלית והרגולטורית המרכזית גם יחד. אם נכון → ה-thesis עובד. אם הפיקוח 25-40 שעות → המנוף קורס.

## Must-Have Features (המינימום לבדיקת ההיפותזה)
1. **Intake + gap-analysis** — הלקוח מעלה מסמכים קיימים + עונה על שאלון פעילות; AI ממפה מול clauses 4-10 ומפיק דוח פערים. (גם ה-wedge השיווקי החינמי.)
2. **AI QMS generator** — מייצר מדריך איכות, נהלים, הוראות עבודה, **תבניות רשומות** — clause-grounded (נגד hallucination), מותאם לפעילות.
3. **תוכנית יישום + record-generation tracking** — לוח עבודה עד יום המבדק; מנגנון שמוביל את הלקוח לייצר **רשומות אמיתיות** (מבדק פנימי, סקר הנהלה, פעולות מתקנות) לאורך ~6-8 שבועות. ← **הליבה שמבדילה מ"מחולל מסמכים".**
4. **Expert review workflow** — תור משימות למומחה (האב): נקודות קריטיות בלבד, אישור/דחייה, חתימה. **מודד שעות פיקוח** (ה-KPI).
5. **Client portal** — העלאת מסמכים מאובטחת, progress, מה נדרש מהלקוח.

## Nice-to-Have (v1.1, לא v1.0)
- IMS multi-standard (14001/45001/27001).
- אנגלית/לוקליזציה (UK).
- אינטגרציית Priority ERP (pull data).
- automated internal-audit simulation.
- דשבורד אנליטיקס ל-pass-rate.

## Explicitly Out of Scope (נגד scope creep)
- **המבדק עצמו** — מבוצע ע"י registrar עצמאי (SII/IQC). אנחנו מכינים בלבד (impartiality).
- ISO 13485/high-stakes.
- שווקים לא-ישראליים ב-v1.
- הפיכה ל-CB / certification arm (לעולם — impartiality).

## Success Criteria (מה יאמת את ה-MVP)
- **2-3 לקוחות pilot עוברים מבדק Stage 2** (pass rate ≥ ~90% norm). ← ה-north star.
- **שעות פיקוח מומחה ≤ ~15/לקוח** (ה-KPI הכלכלי). אם >20 → דגל.
- ≥1 לקוח ממיר ל-אנונת תחזוקה.
- WTP מאומת: לקוחות משלמים ₪12-15K (Core).
- registrar/auditor לא מעלה בעיה עם המקור AI-native של המסמכים (כל עוד יש רשומות אמיתיות).

## Flags
**Red Flags:** ה-MVP חייב להוכיח שעות-מומחה נמוכות *ו*-pass-rate גבוה בו-זמנית — אם trade-off ביניהם (פחות שעות → fail; pass → הרבה שעות), ה-thesis בסכנה.
**Yellow Flags:** ייצור הרשומות האמיתיות תלוי בשיתוף-פעולה של הלקוח לאורך 6-8 שבועות — drop-off risk.
