# Feature Prioritization — startup-2 (RSVP-AI)

**Phase:** Phase 6 — Product
**Project:** startup-2
**Date:** 2026-05-29
**Confidence:** Medium

> MoSCoW + RICE. Effort ב-T-shirt sizing (מייסד יחיד, AI-assisted).

---

## MoSCoW

**Must have (MVP):**
- ייבוא רשימה (S) · שליחת WhatsApp + טופס (M) · תזכורות (S) · דשבורד דיוק-מנות + דוח 48ש' (L) · white-label בסיסי (M) · opt-out/תיעוד הסכמה (S, רגולטורי).

**Should have:**
- voice fallback Yappr (M) — *core לבידול אך תלוי POC*.
- ניהול מספר WhatsApp/BSP מאושר (M).

**Could have (v1.1):**
- העדפות אוכל (M) · סנכרון קייטרינג API (L) · דשבורד זוג (M) · חיוב אוטומטי (M).

**Won't have (this time):**
- אפליקציית native · שפות נוספות · בר/בת מצווה/כנסים · מגזרים ערבי/חרדי.

## RICE (top features)

| פיצ'ר | Reach | Impact | Conf | Effort (חודשי-אדם) | RICE |
|---|---|---|---|---|---|
| דשבורד דיוק-מנות + דוח 48ש' | כל אולם | 3 | 80% | 1.0 | **2.4** |
| WhatsApp + טופס | כל אירוע | 3 | 90% | 0.5 | **5.4** |
| opt-out/תיעוד (רגולטורי) | כל אירוע | 2 | 100% | 0.25 | **8.0** |
| תזכורות | כל אירוע | 2 | 90% | 0.25 | **7.2** |
| white-label | כל אולם | 2 | 80% | 0.5 | **3.2** |
| voice fallback | ~10-20% אורחים | 2 | 50% | 0.75 | **1.3** |

> **תובנה:** ה-RICE מאשר שה-voice fallback (ה-"wedge" המקורי) הוא דווקא **הכי נמוך** — confidence נמוך (סנטימנט), reach חלקי, effort גבוה. ה-value האמיתי הוא בדשבורד הדיוק + ה-pipeline של WhatsApp. **זה מחזק את המסקנה: ה-voice הוא feature, לא הסיפור.**

## Build Order
1. opt-out/תיעוד + WhatsApp + טופס + תזכורות (ה-pipeline הבסיסי, RICE גבוה, רגולטורי).
2. דשבורד דיוק-מנות + דוח (ה-value ל-B2B).
3. white-label.
4. voice fallback (רק אחרי POC מוצלח).

## Dependencies
- WhatsApp BSP מאושר (חוסם הכל).
- חוו"ד משפטית (חוסם launch).
- Yappr integration (חוסם voice בלבד).

---

## Flags
**Red Flags:** ה-wedge המקורי (voice) הכי נמוך ב-RICE — שאלה אם יש בכלל מוצר מבדל.
**Yellow Flags:** דשבורד הדיוק (ה-value העיקרי) הוא ה-Effort הגבוה ביותר.

## Sources
- mvp-definition.md, frameworks.md (RICE/MoSCoW), raw/regulatory.md
