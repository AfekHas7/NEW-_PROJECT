# PROGRESS — startup-3 (AuditPilot — AI-Native ISO audit-prep service)

**Project:** startup-3 — חברת שירות AI-Native שמחליפה את יועץ האיכות בהכנה למבדקי ISO (ישראל-first → גלובלי)
**Start date:** 2026-05-31
**Language:** Hebrew (עברית)
**Mode:** Full Mode, **Deep Research tier** (per founder request — apples-to-apples עם Planny + startup-2)
**Baselines for comparison:** Planny = 6.4/10 (CONDITIONAL GO) · startup-2/RSVP-AI = 4.3/10 (NO-GO).
ראה `planny/06-validation/scorecard.md` (טבלת ההשוואה כוללת עמודת "Startup 3" שתמולא בסוף).

- **Research Depth:** Deep (score: 8/9, override: user request "Deep research, apples-to-apples")

---

## Phase Checklist

- [x] **Phase 1: Intake** — `00-intake/brief.md` (delta round + carryover משני הקודמים)
- [ ] **Phase 2: Brainstorm** — `00-intake/brainstorm.md`
- [ ] **Phase 2.5: Research Depth** — Deep (נעול ע"י המייסד)
- [ ] **Phase 3: Market Research** (4 waves, 15 agents) → `01-discovery/`
  - [ ] Wave 1 (A1 market, A2 trends, A3 regulatory, A4 adjacent)
  - [ ] Wave 2 (B1 direct, B2 indirect, B3 GTM, B4 emerging)
  - [ ] Wave 3 (C1 voice, C2 demand, C3 audience, C4 pricing)
  - [ ] Wave 4 (D1 distribution, D2 geographic, D3 partnerships)
  - [ ] Synthesis: 5 deliverables
- [ ] **Phase 3.5a: Verification** → `01-discovery/verification-report.md`
- [ ] **Phase 3.5: Research Gate** → `01-discovery/research-gate.md`
- [ ] **Phase 4: Strategy** → `02-strategy/` (5 files)
- [ ] **Phase 5: Brand** → `03-brand/` (3 files)
- [ ] **Phase 6: Product** → `04-product/` (3 files)
- [ ] **Phase 7: Financial** → `05-financial/` (3 files)
- [ ] **Phase 8: Validation** → `06-validation/` (6 files + scorecard)
- [ ] **Planny comparison table filled** (Startup 3 column)
- [ ] **Final:** `README.md` + `action-plan-30-days.md` + Dashboard

---

## Session Notes / State

**2026-05-31:**
- Intake הושלם (delta round). אותו מייסד כמו Planny + startup-2.
- **הבדל מבני:** Planny = consumer mobile app; startup-2 = done-for-you event service (B2C/B2B); startup-3 = **AI-native B2B managed service** שמחליף יועץ מקצועי (knowledge work). ה-thesis = YC RFS "AI-Native Service Companies".
- **החלטות אינטייק:** ישראל-first→גלובלי · ISO 9001 beachhead · trigger = first-time wedge + surveillance/recert annuity (אני הכרעתי, המייסד העביר אליי) · אב כשותף-אקוויטי-מומחה.
- **FMF: Moderate-plus (~5-6 צפוי)** — domain expertise שאול מהאב (לא של המייסד), אבל אב=שותף אמיתי (≠ startup-2). Single point of dependency.

### עדיפויות מחקר (highest-risk first)
1. **קבילות רגולטורית (existential)** — האם מבדק/registrar מקבל הכנה AI-native? דרישת "יישום בפועל + records" מול "תיעוד". ISO/IEC 17021 impartiality.
2. **תחרות** — Vanta/Drata/Sprinto (27001) + Qualio/Greenlight Guru/ETQ (QMS 9001/13485) + יועצים מקומיים. מי AI-native, מה ה-whitespace.
3. **Unit economics** — עלות יועץ ISO 9001 בפועל (anchor) + כמה שעות פיקוח/לקוח (מנוף המומחה).
4. **גודל שוק** — # תעודות ISO 9001 בישראל + עולמי (ISO Survey), # הסמכות חדשות/חידושים, גודל שוק הייעוץ/compliance-automation.
5. **first-time vs recertification** — WTP, retention על מנוי, האנונה.

### Environment
- Agent tool זמין → spawn research subagents per wave (Deep = 15 agents).
- WebSearch זמין (להפעיל בתוך subagents).
- Git: branch `claude/funny-ritchie-HhI5u` (מוזג מ-`claude/quirky-hamilton-QiIHk`), push אחרי כל phase.
