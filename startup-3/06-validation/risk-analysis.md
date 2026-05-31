# Risk Analysis — AuditPilot

**Phase:** Phase 8 — Validation
**Project:** startup-3
**Date:** 2026-05-31

> Likelihood × Impact (L/M/H). מדורג לפי חומרה.

---

## Risk Matrix

| # | סיכון | קטגוריה | L | I | חומרה | מיטיגציה + early warning |
|---|-------|---------|---|---|-------|--------------------------|
| R1 | **מנוף מומחה כבד (25-40h/לקוח)** → המודל "אחד לעשרות" קורס | Business | M | H | 🔴 קריטי | POC (ניסוי 3) לפני בנייה; אם >20h — pivot/עצור. EW: שעות ב-pilots. |
| R2 | **"מחולל מסמכים" שנכשל במבדק** (docs ≠ records) → certificate-mill, נזק מותגי | Product/Reg | M | H | 🔴 | record-generation tracking; audit guarantee; ניהול יישום אמיתי. EW: ממצאי Stage 2 ב-pilots. |
| R3 | **אין moat טכני; Scytale/AuditsReady/Vanta MSP נכנסים ל-9001 ישראל** | Market | M-H | H | 🔴 | speed; distribution moat (רשת האב, primes); data flywheel; vertical depth. EW: ניטור Scytale roadmap. |
| R4 | **תלות במומחה יחיד (אב)** — לא זמין/יוצא | Team | M | H | 🔴 | הסכם אקוויטי ברור; תיעוד ידע→system; גיוס מומחה 2 ב-Y2. EW: עומס/זמינות אב. |
| R5 | **SAM ישראלי קטן + מתכווץ** → תקרת לידים | Market | M | M-H | 🟡 | הרחבת UK/IMS מוקדמת; tender-intercept; primes. EW: lead flow Q2-Q3. |
| R6 | **WTP נמוך מהצפוי** (לקוח מעדיף DIY/Fiverr זול) | Market | M | M | 🟡 | ראיונות (ניסוי 2); מיצוב value (pass+accountability); guarantee. EW: conversion ב-pilots. |
| R7 | **trust gap מול AI vendor** חוסם מכירות | Market | M | M | 🟡 | named expert + guarantee + case studies; "human on the hook". EW: שיעור התנגדות "זה AI?". |
| R8 | **retention אנונה נמוך** (לקוח "עושה לבד") → LTV קורס | Business | M | M | 🟡 | ערך מתמשך (ניטור/עדכוני תקן/מבדק פנימי); recert lock. EW: attach rate ב-pilots. |
| R9 | **רגולציה: impartiality breach** (אם נכנסים ל-certification) | Regulatory | L | H | 🟡 | לעולם לא להיות preparer+certifier; arm's-length CB. EW: ביקורת legal. |
| R10 | **privacy (Amendment 13)** — מסמכי לקוח ל-LLM | Regulatory | M | M | 🟡 | DPA, data-residency, consent. EW: legal review לפני launch. |
| R11 | **commitment מחולק** (3 סטארטאפים) | Team | M | M | 🟡 | apples-to-apples decision; להתחייב לאחד. EW: קצב התקדמות. |
| R12 | **ניהול תפעולי מרחוק** (נסיעת ארה"ב) | Team | M | L-M | 🟢 | תהליך לא real-time-critical (שבועות); portal+async. EW: זמני תגובה. |

## High-Priority Risks — פירוט
- **R1 (מנוף):** ה-existential הכלכלי. כל המודל (margin + capacity + תמחור) נשען על 8-15h. זהה במהותו ל-trap של startup-2 ("AI=זול" הופרך). **חובה POC לפני בנייה.**
- **R2 (מחולל מסמכים):** ה-existential הרגולטורי. אם הערך מצטמצם למסמכים → קומודיטי שגם נכשל במבדק. ה-defensible (record-generation) הוא גם ה-feature בעל confidence הנמוך ביותר לבנייה.
- **R3 (אין moat):** window 12-18ח'. ה-defense היחיד = execution speed + distribution.
- **R4 (תלות אב):** ה-FMF כולו עליו. single-point-of-failure.

## Flags
**Red Flags:** R1+R2+R3+R4 — ארבעה סיכונים בחומרה גבוהה, יותר מ-Planny (שהיה לו בעיקר WWDC+retention). אך כולם **controllable/testable** ב-validation, ואין ביניהם fatal-by-default (שלא כמו ה-margin השלילי של startup-2).
**Yellow Flags:** R5-R11 — אשכול סיכוני שוק/team סטנדרטיים ל-bootstrap B2B.
