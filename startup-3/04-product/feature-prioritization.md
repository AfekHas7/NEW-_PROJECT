# Feature Prioritization — AuditPilot

**Phase:** Phase 6 — Product
**Project:** startup-3
**Date:** 2026-05-31

---

## MoSCoW + RICE (build order)

| Feature | MoSCoW | Reach | Impact | Confidence | Effort | סדר |
|---------|--------|-------|--------|-----------|--------|-----|
| Intake + gap-analysis (clause mapping) | Must | גבוה | גבוה | בינוני | M | 1 |
| AI QMS generator (clause-grounded) | Must | גבוה | גבוה (ליבה) | בינוני | L | 2 |
| Expert review workflow + שעות-tracking | Must | גבוה | גבוה (KPI) | גבוה | S-M | 3 |
| תוכנית יישום + record-generation tracking | Must | גבוה | **גבוה (ה-defensible)** | נמוך-בינוני | L | 4 |
| Client portal (upload מאובטח, progress) | Must | גבוה | בינוני | גבוה | M | 5 |
| DPA/privacy + data-residency (Amendment 13) | Must | — | גבוה (legal) | גבוה | S-M | 6 |
| audit-readiness checklist/quiz (lead magnet) | Should | גבוה | בינוני (GTM) | גבוה | S | 7 |
| internal-audit simulation אוטומטי | Could | בינוני | בינוני | נמוך | M | v1.1 |
| IMS multi-standard (14001/45001/27001) | Could | בינוני | גבוה (LTV) | בינוני | L | v1.1 |
| אנגלית/UK localization | Could | — | גבוה (TAM) | בינוני | M | v1.2 |
| Priority ERP integration | Won't (now) | נמוך | בינוני | נמוך | L | post-PMF |

## Dependencies
- gap-analysis (1) → QMS generator (2) → תוכנית יישום (4) [שרשרת ליבה].
- Expert workflow (3) חוצה הכל (כל תוצר עובר אישור).
- DPA/privacy (6) **חוסם launch** (שולחים מסמכי לקוח ל-LLM) — לא ניתן לדחות.
- record-tracking (4) תלוי ב-portal (5) לאיסוף עדויות.

## Effort (T-shirt) ו-build order מומלץ
**Sprint 1 (wedge):** gap-analysis + quiz + portal skeleton + DPA → מאפשר lead-gen + pilot intake.
**Sprint 2 (core):** QMS generator + expert review workflow → מפיק תוצר ראשון, מודד שעות.
**Sprint 3 (defensible):** record-generation tracking + implementation plan → מבדיל מ-"מחולל מסמכים", מכין ל-Stage 2.
**Sprint 4:** ליטוש מ-pilots; הכנה ל-IMS/אנגלית רק אחרי PMF.

## Flags
**Red Flags:** feature 4 (record-generation) הוא ה-defensible אבל בעל confidence הנמוך ביותר — אם קשה לבנות אוטומציה שמובילה ליצירת רשומות אמיתיות, נשארים עם "מחולל מסמכים" (קומודיטי).
**Yellow Flags:** DPA/privacy הוא must שחוסם launch — לתקצב זמן/עלות legal מראש.
