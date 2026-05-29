# MVP Definition — startup-2 (RSVP-AI)

**Phase:** Phase 6 — Product
**Project:** startup-2
**Date:** 2026-05-29
**Confidence:** Medium

> מבוסס pain hierarchy (target-audience.md) + competitor gaps (competitor-landscape.md). מודל B2B white-label.

---

## Core Hypothesis ש-MVP בודק
**"אולם ישלם retainer + per-guest עבור מנוע אישורי הגעה white-label שמספק מספר מנות מדויק 24-48 ש' לפני — והדיוק יהיה גבוה מספיק כדי לחסוך לו כסף אמיתי על מנות."**

(שתי הנחות existential נבדקות כאן: WTP אולם + יעילות הדיוק בפועל.)

## Must-Have Features (המינימום לבדיקת ההיפותזה)
1. **ייבוא רשימת מוזמנים** (Excel/Google Sheets/CSV).
2. **שליחת WhatsApp** ממספר מאושר + טופס אישור (כן/לא/+N).
3. **תזכורות אוטומטיות** למי שלא ענה.
4. **voice fallback (Yappr)** למי שלא ענה גם אחרי תזכורת — שיחת 10 ש' לוגיסטית. *(ניתן לכבות אם POC נכשל.)*
5. **דשבורד דיוק-מנות לאולם** — סטטוסים בזמן אמת, התראת פערים, **דוח 48 ש' לפני**.
6. **White-label בסיסי** — שם/לוגו האולם על ההודעות והדוח.
7. **מנגנון opt-out + תיעוד הסכמה** — *(הכרח רגולטורי, לא nice-to-have).*

## Nice-to-Have (v1.1, לא v1.0)
- העדפות אוכל / שיבוץ שולחנות.
- סנכרון headcount בזמן אמת לקייטרינג (API).
- דשבורד לזוג.
- חיוב/תשלום אוטומטי לאולם.

## Out of Scope (מניעת scope creep)
- בר/בת מצווה, כנסים, מגזרים אחרים (ערבי/חרדי).
- אפליקציית מובייל native (web dashboard מספיק).
- voice בשפות נוספות.
- אינטגרציות עומק למערכות אולם.

## Success Criteria (מה יאמת)
- **3 פיילוטים** מסתיימים עם דיוק מנות טוב יותר מהבסיס (פער מצומצם).
- **≥3 אולמות** מסכימים לשלם retainer אחרי הקייס.
- COGS בפועל ≤0.85₪/מוזמן (דקות voice לא חורגות).
- אפס תקרית ספאם/תלונה משפטית.

---

## Flags
**Red Flags:** ה-MVP בודק 2 הנחות existential בו-זמנית (WTP + דיוק) — אם אחת נכשלת, המודל קורס.
**Yellow Flags:** voice fallback עלול להידרש להיכבות (סנטימנט) — אז הבידול נחלש עוד.

## Sources
- target-audience.md, competitor-landscape.md, raw/partnerships.md, raw/regulatory.md
