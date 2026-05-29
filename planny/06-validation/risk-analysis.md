# Risk Analysis — Planny

**Phase:** Phase 8 — Validation (Risk Analysis)
**Project:** startup-validation (Planny)
**Date:** 2026-05-28
**Confidence:** Medium-High — likelihood/impact מבוססים על Tier-1 evidence (RevenueCat, AppTweak, FTC, Apple/Google policy, Crunchbase) ו-3 קבצי Phase 3 raw + 5 synth. הסיכונים האישיים של המייסד (burnout, focus split על 3 startups, runway) מוערכים qualitatively מ-context שסיפק המייסד עצמו.

---

## תקציר Risk Profile

Planny נכנסת לחלון השקה של 11 ימים לפני WWDC עם פרופיל סיכון **מרוכז ב-3 צירים מתחזקים זה את זה**: (1) **סיכון פלטפורמה בינארי** — WWDC June 8 יכול לקבע (no announcement) או לשבור (ADHD-aware AI scheduler) את ה-positioning תוך 90 ימים; (2) **סיכון רטנציה קיומי** — D30 לקטגוריית productivity 4.1% ו-mental-health 3.3%, ו-Planny צריך 12-15% כדי שמתמטיקת ה-reinvestment תעבוד — אם הסף לא נחצה, הספירלה הופכת שלילית תוך 6-9 חודשים; (3) **סיכון מייסד מורכב** — סולו, ADHD, traveling ל-US בעוד חודש, ללא משכורת 6 חודשים, ועם 2 startups נוספים שמתחרים על תשומת לב. נסיעת ה-US מוסיפה שכבת operational stress בדיוק בשבועות 3-4 של pre-launch.

הסיכונים האלה אינם בלתי תלויים — **WWDC commoditization → CAC inflation → רטנציה מוסטרת → reinvestment fails → burnout מואץ → focus shift ל-startups האחרים**. זהו cascade של 5 צעדים שיכול לקרות תוך 90 ימים אם 2-3 dominoes נופלות במקביל. ברקע יושבת שכבה רגולטורית (MHMDA + FTC pixel exposure) שהיא low-likelihood-high-impact קלאסי — לא ייתפס תחתון בלי enforcement, אבל יחיד enforcement = business-ending.

**איפה מתחילים לטפל:** מקדימים את WWDC contingency (3 גרסאות launch מוכנות עד 7 ביוני), חוסמים את ה-pixel exposure (אסור Meta/TikTok pixels על דפי ADHD לפני יום 1), מקצים founder-self-check שבועי כדי לזהות burnout/pivot signals מוקדם, מוודאים שה-90% UI claim מאומת בעצם (audit פנימי בשבוע הזה), ובונים retention design ל-v1 (לא v1.1) כי זה המשתנה היחיד שמעל לכל הסיכונים האחרים.

---

## Risk Matrix (Likelihood × Impact)

### Methodology
- **Likelihood:** High (>60% chance), Medium (20-60%), Low (<20%)
- **Impact:** Critical (business fails/pivots), Major (significant delay/revenue loss), Moderate (manageable), Minor (inconvenience)
- **Priority Quadrants:**
  1. High likelihood + Critical/Major → **IMMEDIATE** address (pre-launch mitigation שמשנה את ה-launch plan)
  2. Low likelihood + Critical → Monitor + contingency plan (pre-written response, kill switch)
  3. High likelihood + Minor → Accept + manage (operational discipline)
  4. Low likelihood + Minor → Acknowledge + move on (no resources committed)

### Visual Quadrant Snapshot

```
                              IMPACT
                Minor   Moderate   Major   Critical
            ┌────────┬──────────┬────────┬──────────┐
LIKELIHOOD  │        │ Cash lag │ Inflow │ Burnout  │ HIGH
            │        │ Tracy =  │ CPC    │ Pivot to │
   High     │        │   no    │ infl.  │  other 2 │
            │        │ ADDitude │        │          │
            ├────────┼──────────┼────────┼──────────┤
            │  Indy  │  TikTok  │  Tiimo │ WWDC     │ MED
            │  expand│  alg.    │  sync  │ D30<5%   │
   Medium   │        │  shift   │  Saner │  CAC     │
            │        │  Israel  │  90% UI│  Reinvest│
            │        │  defrral │  Trial │  fail    │
            ├────────┼──────────┼────────┼──────────┤
            │        │  EU/GDPR │ Recall │ FTC      │ LOW
            │        │  FDA SaMD│  ADHD  │ MHMDA    │
   Low      │  App   │  Gemini  │  wave  │ Google   │
            │  Store │  Spark   │  rev.  │ OAuth    │
            │  Health│          │        │ deny     │
            └────────┴──────────┴────────┴──────────┘
```

---

## All Identified Risks (Categorized)

### Market Risks

| Risk | Likelihood | Impact | Priority |
|------|-----------|--------|----------|
| Apple ships ADHD-aware AI scheduler at WWDC June 8 (Mayday Labs acquisition + 2yr dev cycle) | Medium (35%) | Critical | **High** |
| Apple ships generic horizontal AI scheduler at WWDC (Personal Context + Calendar AI) | Medium (55%) | Major | **High** |
| Google Gemini Spark prices down to $20 AI Pro + adds ADHD-aware features | Low (15%) | Major | Medium |
| ADHD social-media backlash ("TikTok diagnosis culture" critique resurgence) | Medium (25%) | Moderate | Medium |
| Late-diagnosed ADHD demographic wave peaks/reverses within 12-24 months | Low (10%) | Major | Low |
| Tiimo ships two-way Google/Apple Calendar sync before Planny (Nolt public request open) | Medium (35%) | Major | **High** |
| Saner.AI closes Series A and clones late-dx women positioning | Medium (40%) | Major | **High** |
| Indy by Shimmer expands free-tier features (planning, voice) aggressively | Medium (50%) | Moderate | Medium |
| Motion acquires ADHD brand (Tiimo/Numo) for consumer re-entry | Low (15%) | Critical | Medium |
| Reclaim+Dropbox launches mobile + ADHD framing | Low (12%) | Major | Low |
| US discretionary subscription contraction (economy downturn 2026-27) | Low (20%) | Major | Medium |
| Status-quo inertia (Apple Reminders + paper) beats all paid apps for cold users | High (65%) | Moderate | Medium |

### Product Risks

| Risk | Likelihood | Impact | Priority |
|------|-----------|--------|----------|
| Voice brain-dump UX doesn't deliver "Aha" (>30% drop-off in onboarding) | Medium (40%) | Critical | **High** |
| Google OAuth review rejected or delayed >8 weeks | Low (15%) | Critical | Medium |
| LLM API cost runaway from heavy users (>$0.50/user/mo at scale) | Medium (30%) | Major | Medium |
| iOS Speech Recognition accuracy too low for ADHD speech patterns (rambling, restart) | Medium (30%) | Major | Medium |
| Apple Calendar EventKit limitations break two-way sync UX | Low (15%) | Moderate | Low |
| App Store rejection for medical-claim copy drift | Low (10%) | Major | Medium |
| Google Play Jan 2026 health-disclaimer non-compliance triggers update rejection | Low (12%) | Major | Medium |
| 90% UI claim is overstated; actual completion <60% when audited | Medium (40%) | Major | **High** |
| Onboarding setup >90 sec → ADHD users abandon (well-documented pattern) | Medium (40%) | Major | **High** |
| Sub-90-second Aha moment requires 3+ engineering weeks not budgeted | Medium (35%) | Major | Medium |

### Business Risks

| Risk | Likelihood | Impact | Priority |
|------|-----------|--------|----------|
| Day-30 retention <5% (below mental-health benchmark 3.3% but above productivity 4.1%) | Medium (40%) | Critical | **High** |
| Trial-to-paid conversion <15% (vs 25% base) | Medium (35%) | Major | **High** |
| Refund rate >5% (Inflow precedent; model-breaking at 8%+) | Medium (25%) | Major | Medium |
| CAC inflation from Inflow/Saner/Indy paid spend | High (75%) | Major | **High** |
| Founder DM/support load unsustainable at >500 paying users | High (70%) | Moderate | Medium |
| Refund processing delays (Apple/Google 30-45 days) damage brand promise | Medium (30%) | Moderate | Medium |
| Apple Small Business Program eligibility denied/delayed | Low (10%) | Major | Medium |
| Tier mix skews monthly >65% (low LTV, low cash upfront) | Medium (30%) | Moderate | Low |
| 6-month tier cannibalizes annual (>40% of mix) | Medium (35%) | Moderate | Low |

### Team Risks

| Risk | Likelihood | Impact | Priority |
|------|-----------|--------|----------|
| Founder burnout (solo + ADHD + founder voice = brand voice + 30hr-week ceiling violated) | High (70%) | Critical | **High** |
| Founder shifts focus to other 2 startups he's comparing | High (60%) | Critical | **High** |
| US travel in 1 month disrupts launch readiness (jetlag, timezone, productivity) | High (65%) | Moderate | **High** |
| Founder personal/family runway exhausted before Month 7 (no-salary period) | Medium (30%) | Critical | **High** |
| Single-point-of-failure on founder ADHD disclosure (privacy/personal-brand risk) | Low (10%) | Major | Low |
| Founder medical/health emergency during launch window | Low (10%) | Critical | Medium |
| Israeli reservist call-up disrupts launch or operations | Low (15%) | Major | Medium |
| Founder unable to sustain TikTok/content cadence (3-5 pieces/week per channels.md) | Medium (50%) | Major | **High** |
| Founder lacks DM/community-management discipline at scale (>500 users) | High (60%) | Moderate | Medium |

### Financial Risks

| Risk | Likelihood | Impact | Priority |
|------|-----------|--------|----------|
| Reinvestment compounding fails (negative D30 retention → flat or negative cash flow growth) | Medium (40%) | Critical | **High** |
| Cash flow lag (Apple/Google 30-45 day hold + 30-day refund = 60-day gap) creates Month 2-3 pinch | High (75%) | Moderate | Medium |
| Inflow ad spend prices Planny out of all paid channels (Meta + TikTok + ASA broad) | High (80%) | Major | **High** |
| Saner.AI Series A funds price wars / feature parity race | Medium (35%) | Major | **High** |
| LLM API costs spike to $0.50/user/mo at scale (heavy power users) | Medium (30%) | Moderate | Medium |
| Apple Search Ads CPC inflation by competitors (productivity +90% YoY 2025) | High (70%) | Moderate | Medium |
| $1,500 seed exhausted before first $1K MRR (Month 2-3 risk) | Low (20%) | Major | Medium |
| Y1 cumulative cash insufficient to fund partial founder salary in M8 | Medium (40%) | Major | Medium |

### Regulatory Risks

| Risk | Likelihood | Impact | Priority |
|------|-----------|--------|----------|
| FTC enforcement on ad pixels for ADHD-targeted pages (BetterHelp/Cerebral/GoodRx pattern, $7M+ settlements) | Low (12%) | Critical | **High** |
| Washington MHMDA private right of action ($7.5K-$25K/violation, plaintiffs' firms active) | Low (15%) | Critical | **High** |
| App Store category re-classification by Apple (Productivity → Health) post-March 2026 rule | Low (10%) | Major | Low |
| Israel Amendment 13 compliance triggered at 10K Israeli users (DPO mandatory, ISS handling) | Medium (40% if Israel launches Y2) | Major | Medium (deferred) |
| FDA SaMD inquiry on marketing claims drift ("treats", "improves focus") | Low (10%) | Major | Medium |
| GDPR Article 9 exposure from EU users without explicit consent | Medium (30%) | Moderate | Medium |
| HBNR breach-notification failure ($51,744/violation per affected user) | Low (8%) | Critical | Medium |
| CA/NY/CO auto-renewal law violation (click-to-cancel, single retention offer) | Low (15%) | Moderate | Low |
| HIPAA Business Associate trigger from B2B2C coach/clinic partnership | Low (10%) | Major | Low |

### Distribution & Channel Risks

| Risk | Likelihood | Impact | Priority |
|------|-----------|--------|----------|
| Tracy Otsuka declines or rack rate exceeds $1,500 budget | Medium (50%) | Major | Medium |
| r/ADHDWomen mods ban any founder promotion (700K, zero competitor presence rule strict) | High (60%) | Moderate | Medium |
| TikTok algorithm change reduces ADHD content reach | Medium (40%) | Moderate | Medium |
| ADDitude editorial doesn't reply to pitch (8-16 week decision window) | High (70%) | Moderate | Low |
| Apple Search Ads CPC inflation makes long-tail unviable | Medium (50%) | Moderate | Medium |
| ADHD Awareness Month (Oct 2026) featuring slot lost to Tiimo / Inflow | Medium (55%) | Moderate | Low |
| Focusmate partnership outreach goes nowhere (Taylor Jacobson no response) | High (60%) | Minor | Low |
| 30 ADHD micro-creators don't post despite gifted subs (<30% conversion) | Medium (50%) | Moderate | Medium |
| Kristen Carder fallback also declines | Low (25%) | Major | Medium |

---

## HIGH Priority Risks — Deep Dive + Mitigation

### Risk 1: Apple Ships ADHD-Aware AI Scheduler at WWDC June 8 (Likelihood: Medium 35%, Impact: Critical)

**Evidence base:**
- Apple acquired Mayday Labs April 2024; sunset May 2024. Mayday tech: "AI-Schedule Tasks" + "Ideal Time Scheduling Engine" = core Planny feature set, already 2+ years in Apple development
- WWDC June 8, 2026 keynote: Siri 2.0 overhaul + Personal Context (private on-device knowledge graph) + Calendar app gets Apple Intelligence
- Apple's iPhone install base = Planny beachhead (US women 25-40 are iPhone-heavy)
- Counter-evidence: Apple delayed Personalized Siri March 2025 — credibility deficit on AI delivery

**Detection:**
- Watch WWDC keynote live June 8, 10am PT (war-room session)
- Filter for: "calendar AI", "Siri planning", "intelligent scheduling", "executive function", "neurodivergent", explicit ADHD mentions
- Monitor MacRumors, 9to5Mac, AppleInsider rumor cycle May 30 – June 7

**Mitigation:**
- **Pre-written 3 launch versions ready by June 5** (per go-to-market.md):
  - Version A (no announcement / Apple silent on ADHD) → proceed as planned, "Apple won't build this for us specifically"
  - Version B (generic horizontal scheduler) → reposition as "the ADHD layer on top of Apple Intelligence", emphasize voice brain-dump + partner mode
  - Version C (ADHD-aware Apple scheduler) → 7-day pause, evaluate pivot to AuDHD/couples vertical OR ADHD coaching layer; founder + advisor decision
- War-room June 8: founder watches keynote live, drafts response within 24 hours, locks version by June 15
- Pre-write press release for each scenario; pre-record 3 TikToks
- "Use Apple Intelligence as infrastructure" — EventKit, Shortcuts, on-device LLM. Position Planny as complement, not competitor.

**Early Warning Signals:**
- May 30+: Apple Intelligence rumor density spikes on MacRumors / 9to5Mac
- Apple developer beta releases hinting at new EventKit / Calendar APIs
- Apple PR pre-briefings to NYT / WSJ / Bloomberg about WWDC Calendar features
- Conference-room leaks via Bloomberg Mark Gurman (he correctly predicted Mayday integration)

---

### Risk 2: Day-30 Retention <5% (Likelihood: Medium 40%, Impact: Critical)

**Evidence base:**
- Productivity category D30: 4.1% (Amraandelma 2025)
- Mental-health category D30: 3.3% (HCPLive, Wallace PhD)
- Best-in-class evidence-based health apps: 16% D30
- Planny model assumes 12% (base) / 15% (target) — between mental-health floor and best-in-class
- ADHD audience structural penalty: 31.6% lose-interest abandonment (per research-gate.md)
- Reinvestment math breaks below 8% D30 — model enters death spiral

**Detection:**
- TestFlight beta cohort analysis (D7 as leading indicator: D7 <25% → D30 will be <5%)
- Voice brain-dump completion rate (proxy for Aha): <50% = retention crisis signal
- Push notification opt-in rate <40% = engagement crisis signal
- Day-3 active-use rate <60% = abandonment signal

**Mitigation:**
- Ship retention design **in v1, not v1.1**: gentle re-engagement, no streaks (avoid ADHD shame trigger), no red badges
- Energy-aware mode in v1 (not deferred) — capacity-aware planning per Sunsama playbook adapted for ADHD
- Weekly review prompt — Sunday voice check-in (3-question format, <60 sec)
- Founder personal DM to inactive users at D7 and D14 — "what got in the way?" — qualitative signal + retention nudge
- Proactive refund to honor "no shame" brand if user signals dissatisfaction
- **Kill switch:** if D30 <6% by Month 3 cohort, halt paid acquisition, audit Aha moment, consider pivot

**Early Warning Signals:**
- TestFlight beta D7 <25%
- Voice brain-dump completion <50% in onboarding funnel
- Founder DM responses contain "I forgot about it" / "I tried but…" pattern in >30% of inactives
- Reviews <4.0 with "didn't stick" / "too much friction" / "lost interest" themes

---

### Risk 3: Tiimo Ships Two-Way Sync First (Likelihood: Medium 35%, Impact: Major)

**Evidence base:**
- Tiimo's #1 technical gap = one-way calendar sync (Apple/Google/Outlook reads only, no write-back)
- Feature request publicly logged at **tiimo.nolt.io** — both Apple and Google two-way sync are top-voted
- Tiimo is funded ($4.8M raised, pre-Series A), has 25-30 engineers, just won Apple iPhone App of the Year 2025 (resources + attention)
- If Tiimo ships first, Planny's primary technical wedge closes — must pivot to voice/partner/refund moats

**Detection:**
- Weekly check of tiimo.nolt.io status field (planned / in-progress / shipped)
- Weekly Tiimo changelog scrape
- LinkedIn search for new Tiimo hires in iOS Calendar / EventKit / Google Calendar API expertise
- Tiimo Twitter/blog/podcast appearances mentioning "2026 roadmap"

**Mitigation:**
- **Ship Planny Google OAuth in 3-4 weeks** (per research-gate.md condition #3)
- Submit Google OAuth review Day 1 (before all code complete — review takes 3-4 weeks)
- Build Apple EventKit two-way as parallel track (no Apple review for EventKit, only App Store review)
- If Tiimo ships first within 90 days post-launch → pivot wedge to: voice brain-dump <90s + partner mode + 30-day refund promise + late-dx women persona narrow
- Manual `.ics` import as fallback if OAuth delayed

**Early Warning Signals:**
- Tiimo Nolt status changes from "planned" to "in development"
- Tiimo blog/Twitter "2026 roadmap" content mentions Calendar
- Tiimo Glassdoor / LinkedIn hiring iOS Calendar engineers
- Tiimo product update emails (beta tester signals)

---

### Risk 4: Saner.AI Raises Series A (Likelihood: Medium 40%, Impact: Major)

**Evidence base:**
- Saner.AI = Techstars + Google Accelerator + Value Create Ventures (~$120K disclosed Crunchbase, likely undercount)
- #1 ranked in most "best ADHD app 2026" lists (Morgen, Rivva, OnePageCRM)
- Product Hunt launch: 389 upvotes / 682 comments — strongest ADHD app launch ever
- Broader scope ("Jarvis for ADHD") could absorb Planny's wedge if Series A funded
- Saner founders not publicly ADHD — Planny's founder-ADHD positioning is defensible

**Detection:**
- Crunchbase weekly check (Saner.AI funding rounds)
- Saner.AI team LinkedIn growth signal (engineer/marketer hiring spike)
- Saner.AI guest blog posts on big VC blogs (a16z, First Round, Founder Collective)
- Pricing page changes (if pricing becomes public + aggressive = Series A signal)

**Mitigation:**
- **Lock founder/ADHD positioning** as identity moat (Saner.AI founders not publicly ADHD)
- Build community moat in 90 days: r/ADHDWomen presence (founder-led, NOT promo), 30 micro-creator relationships, Discord ADHD communities embedded
- Out-position rather than out-build: late-dx women narrow vs Saner's knowledge-worker broad
- Race to ship persona-specific features Saner won't build: partner mode, sessions-gated refund, weekly voice check-in
- Tracy Otsuka exclusive (Saner can't take her if Planny locks first)

**Early Warning Signals:**
- Saner.AI hiring spike on LinkedIn (>3 new hires/month)
- Saner.AI guest blog posts on big VC sites
- Saner.AI launches affiliate / creator program
- Saner.AI pricing becomes public

---

### Risk 5: Founder Burnout (Likelihood: High 70%, Impact: Critical)

**Evidence base:**
- Solo founder, ADHD, comparing 3 startups simultaneously
- Founder voice = brand voice (TikTok, podcast intros, r/ADHDWomen presence) — no proxy
- 30 hrs/week content + 30 hrs/week build + DM support + admin = unsustainable
- US travel in 1 month adds disruption
- No salary 6 months = personal financial stress amplifier
- ADHD lose-interest pattern (31.6% baseline) applies to the founder himself

**Detection (founder self-report + observable):**
- Weekly self-check: "Am I still excited about Planny?" (1-10 scale)
- Content posting velocity drop (TikTok posts/week)
- DM response time stretch (>48 hrs)
- Sleep / exercise / medication adherence (founder ADHD baseline)
- Founder partner/family flags ("you seem off")

**Mitigation:**
- **Hard cap 30 hrs/week build** — written commitment, calendared
- **1 full day off/week** non-negotiable (Sunday)
- **Contractor hire trigger:** $5K MRR = fractional iOS contractor (one weekend/month feature ship)
- **Personal ADHD stack:** medication adherence, therapy weekly, accountability buddy outside Planny
- **Asynchronous founder-DM SLA:** 48-hour response window (set expectations), batch reply 2x/day
- **Pre-WWDC US travel:** front-load critical work into May, set travel as "soft" weeks 3-4 not "hard"
- **Sabbatical clause:** if burnout signals trigger 2 weeks in a row, mandatory 7-day step-back

**Early Warning Signals:**
- Missed 3+ days of content posting in a row
- DM response time >48 hours sustained
- Founder posts about feeling overwhelmed / "I need a break"
- Skipped therapy / medication 3+ times in a month
- Partner / family expresses concern unprompted
- Founder reaches for other 2 startups as "easier" escape

---

### Risk 6: Founder Pivots to Other 2 Startups (Likelihood: High 60%, Impact: Critical)

**Evidence base:**
- Founder explicitly compared 3 startups against same validation framework (per project context)
- Single-bet bias is unfair; founder is doing right thing methodologically, but it creates pivot temptation
- ADHD founders have higher pivot rate (lose-interest pattern)
- If Planny fails to show clear traction by Day 14 post-launch, the other 2 startups will look more attractive

**Detection:**
- Founder time allocation tracking (hours/week on Planny vs other 2)
- Founder asks more questions about other 2 startups than Planny
- Founder spending more research time on other 2 startups
- Founder mentions other 2 startups in casual conversation more frequently

**Mitigation:**
- **Apply same scorecard** to all 3 startups (apples-to-apples, deterministic comparison)
- **Set decision date:** by Day 14 post-launch (June 22 + 14 = July 6, 2026), founder commits to Planny for 90 days OR moves on — no halfway
- **90-day Planny commitment** if chosen: written, dated, signed (to self) — minimum 60 hrs/week Planny only, other startups deferred
- **Sunk-cost framing reframe:** "If I pivot to another startup, the Planny methodology + validation work isn't wasted — it applies"
- **Decision gate Month 3:** review traction; if MRR <$500 at M3, formal pivot evaluation
- **Decision gate Month 6:** review per pessimistic scenario; if <$1,000 MRR + <$1,500 cumulative cash, hard kill / pivot / bridge decision

**Early Warning Signals:**
- Founder asks more questions about other 2 startups than Planny in weekly check-ins
- Founder spends >5 hrs/week researching other 2 startups
- Founder uses "but my other idea…" phrasing in conversation
- Content posting for Planny drops without corresponding content for others = neither, just burnout
- Content posting for another startup ramps up = active pivot in progress

---

### Risk 7: US Travel in 1 Month Disrupts Launch Readiness (Likelihood: High 65%, Impact: Moderate)

**Evidence base:**
- Founder traveling to US in ~1 month (late June 2026)
- Launch window: June 22 – July 1 — overlaps directly with travel
- Jetlag + timezone shifts + meeting load reduce focus
- ADHD founder + new environment = adjustment cost
- TestFlight beta + bug fix cycle requires concentrated dev work

**Detection:**
- Travel calendar laid against launch calendar — overlap audit
- Founder energy/output tracking pre/post travel days
- Hotel/coworking setup adequacy (laptop, charger, internet, quiet space)

**Mitigation:**
- **Front-load critical work into May 28 – June 18** (3 weeks before travel)
- **Plan launch for AFTER travel returns** if travel >7 days (push to July 1-8 if needed)
- **Designate travel weeks as "soft" not "hard"** — DM response only, no major dev/launch decisions
- **Pre-write 14 days of TikTok content** before travel (schedule via Buffer / TikTok scheduler)
- **WWDC viewing:** if traveling June 8, ensure hotel TV / VPN / laptop ready
- **Quiet/focus space:** book Airbnb with desk, not just hotel room — ADHD founders need dedicated workspace
- **Time-zone buffer:** if East Coast travel, gain 7 hrs vs Israel — use for morning founder work block

**Early Warning Signals:**
- Travel dates extend or compress (US plan changes)
- Founder energy <6/10 during week 1 of travel
- Critical bugs surface post-departure with no remote contractor backup
- DM backlog >24 hours during travel

---

### Risk 8: 90% UI Claim Overstated (Likelihood: Medium 40%, Impact: Major)

**Evidence base:**
- Founder self-reports 90% UI done, voice + Google OAuth remaining
- Founders systematically overestimate completion (Hofstadter's law)
- "UI done" ≠ "production-ready" — bug fixes, edge cases, accessibility, App Store review iteration
- Voice + Google OAuth are non-trivial: Voice = speech recognition tuning + LLM prompt design; Google OAuth = 3-4 weeks + Google review

**Detection:**
- Audit F1-F10 (feature list) against current build within 1 week
- Demo each screen to non-founder observer — friction = incomplete
- TestFlight build with 5-10 testers — pre-beta sanity check

**Mitigation:**
- **This week: F1-F10 audit** — checklist with screens, states, edge cases
- If <70% actually done, **replan launch timeline** — push June 22 → July 1-8
- **Communicate honest timeline** to anyone waiting (waitlist, Tracy, beta testers)
- **De-scope ruthlessly:** ship voice + Google OAuth + sync; defer partner mode v1.1, energy-aware mode v1.2, Hebrew RTL Y2
- **Founder + 1 external reviewer** (friend / fellow founder) sanity-check completion claim

**Early Warning Signals:**
- Founder unable to demo specific screens from F1-F10 list on request
- "I haven't built X yet" appearing in conversation
- TestFlight build crashes or major UI bugs on first install
- Voice brain-dump >5 seconds latency or transcription accuracy <80%

---

### Risk 9: Voice Brain-Dump Aha Moment Fails (Likelihood: Medium 40%, Impact: Critical)

**Evidence base:**
- Voice brain-dump → AI weekly plan in 30-90 sec is **the** Aha moment for Planny
- If users don't get "this app gets me" reaction in first session, retention collapses
- iOS Speech Recognition has known issues with ADHD speech patterns (rambling, restart, mid-sentence pivots)
- LLM prompt design to convert "I have a chaotic week" → coherent weekly plan = non-trivial
- No competitor has solved this — both the opportunity AND the risk

**Detection:**
- TestFlight cohort completion of voice brain-dump (target >70% complete in onboarding)
- Time-to-first-plan metric (target <90 sec from launch)
- Founder-DM qualitative: did first session feel magical?
- Post-onboarding NPS: "Would you recommend Planny?" target >40

**Mitigation:**
- **Prototype voice flow in week 1 of TestFlight** — get 10-20 ADHD women voicing real brain-dumps
- **Iterate prompts weekly** based on transcription failures
- **Fallback to text input** in onboarding if speech fails — don't force voice (better UX than broken voice)
- **Pre-warm with prompts:** "Tell me what's on your plate this week. Just talk, I'll figure it out." (lowers ADHD activation energy)
- **Constraint design:** time-box voice to 60-90 sec max (prevents ADHD ramble paralysis)
- **Show plan within 5 sec of voice end** — instant gratification = ADHD-friendly

**Early Warning Signals:**
- TestFlight users abandon voice flow >50% rate
- Transcription accuracy <80% on beta cohort
- LLM output requires >2 user edits before usable
- Beta testers describe voice flow as "frustrating" / "didn't get me"

---

### Risk 10: Inflow Ad Spend Saturation Locks Planny Out of Paid (Likelihood: High 80%, Impact: Major)

**Evidence base:**
- Inflow: $11M Series A, $11M+ spent on Meta + TikTok ADHD-niche targeting (TechCrunch, Octopus Ventures)
- Meta CAC for ADHD audience iOS: $30-80 (vs $17-22 sustainable ceiling)
- TikTok @inflow: 296.6K followers, 16.2M likes — dominant
- Apple Search Ads productivity +90% YoY CPI 2025 (AppTweak) — compounding inflation
- $1,500 budget = ~40-100 users via paid (per research-gate.md)

**Detection:**
- Apple Search Ads CPI/CPA dashboard weekly
- Meta / TikTok CPM trends on ADHD-keyword targeting (if tested at all)
- Inflow announces fundraise (rare leak — would compound the problem)
- Inflow expands creator program signal

**Mitigation:**
- **Skip Meta and TikTok paid entirely** (per GTM plan)
- **Niche ASA only:** long-tail ("late diagnosed ADHD planner", "ADHD weekly planner for women") not "ADHD"
- **Defensive brand ASA only on "Planny"** (competitors will bid)
- **Lean 80% organic, 20% paid maximum** (Tracy Otsuka + micro-creators + r/ADHDWomen + TikTok founder-led)
- **CAC kill switch:** pull paid spend if blended CAC >$25 for 2 consecutive weeks

**Early Warning Signals:**
- Apple Search Ads CPC >$5 on long-tail keywords (currently $2.84-4.50)
- Inflow announces fundraise (TechCrunch, Crunchbase weekly check)
- Saner.AI Series A announced (compounds the problem)
- Indy by Shimmer launches paid acquisition

---

### Risk 11: Reinvestment Compounding Fails (Likelihood: Medium 40%, Impact: Critical)

**Evidence base:**
- Reinvestment math assumes positive D30 retention (>8%) and positive trial-to-paid (>15%)
- Cash flow lag: Apple/Google hold 30-45 days + refund window 30 days = 60-day gap
- If first 50-100 paying users don't materialize by Month 3, runway tightens fast
- Hidden risk: every $1 in acquisition must return >$1 in 6-month LTV — if retention fails, math inverts

**Detection:**
- MoM net cash flow growth (target >15% MoM in Months 3-12)
- Marketing spend efficiency: $/paying-user week-over-week
- Cohort LTV at D60, D90 (against $17-22 CAC ceiling)
- Reinvestment pool sufficient to fund next month's marketing?

**Mitigation:**
- **Strict CAC ceiling: $20 max** — kill any channel that exceeds for 2 weeks
- **Double down on organic if paid fails** — TikTok + Reddit + Pinterest + r/ADHDWomen
- **Founder personal savings buffer:** ensure 3-6 months living costs in reserve before launch
- **Conservative tier mix planning:** assume 50% monthly (lower LTV, lower cash upfront) for first 60 days
- **Pessimistic scenario decision gate Month 6:** if <$500 net MRR + cumulative <-$1,000, pivot / bridge / sunset
- **Don't over-commit marketing on Day 1-30 bookings** — treat all cash <Day 60 as conditional

**Early Warning Signals:**
- Month 2 net cash worse than Month 1
- Apple Search Ads CPI >$5
- Trial-to-paid conversion <15% in first 30-day cohort
- D7 retention <25% in TestFlight
- Founder personal runway forecasts <3 months remaining

---

### Risk 12: Founder Personal/Family Runway Exhausted (Likelihood: Medium 30%, Impact: Critical)

**Evidence base:**
- No salary 6 months = personal/family runway dependency
- $1,500 seed is project budget, not living costs
- Y1 cumulative cash base case $18K — insufficient to retroactively cover 6 months salary
- Per business-model.md: "if family/personal runway exhausted before month 6, model collapses regardless of MRR trajectory"

**Detection:**
- Monthly personal runway forecast (founder self-report)
- Family stress signals (partner conversations, kids' impact)
- Founder medication / therapy continuity (covered by insurance? out of pocket?)

**Mitigation:**
- **Pre-launch runway audit:** confirm 7-14 months living costs in personal savings BEFORE June 22
- **Spouse / partner alignment:** explicit conversation about 6-month no-salary commitment + decision date
- **Plan B income:** identify 5-10 hr/week consulting / contracting backstop if runway gets tight
- **Decision gate Month 4:** if personal runway <3 months remaining, trigger founder salary discussion early ($1K-1.5K/mo) even if pre-$5K MRR
- **Bridge round optionality:** identify 2-3 friends/family who could write $5-10K bridge check if needed (NOT counted on, just contingency)

**Early Warning Signals:**
- Founder personal credit card balance climbing
- Family stress signals (partner conversations about money)
- Founder skipping medication / therapy due to cost
- Founder declining social events for cost reasons

---

### Risk 13: CAC Inflation from Combined Competitor Spend (Likelihood: High 75%, Impact: Major)

**Evidence base:**
- Inflow ($11M) + Saner.AI (Series A pending) + Indy (Shimmer $3.5M) = combined pressure on ADHD-niche keyword auctions
- Apple Search Ads productivity CPI +90% YoY 2025 — already inflating
- Tiimo App of the Year halo drives organic search away from new entrants
- Multiple competitor effect: even if Planny avoids head-to-head, generic "ADHD planner" SEO/SEM gets pricier

**Detection:**
- Apple Search Ads weekly CPI/CPA dashboard
- Meta / TikTok CPM trends (if any test spend)
- Organic SEO ranking position for target long-tail keywords (Ahrefs / Semrush)
- Competitor ASA bid signals (visible in some keyword tools)

**Mitigation:**
- **Skip all paid channels except niche ASA long-tail + defensive brand "Planny"**
- **Lean organic-heavy:** Tracy Otsuka, micro-creators, founder TikTok, r/ADHDWomen, Pinterest
- **CAC ceiling enforced weekly:** $20 blended, $5 organic-only target
- **Out-positioning** rather than out-spending — late-dx women narrow persona competitors don't own
- **Long-tail SEO compounding** — 90-180 days to rank but free

**Early Warning Signals:**
- Inflow announces fundraise
- Saner.AI announces fundraise
- Apple Search Ads CPI >$5 on long-tail
- Generic "ADHD planner" CPC >$8 (competitor war signal)

---

### Risk 14: FTC/MHMDA Enforcement on Mental-Health Data Practices (Likelihood: Low 12-15%, Impact: Critical)

**Evidence base (Combined Risks 14a + 14b — treated together as "regulatory ad-pixel pattern"):**
- FTC enforcement pattern: BetterHelp ($7.8M, 2023), Cerebral ($7M + $3.6M DOJ, 2024), GoodRx ($1.5M HBNR, 2023)
- All FTC actions = ad pixel sharing of mental-health-related data with Meta/TikTok/Google
- WA MHMDA private right of action = $7,500/violation, treble damages up to $25K/violation
- Plaintiffs' firms actively trolling for MHMDA violations
- Single enforcement action = $1-7M settlement = business-ending for bootstrap

**Detection:**
- Internal audit: every page that mentions "ADHD" — check for Meta Pixel, TikTok Pixel, Google Tag
- Marketing copy review monthly: no "treats", "improves focus", "clinically proven", "doctor-recommended"
- Privacy policy + Health Data Privacy Policy current and MHMDA-compliant
- Annual lawyer review (~$500-2,000)

**Mitigation:**
- **Zero third-party ad pixels on any ADHD-mentioning page** (default position per regulatory.md)
- **Server-side conversion API + hashed IDs + separate explicit consent** if attribution needed
- **Marketing Language Policy (1-page do/don't list)** signed by founder + any contractor/influencer
- **Separate Health Data Privacy Policy** at launch (not retrofit) per MHMDA requirement
- **Separate consent for collection AND sharing** — granular UX
- **Category: Productivity** (not Health & Fitness) on Apple + Google to avoid March 2026 medical device declaration
- **Lawyer-reviewed privacy templates** before launch ($500-2,000)
- **HBNR breach-response runbook** — 60-day clock pre-documented

**Early Warning Signals:**
- FTC announces new mental-health-app enforcement (BetterHelp / Cerebral pattern)
- WA MHMDA enforcement action against any consumer app
- Plaintiff's firm contacts Planny (cease-and-desist letter)
- Marketing copy drift detected in audit (any "treats" / "improves" language)
- New ad pixel added to landing page without consent UX

---

### Risk 15: Onboarding Setup >90 Seconds → ADHD Abandonment (Likelihood: Medium 40%, Impact: Major)

**Evidence base:**
- Per competitor-landscape.md: "Sub-90-second setup" is required for ADHD audience
- RevenueCat 2025: 84% of 3-day, 64% of 7-day cancellations happen Day 0-1
- ADHD activation energy is real — every extra friction step = exponential drop-off
- Tiimo setup overwhelm is documented #1 complaint — Planny must not repeat

**Detection:**
- Time-to-first-plan metric in onboarding funnel
- Drop-off rate per onboarding step
- TestFlight cohort completion rate (target >80% through onboarding)
- Qualitative: founder DM "how was setup?" to first 100 users

**Mitigation:**
- **One-tap calendar connect** (Apple EventKit one-tap, Google OAuth one-tap)
- **Auto-detect existing patterns** from calendar history — no manual data entry
- **Voice brain-dump first, account second** — Aha before friction
- **Account creation deferred** — let user experience plan first, sign up after (per voice-aha logic)
- **Sub-90-second target** measured weekly; if >90 sec, audit + cut steps
- **Skip / defer non-essential settings** — push to Settings menu, not onboarding flow

**Early Warning Signals:**
- TestFlight time-to-first-plan >120 sec
- Onboarding drop-off >40% at any single step
- "Too many setup screens" / "too much to set up" in reviews
- D1 active rate <50%

---

### Risk 16: Founder Unable to Sustain Content Cadence (Likelihood: Medium 50%, Impact: Major)

**Evidence base:**
- GTM plan requires 3-5 pieces of TikTok / Reddit / Pinterest content per week
- Per research-gate.md: "המייסד חייב להיות organic content creator"
- Solo founder + build + DM + admin + content = stretched
- ADHD founder + content cadence consistency = structural challenge
- Failed cadence = no distribution = no growth

**Detection:**
- Content output per week (TikTok, Reddit, Pinterest, blog) tracked weekly
- Engagement metrics: views, comments, follower growth
- Founder energy / interest in content (self-report weekly)

**Mitigation:**
- **Batch content creation** — 1 full day/week (e.g., Sunday) for 7-10 pieces of content
- **Content templates** — 5-10 repeatable formats (founder story, day-in-life, ADHD struggle, planner comparison, voice demo)
- **Scheduling tool** — Buffer / Later / TikTok scheduler — post automatically
- **Repurpose ruthlessly** — 1 TikTok → 1 Reddit post → 1 Pinterest pin → 1 blog snippet
- **Audience engagement, not content creation, is the unfair advantage** — spend 50% of "content time" replying to DMs / comments rather than creating new
- **Hire creator contractor at $5K MRR** — fractional content support

**Early Warning Signals:**
- Content output <3 pieces/week for 2 consecutive weeks
- Founder describes content as "draining" / "I can't anymore"
- Engagement metrics flat-lining (no new followers, low comments)
- Founder skips Sunday content batch day

---

### Risk 17: Trial-to-Paid Conversion <15% (Likelihood: Medium 35%, Impact: Major)

**Evidence base:**
- RevenueCat / Adapty opt-in CC trial benchmark: 18-25%
- Planny model assumes 25% (high end of benchmark)
- If conversion drops to 15%, Y1 ARR drops 40%
- Trial structure + paywall design = single highest-leverage decision in business model

**Detection:**
- Trial-start → paid conversion rate weekly (D14 trial endpoint)
- Paywall view → trial-start rate (engagement signal)
- Trial cancellation reasons (qualitative)

**Mitigation:**
- **Paywall A/B testing from Month 1** — test copy, pricing emphasis, badge ("Most Popular"), social proof
- **Reminder cadence:** D11, D13, D14 push + email — value reminders, not hard sells
- **In-trial Aha reinforcement:** weekly review prompt D7, D14 to drive engagement during trial
- **Founder DM at D10 to non-converters:** "how's the trial going? anything blocking?"
- **Pricing psychology:** annual pre-selected, badged "Save 50% + 14 days free", 6mo as decoy
- **Kill switch:** if conversion <18% by M3, redesign paywall before scaling acquisition

**Early Warning Signals:**
- Paywall view rate <50% (low engagement)
- Trial-start rate <60% of paywall views
- D7 trial active <50% (users disengaging mid-trial)
- Trial cancellation reasons cluster on "too expensive" / "didn't see value"

---

## Medium Priority Risks (Monitor + Plan)

### Indy by Shimmer expands free tier (Med 50%, Moderate)
Free competitor with $3.5M parent funding. Mitigation: emphasize Planny depth (two-way sync, voice, partner mode) that funnel-app won't build. Position: "Indy is free because they're selling coaching upsell; Planny isn't."

### Cash flow lag Month 2-3 pinch (High 75%, Moderate)
60-day Apple/Google hold + refund window = working capital gap. Mitigation: treat all cash <Day 60 as conditional; conservative marketing spend Months 1-3; founder personal buffer 3+ months.

### Apple Search Ads CPC inflation (High 70%, Moderate)
Productivity +90% YoY 2025. Mitigation: long-tail only, defensive brand only, $20 CAC ceiling enforced.

### r/ADHDWomen mods ban promotion (High 60%, Moderate)
700K members, strict anti-promo rules. Mitigation: founder-led organic, 4-6 week relationship build before any pitch, modmail AMA program request, NEVER post link.

### TikTok algorithm change (Med 40%, Moderate)
Diversification across platforms (Pinterest, Reddit, YouTube long-form) reduces dependency.

### LLM API cost runaway (Med 30%, Major)
Rate-limiting on free chat, tier-up to GPT-4o for power users ($14.99 add-on), on-device inference for iOS 27+ if WWDC enables.

### ASA conversion below benchmark (Med 30%, Moderate)
Defensive only ($200-500/mo cap), kill if CPA >$40.

### Refund rate >5% (Med 25%, Major)
Sessions-gated refund (<10 sessions/30d) enforced from Day 1. Intervention if >5% by M3.

### 30 micro-creators don't post despite gifts (Med 50%, Moderate)
Mitigation: 30% lifetime affiliate (cash incentive beyond gift), screen for actually-active planners, follow up at week 2 with content templates.

### iOS Speech Recognition accuracy issues (Med 30%, Major)
Text fallback always available; transcription tuning per ADHD speech patterns; LLM cleanup of imperfect transcription.

### Apple SBP eligibility denied/delayed (Low 10%, Major)
Apply Day 1; if delayed, Y1 economics moderately worse but viable; Y2 ARR -21% if denied entirely.

### Israel Amendment 13 (Med 40% if launch, Major, deferred)
Defer Israeli launch to Y2 M6 per business-model.md; fractional DPO budget $8-25K/yr when triggered.

### GDPR Article 9 if EU users (Med 30%, Moderate)
Geo-block EU at launch OR explicit consent UX; defer EU formal launch to Series A.

### Y1 cash insufficient for partial founder salary M8 (Med 40%, Major)
$18K Y1 cash (base) ÷ 5 months = $3.6K/mo max — partial salary OR continued reinvestment OR raise decision.

### Founder family/medical/reservist disruption (Low 10-15%, Critical/Major)
Reservist insurance check; family emergency fund separate from Planny; founder partner can cover 1-2 weeks emergency.

---

## Risk Mitigation Calendar

| Week | Date | Action |
|------|------|--------|
| **Week 0 (now)** | May 28 – Jun 3 | Apple SBP application; legal templates ordered ($500-2K); F1-F10 UI audit; pre-launch personal runway audit; spouse alignment conversation; Marketing Language Policy drafted |
| **Week 1** | Jun 4 – Jun 10 | Waitlist landing live; outreach Tracy Otsuka + Kristen Carder + 80 micro-creators; pre-write 3 WWDC launch versions; **WWDC viewing Jun 8 (war-room)**; lock launch version by Jun 15 |
| **Week 2** | Jun 11 – Jun 17 | Google OAuth submission to Google review; TestFlight beta build live; 10-20 ADHD women voice-flow testing |
| **Week 3** | Jun 18 – Jun 24 | TestFlight beta cohort 1 (50-100 testers); pricing A/B test setup; D7 retention measurement starts; **launch June 22 (or push to Jul 1 if not ready)** |
| **Week 4** | Jun 25 – Jul 1 | Launch monitor: refund rate, Aha completion, CAC; founder DM to first 100 users; content cadence check |
| **Month 2** | Jul 2026 | Tracy Otsuka episode aim; D7 cohort 1 measurement; first reinvestment pool flow |
| **Month 3** | Aug 2026 | D30 cohort 1 measurement (the critical signal); Apple SBP approval window; cash flow break-even (base); **decision: continue or intervene on retention** |
| **Month 4** | Sep 2026 | Refund/retention re-baseline; pricing A/B winner deployed; Discord launch prep if $2K MRR |
| **Month 6** | Nov 2026 | **Pessimistic decision gate** — if <$500 MRR + cumulative <-$1,000 → pivot/bridge/sunset; Discord community launch (if $2K MRR base) |
| **Month 8** | Jan 2027 | Founder salary decision at $5K MRR threshold |
| **Month 12** | May 2027 | Y1 review → Y2 plan (Android, Hebrew RTL, raise decision); decision gate: continue / pivot / seed round |

---

## Founder Self-Check Questions

### Weekly check-in (every Sunday, 15 minutes, written)
1. **Am I still excited about Planny?** (1-10 scale; <6 for 2 weeks = burnout signal)
2. **Am I tempted to pivot to my other 2 startups?** (yes / no / "kinda" — track frequency)
3. **Has any data invalidated my core assumptions this week?** (honesty signal — voice Aha, D7 retention, CAC, conversion)
4. **Am I avoiding any hard conversation or decision?** (procrastination signal — what's been on the to-do list >7 days?)
5. **Content cadence: how many pieces did I publish this week?** (target 3-5)
6. **DM response time average?** (target <48 hrs)
7. **Sleep + medication + therapy this week?** (founder ADHD baseline)

### Monthly check-in (first of month, 1 hour, written)
1. **Is my personal runway still 3+ months ahead of MRR-supported salary?**
2. **Am I still building the wedge or scope-creeping?** (Persona narrow? Feature focus?)
3. **Are my metrics improving month-over-month?** (MRR, paying users, retention, CAC)
4. **What's the biggest risk for next month?** (forecast + mitigation)
5. **What would I tell another founder in my exact situation?** (perspective check)
6. **Am I closer to the 90-day commit-or-pivot decision?** (Day 14 / 30 / 60 / 90 gates)

### Quarterly check-in (every 90 days, half-day, written + advisor if available)
1. **Has the strategic landscape shifted?** (Apple, Saner, Tiimo, Indy, FTC)
2. **Should I reconsider seed round optionality?** (MRR + market signal)
3. **Is the brand voice still authentic to me?** (founder-led brands burn out)
4. **Am I building the company I want to run in 3 years?**

---

## Strategic Connections
- ראה `validation-playbook.md` (upcoming) ל-experiments שמורידים את ה-uncertainty על high-priority risks
- ראה `assumptions-tracker.md` (upcoming) ל-explicit assumptions והקשר ל-risks
- ראה `kill-criteria.md` (upcoming) ל-numerical thresholds ל-pivot/sunset decisions
- ראה `scorecard.md` (upcoming) ל-final assessment
- ראה `../02-strategy/business-model.md` ל-unit economics + scenarios שמהם נגזרו רוב הסיכונים הכלכליים
- ראה `../05-financial/projections.md` ל-scenarios (Conservative / Base / Optimistic / Pessimistic) + sensitivity analysis
- ראה `../01-discovery/research-gate.md` ל-3 התנאים הקריטיים (interviews, WWDC plan, Google OAuth)
- ראה `../01-discovery/competitor-landscape.md` ל-Tier 1 threats (Tiimo, Saner, Indy) + platform risk
- ראה `../01-discovery/raw/regulatory.md` ל-MHMDA + FTC + Apple/Google policy + FDA SaMD detail

---

## Sources

### Tier 1 (primary, recent, methodologically strong)
- RevenueCat State of Subscription Apps 2025 + 2026 — D30 retention benchmarks, trial conversion, annual cohort
- AppTweak 2026 — iOS CPI productivity NA $2.84 (+90% YoY)
- FTC enforcement orders — BetterHelp (2023), Cerebral (2024), GoodRx (2023)
- WA RCW 19.373 — MHMDA full text
- FDA — General Wellness Policy 2026 guidance, CDS Software 2026 guidance
- Apple Developer — App Review Guidelines, March 2026 health category rule
- Google Play Console — Health Apps policy Jan + Apr 2026
- Crunchbase — Inflow $11M Series A, Saner.AI Techstars + Google, Shimmer $3.5M
- SEC 8-K — Dropbox acquisition of Reclaim.ai $40.2M Aug 2024
- Library of Congress — Israel Amendment 13 effective Aug 14, 2025

### Tier 2 (specialized industry, useful)
- Adapty State of In-App Subscriptions 2025
- Amraandelma 2025 — productivity D30 4.1%
- HCPLive, Wallace PhD — mental health D30 3.3%
- IAPP, Cooley — MHMDA scope and enforcement signals
- Wilson Sonsini, Alston & Bird — FTC HBNR final rule analysis
- TechCrunch — Inflow Series A coverage
- Daring Fireball — Apple iPhone App of the Year 2025 (Tiimo)
- Bloomberg Mark Gurman — Apple Mayday Labs acquisition coverage
- MacRumors / 9to5Mac — WWDC 2026 preview
- SARAL case study — Sunsama 600+ creator ambassador model
- Trustpilot aggregation — Inflow billing reputation
- Tiimo Nolt feature request board — two-way sync public request

### Tier 3 (anecdotal, used with skepticism)
- Reddit r/ADHDWomen sentiment summaries
- Product Hunt — Saner.AI launch metrics
- Founder self-report on personal/family/runway context

---

## Flags

### Red Flags
1. **15 High-priority risks** for a pre-launch solo bootstrap startup is significant — concentration risk on founder + retention + WWDC + CAC
2. **Founder personal risks (burnout 70% + pivot to other 2 startups 60% + travel disruption 65%) are highest-probability cluster** — and they compound
3. **WWDC binary outcome (3-7 days from now) is largest external risk** — cascade risk if ADHD-aware Apple scheduler ships
4. **Retention D30 is existential variable** — model breaks below 6%, no precedent for ADHD audience exists publicly, first reliable signal is M3
5. **Combined competitor CAC inflation (Inflow + Saner + Indy) makes paid acquisition mathematically unviable** — organic-only is mandatory, not optional, and failure to execute organic = no growth
6. **FTC ad-pixel pattern (BetterHelp/Cerebral/GoodRx) is a single-action business-ending risk** — must enforce zero pixels on ADHD pages from Day 1

### Yellow Flags
1. **Several medium-priority risks compound:** Saner Series A + Tiimo two-way sync + Inflow CAC inflation all push CAC up simultaneously
2. **ADHD social-media saturation is slow-burn (3-5 year horizon)** — late-dx wave may peak in 2027-28
3. **Cash flow lag (60-day Apple/Google + refund window) is structural** — cannot be mitigated, only planned around
4. **Founder no-salary period (6 months) is operationally fragile** — any personal emergency invalidates the model
5. **Israel + Android in Y2 add execution complexity** — solo founder + iOS + Android + Hebrew RTL + partner mode v1.1 is aggressive

### Green Signals
1. **Founder ADHD = unique fit** — defensible identity moat that Saner / Tiimo / Motion / Inflow cannot replicate
2. **Late-dx women persona narrow + Tracy Otsuka unclaimed** = positioning + distribution opportunity in same package
3. **Two-way calendar sync wedge** still open if shipped within 30-45 days (per research-gate.md condition #3)
4. **Voice brain-dump Aha** is unique in category — no competitor unifies voice-capture → AI schedule → ADHD context → calendar write
5. **30-day no-questions refund + sessions-gated** = ethical wedge against Inflow billing reputation
6. **Founder-led organic distribution** is the right strategy for $1,500 budget — and founder has the raw material (ADHD authenticity)
