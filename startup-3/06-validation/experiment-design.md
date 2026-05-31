# Experiment Design — Top 3 — AuditPilot

**Phase:** Phase 8 — Validation
**Project:** startup-3
**Date:** 2026-05-31

> 3 הניסויים בעלי ה-leverage הגבוה ביותר, תוקפים את ה-existential assumptions לפני בניית קוד.

---

## ניסוי 1 — ראיונות Auditors (קבילות AI-native)
- **Hypothesis:** registrar מוסמך יסמיך חברה שהוכנה AI-native, כל עוד יש רשומות אמיתיות ויישום.
- **Method:** קרא ISO/IEC 17021-1 §5 + ISO 19011 verbatim. ראיין 3-5 lead auditors (דרך רשת האב + SII/IQC). שאל: "אם חברה הכינה QMS בעזרת AI + מומחה, אבל הרשומות אמיתיות והמערכת פועלת — יש בעיה?"
- **Metrics:** ≥4/5 "מקובל"; אפס "פסול עקרונית".
- **Success:** A3 validated. **Invalidate:** אם auditors דורשים יד אנושית כבדה ביישום → pivot ל-V6 (copilot ליועצים).
- **Timeline/cost:** שבוע / $0 (+ עלות תקן ISO).
- **Script:** "אני בודק שירות שמכין חברות ל-9001 עם AI ומומחה מלווה. מניסיונך כ-auditor — מה היית רוצה לראות כדי לאשר? איפה זה נופל?"

## ניסוי 2 — ראיונות WTP (persona "רונן")
- **Hypothesis:** מנהל תפעול שנדחף ל-9001 ישלם ₪12-15K עבור done-for-you מהיר עם guarantee.
- **Method:** 8-10 ראיונות (30 דק') עם מנהלי תפעול/איכות שעברו/עוברים 9001. סינון: עברו בשנתיים האחרונות או מול דדליין. דרך רשת האב + LinkedIn + תעשיינים.
- **Metrics:** ≥6/10 "הייתי משלם ₪12-15K"; ≥7/10 trigger=מכרז/לקוח/יצוא; ≥6/10 הביעו את ה-pain "יקר/איטי/template".
- **Success:** A5+A8 validated. **Invalidate:** אם רובם "הייתי עושה לבד/Fiverr" → WTP חלש.
- **Timeline/cost:** שבוע-שבועיים / $0.
- **שאלות מפתח:** "מה היה הכי מתסכל בתהליך?", "כמה שילמת/ציפית?", "מה היה משכנע אותך לסמוך על שירות מבוסס-AI?"

## ניסוי 3 — POC מנוף-מומחה (ה-existential הכלכלי) ⭐
- **Hypothesis:** AI + פיקוח אב = ≤15h/לקוח לתוצר pass-ready.
- **Method:** בנה QMS אמיתי ל-1-2 חברות (מ-pilots/רשת האב). ה-AI מייצר; **מדוד בשעון את שעות האב** (review/תיקון/אישור). עקוב עד מוכנות Stage 1.
- **Metrics:** שעות אב ≤15 (first-time); איכות תוצר שהאב מאשר כ-audit-ready; שיעור התיקונים של האב (אם האב משכתב >40% → ה-AI לא מספיק טוב = A2 נכשל).
- **Success:** A1+A2 validated → ה-thesis עומד. **Invalidate:** אם >20h או האב משכתב רוב → המנוף קורס, **עצור לפני בניית מוצר מלא.**
- **Timeline/cost:** 3-4 שבועות / זמן (אב + מייסד).
- **למה זה ה-#1:** זה ה-make-or-break של כל הסטארטאפ. כל המודל הכלכלי, התמחור, וה-scale נשענים עליו. כמו ש-Planny's existential היה retention ו-startup-2's היה WTP-של-אולם — **כאן זה מנוף המומחה.**

## Flags
**Red Flags:** שלושת הניסויים תלויים בגישה דרך האב (auditors, לקוחות, POC) — אם האב לא מגויס/זמin, ה-validation נחסם (R4).
**Yellow Flags:** POC דורש חברה אמיתית עם נתונים אמיתיים — לתאם pilot מוקדם.
