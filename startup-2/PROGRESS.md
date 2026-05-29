# PROGRESS — startup-2 (RSVP-AI)

**Project:** startup-2 — חברת אישורי הגעה אוטונומית לחתונות (ישראל-first)
**Start date:** 2026-05-29
**Language:** Hebrew (עברית)
**Mode:** Full Mode, **Deep Research tier** (per founder request — apples-to-apples עם Planny)
**Baseline for comparison:** Planny = 6.4/10 (CONDITIONAL GO). ראה `planny/06-validation/scorecard.md` (טבלת ההשוואה כוללת עמודת "Startup 2").

---

## Phase Checklist

- [x] **Phase 1: Intake** — `00-intake/brief.md` (2 סבבי שאלות + carryover מ-Planny)
- [ ] **Phase 2: Brainstorm** — `00-intake/brainstorm.md` (כולל B2C-vs-B2B variations)
- [ ] **Phase 2.5: Research Depth** — Deep (נעול ע"י המייסד)
- [ ] **Phase 3: Market Research** (4 waves) → `01-discovery/`
- [ ] **Phase 3.5a: Verification** → `01-discovery/verification-report.md`
- [ ] **Phase 3.5: Research Gate** → `01-discovery/research-gate.md`
- [ ] **Phase 4: Strategy** → `02-strategy/`
- [ ] **Phase 5: Brand** → `03-brand/`
- [ ] **Phase 6: Product** → `04-product/`
- [ ] **Phase 7: Financial** → `05-financial/`
- [ ] **Phase 8: Validation** → `06-validation/` (כולל scorecard להשוואה)
- [ ] **Final:** `README.md` + `action-plan-30-days.md` + Final Assessment Dashboard

---

## Session Notes / State

**2026-05-29:**
- Intake הושלם. אותו מייסד כמו Planny.
- **הבדל מבני מהותי מ-Planny:** Planny = consumer mobile app; כאן = done-for-you managed B2B/B2C service. Unit economics, sales motion, ו-FMF שונים לגמרי.
- **FMF: Moderate** (מפיק קטן לשעבר, גישה ראשונית, ללא קשרי אולמות עמוקים) — מול 8/10 של Planny. זהו ההבדל הצפוי הגדול בציון.
- 3 Red Flags + 5 Yellow Flags זוהו ב-intake.
- 5 שאלות פתוחות שהמחקר יכריע (B2C/B2B, עלות פר-מוזמן, WTP, רגולציה, איכות voice AI).

### עדיפויות מחקר (highest-risk first)
1. **רגולציה** — חוק הספאם (תיקון 40) + WhatsApp Business API policy + שיחות קוליות אוטומטיות. Existential gate.
2. **נוף תחרותי** — חברות אישורי הגעה בישראל (מי, תמחור, כמה אוטומציה כבר יש, distribution moat).
3. **Unit economics** — עלות WhatsApp BSP + voice AI בעברית (דקה/שיחה) + ניתוח, פר-מוזמן.
4. **גודל שוק** — # חתונות/שנה בישראל, # מוזמנים ממוצע, גודל שוק אישורי הגעה.
5. **B2C vs B2B** — buying behavior, מי משלם, ערוצי הפצה.

### Environment
- Agent tool זמין → spawn research subagents per wave.
- WebSearch זמין.
- Git: branch `claude/quirky-hamilton-QiIHk`, push אחרי כל phase.
