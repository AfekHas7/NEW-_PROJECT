# Assumptions Tracker — AuditPilot

**Phase:** Phase 8 — Validation
**Project:** startup-3
**Date:** 2026-05-31

> Status: untested / testing / validated / invalidated

---

| # | הנחה | Confidence | איך לבדוק | Status | קריטיות |
|---|------|-----------|-----------|--------|---------|
| A1 | **מנוף מומחה: 8-15h/לקוח first-time** | Low | POC עם האב (ניסוי 3) | untested | 🔴 EXISTENTIAL |
| A2 | **AI מפיק QMS clause-grounded מספיק טוב ש-reviewer בודק-לא-כותב** | Low-Med | POC + ממצאי Stage 2 | untested | 🔴 EXISTENTIAL |
| A3 | **registrar/auditor מקבל הכנה AI-native** (יש רשומות אמיתיות) | Med (Tier 2) | ראיונות auditors (ניסוי 1) + 17021 §5 | untested | 🔴 EXISTENTIAL |
| A4 | **record-generation: ניתן להוביל לקוח לייצר רשומות אמיתיות ב-6-8 שב'** | Low | pilots (ניסוי 6) | untested | 🔴 |
| A5 | **WTP: ₪12-15K עבור Core** | Med | ראיונות (ניסוי 2) + pilots | untested | 🔴 |
| A6 | **maintenance attach ≥50%** (האנונה = LTV) | Low-Med | הצעה ל-pilots (ניסוי 7) | untested | 🟡 |
| A7 | **זרימת לידים מספקת ב-SAM קטן** (~30 לקוחות Y1) | Low | landing+quiz+tender (ניסויים 4-5) | untested | 🔴 |
| A8 | **trigger = מכרז/לקוח/יצוא** (trigger-driven) | Med-High | ראיונות + tender data | partial | 🟡 |
| A9 | **Hebrew SEO niche לא-רווי, keywords בעלי intent** | Med | Ahrefs/Semrush חודש | untested | 🟡 |
| A10 | **האב מחויב, זמין, ומספיק קיבולת** (FMF) | Med | הסכם אקוויטי + capacity check | partial | 🔴 |
| A11 | **אין מתחרה ישראלי AI-native שנכנס ב-12ח'** (Scytale) | Med | ניטור רבעוני | untested | 🟡 |
| A12 | **gross margin בריא בתמחור** (cash) | Med-High | מודל + pilots | partial | 🟡 |
| A13 | **privacy/legal פתיר ב-~$1-3K** | Med | חוו"ד עו"ד | untested | 🟡 |
| A14 | **commitment מספיק** (מול 3 סטארטאפים) | Low-Med | self-eval Day 30/60/90 | ongoing | 🟡 |

## ההנחות ה-EXISTENTIAL (אם נופלות → אין עסק)
- **A1+A2 (מנוף + איכות AI):** הלב הכלכלי. נבדקות יחד ב-POC. אם נופלות → המודל הוא "יועץ עם AI assist", לא "AI-native service" → margin/scale קורסים (טעות startup-2).
- **A3 (קבילות):** נחקרה כ-Medium (לא killed), אך דורשת אישור auditor ראשוני.
- **A5+A7 (WTP + לידים):** האם יש שוק משלם נגיש ב-SAM קטן.

## Flags
**Red Flags:** 5 הנחות existential (A1-A3, A5, A7) — כולן untested. זה ה-state הנכון לפני validation, אבל אומר שה-thesis עדיין היפותזה.
**Yellow Flags:** A10 (תלות אב) ו-A14 (commitment) הם סיכוני founder שחוזרים מ-Planny/startup-2.
