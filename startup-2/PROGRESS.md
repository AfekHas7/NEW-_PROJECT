# PROGRESS — startup-2 (RSVP-AI)

**Project:** startup-2 — חברת אישורי הגעה אוטונומית לחתונות (ישראל-first)
**Start date:** 2026-05-29
**Language:** Hebrew (עברית)
**Mode:** Full Mode, **Deep Research tier** (per founder request — apples-to-apples עם Planny)
**Baseline for comparison:** Planny = 6.4/10 (CONDITIONAL GO). ראה `planny/06-validation/scorecard.md` (טבלת ההשוואה כוללת עמודת "Startup 2").

---

## Phase Checklist

- [x] **Phase 1: Intake** — `00-intake/brief.md` (2 סבבי שאלות + carryover מ-Planny)
- [x] **Phase 2: Brainstorm** — `00-intake/brainstorm.md` (כולל B2C-vs-B2B variations)
- [x] **Phase 2.5: Research Depth** — Deep (נעול ע"י המייסד)
- [x] **Phase 3: Market Research** (4 waves, 15 agents) → `01-discovery/` ✅
  - [x] Wave 1-4 (all 15 raw files) ✅
  - [x] Synthesis: 5 deliverables (market-analysis, competitor-landscape, target-audience, industry-trends, confidence-dashboard) ✅
- [x] **Phase 3.5a: Verification** → `01-discovery/verification-report.md` (2 critical fixed) ✅
- [x] **Phase 3.5: Research Gate** → `01-discovery/research-gate.md` — **YELLOW-RED ~4.5/10** ✅
  - המייסד בחר: **להשלים את כל ה-phases** על מודל B2B white-label (השוואה מלאה מול Planny)
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

### ממצאי מחקר מצטברים (Wave 1-2)
- **שוק:** TAM ~29-58M₪/שנה — קטן, מתכווץ, עונתי חריף (מאי-אוקט). לא venture-scale.
- **כלכלה:** B2C = רכישה חד-פעמית, LTV:CAC ~3.3:1 שביר. B2B-אולמות = LTV פי 50-100, 12-30:1. → נטייה ברורה ל-B2B.
- **תחרות (קשה):** 11+ מתחרים. **Lunsoul כמעט זהה** (voice-AI + WhatsApp + אנושי + 6 שפות + אולמות) במחיר רצפה 99₪. WiWi done-for-you 1.7-1.9₪.
- **חפיר:** ~אין. voice-AI = off-the-shelf, עלויות מעבר אפסיות, בידול ניתן-להעתקה. distribution+מותג בידי ותיקים.
- **רגולציה: HIGH risk.** ספאם (סעיף 30א) + פרטיות (תיקון 13) + סיכון באן WhatsApp. חוו"ד משפטית (₪15-40K) חובה לפני launch.
- **תזמון:** חלון טכנולוגי 6-12 ח'. voice-AI בעברית "טוב מספיק". הון זורם → חסם כניסה יורד.
- **סתירה לאימות:** B1 (Lunsoul עושה voice-AI) מול B4 (אף אחד לא עושה voice שיחתי בעברית) — IVR מוקלט מול AI שיחתי? לבדוק ב-Verification.
- **הזדמנות פתוחה:** B2B-אולמות white-label (פחות צפוף) + "דיוק מנות מוכח".

### Environment
- Agent tool זמין → spawn research subagents per wave.
- WebSearch זמין.
- Git: branch `claude/quirky-hamilton-QiIHk`, push אחרי כל phase.
