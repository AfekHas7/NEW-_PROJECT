# Business Model — startup-2 (RSVP-AI)

**Phase:** Phase 4 — Strategy
**Project:** startup-2
**Date:** 2026-05-29
**Confidence:** Medium-Low (unit economics תלויים ב-2 DATA GAPS: דקות voice בפועל + WTP אולם)

---

## Revenue Model

**B2B white-label, מבנה דו-רכיבי:**
1. **Retainer:** ₪290-490/אולם/חודש — מבטיח מרווח חיובי גם בחודש דליל (עונתיות).
2. **Per-guest wholesale:** ₪0.95/מוזמן — האולם גובה מהזוג 299-400₪/אירוע ומרוויח spread 30-50%.

**למה דו-רכיבי:** ה-retainer פותר את העונתיות (מאי-אוקט שיא, חורף דליל) ואת המלקחיים של COGS גבוה. בלי retainer, per-guest בלבד = אותה כלכלה שלילית של B2C.

## Unit Economics

| מדד | ערך | ביטחון |
|---|---|---|
| COGS/מוזמן | 0.6-0.85₪ | Medium (פרוקסי voice) |
| מחיר wholesale/מוזמן | 0.95₪ | Estimate |
| מרווח/מוזמן | 0.10-0.35₪ | דק — רגיש מאוד ל-COGS |
| Retainer/אולם/ח' | 290-490₪ | Estimate |
| הכנסה/אולם/שנה | 25,000-60,000₪ | Estimate (100 אירועים) |
| LTV אולם (3 שנים, churn 20%/שנה) | ~60-150K₪ | Estimate, Low |
| CAC אולם | זמן מכירה (≈₪0 כסף, גבוה בזמן) | Low |

> **🔴 רגישות קריטית:** המרווח/מוזמן (0.10-0.35₪) דק מאוד. אם דקות ה-voice בפועל גבוהות מההנחה (70%×2 דק' במקום 40%×1.5), COGS→~1.15₪ והמרווח **שלילי גם ב-wholesale 0.95₪**. ה-retainer הוא מה שמציל את המודל — לכן הוא לא אופציונלי.

## Scalability
- **חיובי:** marginal cost נמוך פר-אירוע; אולם אחד = עשרות אירועים (מינוף).
- **שלילי:** מכירה B2B לא-סקיילבילית (כל אולם = מכירה אישית); תפעול done-for-you דורש יד מנהלת (קשה מרחוק); עונתיות.
- **תקרה:** ~6-12 אולמות פעילים = ~300K₪ ARR. bootstrap, לא venture.

## Dependencies & Key Partnerships
- **Yappr** (voice עברית) — partner, לא build.
- **360dialog/Twilio** (WhatsApp BSP) — partner.
- **אולמות/קייטרינג** — שותפי הפצה + לקוחות (ה-moat).
- **עו"ד תקשורת/פרטיות** — חוו"ד gate.

## Build vs Buy
**PARTNER על הכל הטכנולוגי** — ה-voice וה-WhatsApp קומודיטי. ה-IP היחיד שכדאי לבנות: שכבת ה-orchestration + דשבורד דיוק-המנות + ה-white-label. שם הערך המוסף, לא בקול.

---

## Flags
**Red Flags:** מרווח דק ושביר ל-COGS; תלוי ב-retainer; מכירה B2B לא-סקיילבילית.
**Yellow Flags:** עונתיות; תקרת ARR נמוכה; CAC בזמן גבוה למייסד יחיד מרחוק.

## Sources
- market-analysis.md, raw/pricing-deep-dive.md, raw/partnerships.md
