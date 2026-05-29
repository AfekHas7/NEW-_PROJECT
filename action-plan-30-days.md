# 30-Day Action Plan — Planny

**Start Date:** 2026-05-29 (Friday)
**End Date:** 2026-06-27 (Saturday — 5 days post-launch target)
**Founder:** Solo, ~25-30 hrs/week
**Pre-Commit:** Honor the 3 conditions from `research-gate.md` and `scorecard.md`

---

## Pre-Plan: Founder's 3 Conditions Acknowledged

Before reading this plan, the founder commits to:
1. **Defer launch to post-WWDC June 8** — with pre-written 3 launch versions ready
2. **Direct Google Calendar OAuth integration shipped in 3-4 weeks** — Day 1 application
3. **Lightweight signal collection replacing live interviews** (founder traveling to US in 1 month — Experiment 5 deferred to US trip)

---

## Week 1: Customer Discovery + Pre-Launch Foundation
**(2026-05-29 to 2026-06-04)**

### Day 1 (Fri 5/29) — Decision Day
- [ ] **Final go/no-go decision** vs Startup 2 + Startup 3 (apply same scorecard methodology to other 2 startups; pick highest)
- [ ] If Planny chosen: continue plan
- [ ] Read all 6 Phase 8 docs cover-to-cover (validation, risk, assumptions, kill criteria, experiment design, scorecard) — ~3 hours

### Day 2-3 (Sat-Sun 5/30-31) — Waitlist Foundation
- [ ] Build waitlist landing page (Carrd or Framer) — 3-4 hours
  - Use copy from `experiment-design.md` Experiment 1 template
  - Hero: "Voice your week in 60 seconds. By an ADHD adult, for ADHD adults."
  - Email capture only (no upfront payment)
  - Founder photo + ADHD disclosure
  - Sub-headline: "Coming late June. 30-day refund. No streaks."
- [ ] Domain registration: planny.app or planny.me ($12/yr)
- [ ] Set up ConvertKit / Mailchimp free tier for emails
- [ ] Test mobile responsiveness

### Day 4 (Mon 6/1) — Google OAuth Submission (CRITICAL PATH)
- [ ] Create Google Cloud project
- [ ] Set up OAuth consent screen
- [ ] Submit Google Calendar API verification (sensitive scope)
- [ ] Draft Privacy Policy + ToS + MHMDA Health Data Policy
- [ ] **This blocks Sprint 2 — do not delay**

### Day 5-6 (Tue-Wed 6/2-3) — Outreach Wave 1
- [ ] Email Tracy Otsuka (`tracy@adhdforsmartasswomen.com`) — use template from `experiment-design.md`
- [ ] Email Kristen Carder (`kristen@ihaveadhd.com`) as parallel option
- [ ] Email ADDitude editorial pitch ("ADHD founder builds the planner he wanted" angle)
- [ ] DM 20 ADHD micro-creators (10-100K followers) offering free annual sub for honest review
  - Use template from `experiment-design.md`
  - Target: Dani Donovan, Rene Brooks, Catieosaurus, Connor DeWolfe, The Mini ADHD Coach + 15 more
- [ ] Twitter/X poll: "ADHD adults — which planner app are you using right now?"

### Day 7 (Thu 6/4) — Reddit Value Post + Audit
- [ ] Read r/ADHDWomen mod rules carefully
- [ ] Post value question (NO link to product): "How do you actually plan your week with ADHD?" — use template
- [ ] Engage replies for 48 hours
- [ ] **Audit:** confirm UI "90% done" claim against feature list F1-F10. Honest self-assessment.

**Week 1 Deliverables:**
- ✅ Waitlist landing page LIVE
- ✅ Google OAuth submitted (clock started)
- ✅ Tracy/Kristen outreach sent
- ✅ Twitter poll launched
- ✅ Reddit value post live
- ✅ UI completion honestly assessed

**Week 1 Spending:** ~$30-80 (domain, Carrd Pro)

---

## Week 2: Validation Signals + Build Sprint 1
**(2026-06-05 to 2026-06-11)**

### Day 8-10 (Fri-Sun 6/5-7) — Build Sprint
- [ ] F1 (Voice brain-dump → AI plan) integration with OpenAI Whisper + GPT-4o-mini
- [ ] F2 (Weekly view UI) polish + state management
- [ ] F8 (Onboarding <90s) build founder voice intro + voice prompt flow
- [ ] Monitor waitlist signups daily (target: 20+ by end of Week 2)

### Day 11 (Mon 6/8) — **WWDC DAY** 🚨
- [ ] Watch Apple WWDC keynote 10am PT live
- [ ] Filter announcements for: AI calendar, Siri scheduling, intelligent planning, ADHD-aware features
- [ ] **DECISION within 24 hours:**
  - **Version A (no scheduler announcement)** → proceed with Version A copy, launch June 22
  - **Version B (generic AI scheduler)** → reposition as "ADHD layer", launch July 1
  - **Version C (ADHD-aware Apple scheduler)** → PAUSE, evaluate pivot or kill within 72 hours
- [ ] Update landing page + all marketing materials per chosen version

### Day 12-13 (Tue-Wed 6/9-10) — Build Sprint Continued
- [ ] F6 (Voice quick-add) — reuse F1 infrastructure
- [ ] F7 (Refund + 2-tap cancel) — StoreKit2 integration
- [ ] F5 (Gentle push notifications) — OneSignal free tier
- [ ] Begin TestFlight build preparation

### Day 14 (Thu 6/11) — Signal Check + Outreach Wave 2
- [ ] Audit waitlist signups + channel performance
- [ ] Audit Twitter poll results (target 100+ votes)
- [ ] Audit Reddit value post engagement
- [ ] **Mini-checkpoint:** if <30 waitlist signups by Day 14, re-examine positioning before continuing
- [ ] Tracy Otsuka follow-up (if no response by now)
- [ ] DM 30 more ADHD micro-creators

**Week 2 Deliverables:**
- ✅ WWDC decision made (A/B/C)
- ✅ F1/F2/F6/F7/F8 working in development
- ✅ 30-50 waitlist signups accumulated
- ✅ Tracy Otsuka response (or fallback to Kristen)

**Week 2 Spending:** $0 cash (founder time only)

---

## Week 3: Validation Experiments + Build Sprint 2
**(2026-06-12 to 2026-06-18)**

### Day 15-17 (Fri-Sun 6/12-14) — Sprint 2: Sync
- [ ] F4 (Apple EventKit) — read + write integration
- [ ] F3 (Google Calendar OAuth) — finish integration (assumes Google approved by now; if not, manual fallback)
- [ ] F10 (Settings) — basic account management
- [ ] F9 (Privacy + MHMDA policies) — finalize legal docs

### Day 18 (Mon 6/15) — TestFlight Beta Launch
- [ ] Submit TestFlight build to Apple
- [ ] Email first 50 waitlist members with TestFlight invite
- [ ] Use TestFlight welcome email template from `experiment-design.md`
- [ ] Start tracking Mixpanel funnel events (install → voice → calendar connect → Day 1 return)

### Day 19-20 (Tue-Wed 6/16-17) — Beta Iteration
- [ ] Daily check of TestFlight feedback + analytics
- [ ] Critical bug fixes only (no scope creep)
- [ ] Direct DM to first 10 beta testers offering 15-min call
- [ ] Target: voice brain-dump completion ≥60% in first session

### Day 21 (Thu 6/18) — Pre-Launch Audit
- [ ] App Store submission preparation: screenshots, video preview, description, keywords
- [ ] Submit Privacy Nutrition Label
- [ ] Apply to Apple Small Business Program (15% fee — CRITICAL)
- [ ] Schedule ProductHunt launch for chosen date (June 22 or July 1)

**Week 3 Deliverables:**
- ✅ TestFlight beta live with 50 users
- ✅ F1-F10 functionally complete
- ✅ App Store submission ready
- ✅ Apple SBP application submitted
- ✅ ProductHunt scheduled

**Week 3 Spending:** $0-500 (legal review if needed)

---

## Week 4: MVP Scoping Refinement + Launch Day
**(2026-06-19 to 2026-06-25)**

### Day 22-23 (Fri-Sat 6/19-20) — Pre-Launch Final
- [ ] Final QA on TestFlight build
- [ ] Apple App Store review submission (allow 24-48 hr review)
- [ ] Tracy Otsuka episode recorded (if deal closed)
- [ ] Final waitlist email scheduled for launch day

### Day 24 (Sun 6/21) — Launch Day Eve
- [ ] All systems check
- [ ] Founder time: rest, eat, sleep early
- [ ] Pre-write Day 0 social posts (5-7 TikToks, Twitter thread, Reddit announcement)

### Day 25 (Mon 6/22) — **🚀 LAUNCH DAY** (Version A) OR Delay to July 1 (Version B/C)
- [ ] 6:00 AM PT: App Store live, Google Play live (if Android included)
- [ ] 7:00 AM PT: ProductHunt launch posted
- [ ] 8:00 AM PT: Waitlist email blast: "Planny is live. 7-day annual at $39 (33% off)."
- [ ] 9:00 AM PT: First TikTok of founder voicing his own week
- [ ] 10:00 AM PT: HackerNews "Show HN: Planny — ADHD weekly planner I built because Tiimo broke my brain"
- [ ] 11:00 AM PT: Twitter announcement thread
- [ ] 1:00 PM PT: Reddit r/ADHDWomen post (per mod rules — value-first)
- [ ] Throughout day: respond to every DM + review + reply
- [ ] **Tracy Otsuka episode airs** (if scheduled)

### Day 26-28 (Tue-Thu 6/23-25) — Honeymoon Period
- [ ] Daily TikTok (founder POV)
- [ ] Respond to every review (signed "Afek")
- [ ] DM every paying user with thank-you + 15-min interview offer
- [ ] Apple Search Ads test: $50/day, productivity keywords
- [ ] Monitor refund rate hourly (alert if >15% in any 24-hour window)
- [ ] Monitor voice brain-dump completion rate (target ≥70%)

**Week 4 Deliverables:**
- ✅ Planny launched on App Store + Google Play
- ✅ First 30-60 paying users acquired
- ✅ Tracy Otsuka episode aired
- ✅ Initial retention + refund + completion metrics

**Week 4 Spending:** $300-800 (ASA test + Tracy episode + any last-minute legal)

---

## Day 30 Mini-Decision Gate
**(2026-06-27 — End of Plan)**

### Hard Numbers Check
| Metric | Target | Action if Missed |
|--------|--------|------------------|
| Cumulative paying users | 30-50 | <15: re-examine positioning |
| Voice brain-dump completion | ≥60% | <40%: emergency onboarding rework |
| Refund rate | <10% | >15%: pause ASA, investigate |
| Apple Search Ads CPA | <$8 | >$15: kill paid, double organic |
| Day-7 retention (cohort 1) | ≥30% | <15%: emergency call with advisor |

### Founder Self-Check
- Am I still excited about Planny?
- Am I tempted to pivot to other 2 startups?
- Has any data invalidated my core assumptions?
- Should I commit Day 90 to Planny full-focus?

---

## Beyond Day 30 — Continuation

### Month 2 (Day 31-60)
- Iterate based on Day 30 cohort retention data
- Build v1.1 features (Energy-aware mode, Weekly review prompt, Widget)
- Scale Apple Search Ads with reinvestment
- ADDitude newsletter slot (if not yet booked)
- Apple SBP approval received → re-baseline projections

### Month 3 (Day 61-90)
- Cohort 1 Day-30 retention measurement → kill criteria check
- Decision Day 90: continue / pivot / kill
- If continuing: Month 4-6 planning
- If pivoting: V1 Working Parents from Brainstorm doc
- If killing: refund all annual subs, document learnings, move to next startup

---

## Spending Allocation Summary (30 Days)

| Category | Amount | Status |
|----------|--------|--------|
| Domain + hosting | $30-50 | Critical |
| Carrd Pro | $19 | Optional |
| Legal review (Privacy + MHMDA) | $500-1,000 | Important |
| Tracy Otsuka / Kristen pod episode | $600-1,000 | High ROI |
| Apple Search Ads test (3 weeks) | $300-500 | Test |
| Buffer | $100 | Reserve |
| **Total Month 1** | **$1,549-2,669** | (overlap with revenue if launch successful) |

---

## What Could Go Wrong This Month

### Critical
- **WWDC June 8 Apple ships ADHD-aware scheduler** → Activate Version C plan
- **Google OAuth review rejected or delayed >6 weeks** → Manual import fallback, delay launch
- **App Store rejects on health/medical grounds** → Productivity category appeal
- **Voice brain-dump UX fails in TestFlight (<40% completion)** → Onboarding rework, delay launch 2 weeks
- **Founder burnout** → Hard stop, 1 week off, re-evaluate

### Manageable
- Tracy Otsuka declines → Fallback to Kristen Carder + diversified micro-creators
- Reddit r/ADHDWomen mods ban post → DM-based discovery + Facebook ADHD Women Support
- Apple Search Ads CPA spikes → Reduce paid spend, double organic content
- 90% UI overstated → Honest reschedule + scope cut to F1+F3+F8 minimum viable

---

## Founder Pre-Commit Statement (Sign Mentally)

Before starting Day 1:

> I commit to:
> - Following this plan for 30 days
> - Honoring the kill criteria if data demands it
> - Being honest in my self-checks
> - Maintaining 30 hrs/week max (anti-burnout)
> - Disclosing my ADHD publicly (it's my unfair advantage)
> - Refunding any user who asks, no questions, within 48 hours
> - Comparing Planny apples-to-apples vs Startup 2 + Startup 3 if I get distracted
>
> I acknowledge that:
> - The data may tell me to stop
> - $1,500 + my time is what I'm risking
> - The 2 other startups exist as Plan B
> - Success is not pre-ordained
>
> I have an ADHD brain. This is what I built for it.

---

## Next Steps After Reading This

1. Read the scorecard (`planny/06-validation/scorecard.md`)
2. Read the validation playbook (`planny/06-validation/validation-playbook.md`)
3. Read the experiment design (`planny/06-validation/experiment-design.md`) — has all copy templates
4. **Start Day 1 tomorrow (2026-05-29).**

You have everything you need. Go.

— Validation methodology by startup-design skill v1.6.0
