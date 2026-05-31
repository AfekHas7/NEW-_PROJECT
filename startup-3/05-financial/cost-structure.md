# Cost Structure — AuditPilot

**Phase:** Phase 7 — Financial
**Project:** startup-3
**Date:** 2026-05-31
**Confidence:** Medium

---

## Fixed Costs (חודשי, שנה-1)
| פריט | עלות |
|------|------|
| Hosting + portal infra | ~$30-60 |
| LLM API (base load) | ~$50-150 (משתנה עם volume) |
| SEO tool (Ahrefs/Semrush) | ~$100-200 (לאמת keywords; אפשר לבטל אחרי) |
| Tender alerts (Wizbiz) | ~$50-150 |
| Misc tooling (quiz, email) | ~$30-50 |
| **סה"כ** | **~$300-550/חודש** |

> משכורות: $0 (מייסד + אב על reinvestment/equity, ללא משכורת — carryover).

## Variable Costs (פר-לקוח)
| פריט | עלות | הערה |
|------|------|------|
| LLM generation/לקוח | ~$20-50 | clause-grounded, מסמכים + iterations |
| **זמן מומחה (האב)** | 8-15h first-time, 2-5h/yr maintenance | **העלות "היקרה" — אך equity, לא cash. ה-constraint הוא קיבולת לא תזרים.** |
| תמיכת לקוח/onboarding | זמן מייסד | — |

## One-Time Costs
| פריט | עלות |
|------|------|
| בניית המנוע (MVP) | זמן מייסד (vibe-coded, AI-assisted) ~$0 cash |
| **Legal: DPA/privacy (Amendment 13) + impartiality review** | ~$1,000-3,000 ⚠️ |
| domain + brand assets | ~$100-300 |

## Break-Even Analysis
- עלות cash חודשית ~$400 → break-even על cash הוא **~1-2 לקוחות Core/חודש** (margin cash גבוה כי האב = equity).
- **ה-constraint האמיתי אינו cash break-even** (כמעט מיידי ב-organic) — אלא **קיבולת המומחה** ו**זרימת לידים**.
- אם מתמחרים את שעות האב בעלות-הזדמנות (~$100-150/h × 12h = $1,200-1,800/לקוח) → margin על Core ($3.5K) עדיין בריא ~50-65%, **אם** השעות נשארות נמוכות. ב-25h → margin מתכווץ ל-~10-30%.

## Comparison ל-prior two
- שלא כמו startup-2 (margin שלילי במחיר שוק) — כאן ה-cash margin בריא וה-break-even מיידי. **הסיכון הכלכלי כאן אינו "האם יש margin" אלא "האם המנוף מאפשר scale" + "האם יש מספיק לידים ב-SAM קטן".**

## Flags
**Red Flags:** עלות שעות-מומחה (גם אם equity) היא ה-capacity bottleneck; legal/privacy הוא one-time שחוסם launch (~$1-3K — נתח מ-seed/reinvestment).
**Yellow Flags:** LLM cost runaway אם iterations רבות/לקוח (heavy clients); SEO tool הוא הוצאה שמצדיקה רק אם keywords מאומתים.
