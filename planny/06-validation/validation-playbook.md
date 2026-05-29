# Validation Playbook — Planny

**Phase:** Phase 8 — Validation (Playbook)
**Project:** startup-validation (Planny)
**Date:** 2026-05-28
**Confidence:** Medium-High — סדר הניסויים מבוסס ישירות על Phase 4 GTM (90-day channel calendar) + Phase 6 MVP (success criteria) + Phase 7 Projections (existential variable = D30 retention) + Phase 3 Audience (Maya channels). נקודות החולשה: (1) חלק מהניסויים תלויים בתגובה חיצונית מחוץ לשליטת המייסד (Tracy Otsuka, r/ADHDWomen mods); (2) D30 retention benchmark ל-ADHD audience לא קיים פומבית — ה-floor של 4.1% (productivity) ו-ceiling 16% (evidence-based best-in-class) הם proxy; (3) WWDC June 8 הוא binary risk event שעלול לבטל את כל הסדר תוך 11 ימים.

---

## תקציר Playbook

**אסטרטגיית הולידציה היא funnel של risk-burn מהזול לקריטי**: קודם בודקים שהביקוש בכלל קיים ($0-50 בשבועיים), אחר כך שהפרסונה והמסר מדויקים (חינם + שעות-מייסד), אחר כך שהמוצר עצמו עובד ב-beta סגור (TestFlight, $0), ורק אז משקיעים כסף אמיתי בערוצי הפצה ($1,000-2,000). הסיבה: כל ניסוי שמופעל מחוץ לסדר הזה — שורף תקציב על הנחות שלא נבדקו.

**מה לעשות קודם (2-3 שבועות הקרובים, $0-150):** Experiments 1-5 — landing page + Twitter poll + Reddit value post + Tracy outreach + 5-10 in-person coffee chats בארה"ב. אלו ה-cheapest data שנקבל בכל החיים של Planny, והם בודקים את ה-3 הנחות הבסיסיות (יש ביקוש, יש שפה משותפת עם Maya, יש willingness-to-pay).

**מה לעשות אחר כך (3-4 שבועות לפני launch, $0):** Experiments 6-7 — TestFlight beta (50-100 משתמשים מה-waitlist) + pricing A/B in-beta. אלו ה-product-validation experiments — בודקים שה-Aha moment עובד, ש-voice completion >70%, ש-Day-7 retention >40%, ושה-trial structure (annual-only) לא קורס.

**מה לדחות ל-launch ואחריו ($1,000-2,000):** Experiments 8-13 — Apple Search Ads, Tracy Otsuka episode, refund tracking, Day 30/90 cohort retention, NPS, coach affiliate. אלו ה-existential experiments — Experiment 11 (D30 retention) הוא ה-#1 משתנה בכל הסיפור הפיננסי (per `projections.md` — אם D30 <6%, model מתפרק תוך 6-9 חודשים).

**מה לא לעשות כרגע:** Meta paid, TikTok paid, Google Search Ads, BetterHelp affiliate, conferences, Jessica McCabe pitch — כל אלו מסוננים ב-`go-to-market.md` כ-channels to avoid או Year-2.

**הקריטריון לסיום כל ניסוי:** או Validate (עוברים לבא) או Invalidate (עוצרים, מנתחים, אולי pivot). אסור "let's run it longer and see" — זה ה-trap של founders אופטימיים. המודל הפיננסי דורש החלטות בזמן.

---

## Validation Order (Cheapest/Fastest → Most Expensive)

### Pre-Launch Phase (Now → Launch Day, May 28 → June 22)

#### Experiment 1: Waitlist Landing Page Demand Test
- **Tests:** האם קיים demand בפרסונת Maya למוצר ADHD weekly planner ב-price point $9.99/$39.99/$59.99 — באמצעות email capture
- **Cost:** $0-50 (domain planny.app $12/yr already in budget; Carrd free tier sufficient OR Carrd Pro $19/yr; ConvertKit free tier <1K subs)
- **Time:** 2-3 hours setup + 2-3 weeks signal collection (overlaps with Experiments 2-4)
- **How (step-by-step):**
  1. Register planny.app domain (already in Week 1 of GTM calendar)
  2. Build single-page Carrd/Framer landing page
  3. Hero copy (verbatim from positioning): **"Planny: a weekly planner for late-diagnosed ADHD women. By an ADHD adult, for ADHD adults. Coming June."**
  4. Sub-hero: **"Voice your week in 60 seconds. No setup. No streaks. No shame."**
  5. CTA: "Join the waitlist — first 100 get 50% off year one"
  6. Email capture form → ConvertKit free tier
  7. Add social proof if any (founder Twitter handle, "Built by Afek — diagnosed at 31")
  8. Source attribution via UTM params (twitter, reddit, tiktok, dm)
  9. Distribute: founder Twitter (#buildinpublic), 1 r/ADHDWomen value post (READ MOD RULES FIRST — link in bio only), 20 DMs to ADHD micro-creators with personal note, Twitter/X poll (see Exp 2)
- **Measure:**
  - Email signups per visit (conversion rate)
  - Total emails in 2-3 weeks
  - Source attribution (which channel converts best)
  - Bounce rate (>80% = headline mismatch)
- **Validate:** ≥2% visit-to-email conversion + ≥200 emails in 2-3 weeks
- **Invalidate:** <0.5% conversion OR <50 emails in 3 weeks → re-examine positioning copy + audience fit BEFORE launch

---

#### Experiment 2: Twitter/X Poll on Current Behavior
- **Tests:** מה ADHD adults משתמשים בו היום + מה עובד/נכשל — proxy ל-switching intent
- **Cost:** $0
- **Time:** 5 min setup + 24-48 hr collection
- **How (step-by-step):**
  1. Post from founder's personal Twitter/X account (must be visible as ADHD-self-identifying founder)
  2. Poll text: **"ADHD adults — which planner app are you using right now? [Tiimo / Sunsama / Apple Reminders / Paper / Nothing]"**
  3. Add context tweet: "Building Planny — a weekly planner for late-diagnosed ADHD adults. Trying to understand what's actually in use today."
  4. Tag 2-3 ADHD-adjacent accounts for visibility (Tracy Otsuka, ADDitude — without aggressive ask)
  5. Pin tweet for 48 hours
  6. Reply to every commenter — qualitative gold mine
- **Measure:**
  - Total votes
  - Distribution across options ("Nothing/Paper" % is the key signal)
  - Number of qualitative replies + screenshot-quote-worthy ones for landing page social proof
- **Validate:** ≥100 votes + ≥30% "Nothing/Paper" → confirms unmet need (gap is real, not just preference)
- **Invalidate:** <50 votes → weak signal; founder Twitter not yet warmed up; re-run after first viral TikTok

---

#### Experiment 3: Reddit r/ADHDWomen Value Post (No Promo)
- **Tests:** האם framing + language של Planny רוננים עם הקהל הצפוף ביותר של Maya (700K members, zero direct competitor presence)
- **Cost:** $0
- **Time:** 1 hour to write + 24-72 hr to engage with comments
- **How (step-by-step):**
  1. Founder Reddit account must have ≥10 substantive comments in r/ADHDWomen before posting (per Week 1 GTM calendar)
  2. Read mod rules carefully — NO link to Planny in post body (only in user bio)
  3. Post title: **"How do you actually plan your week with ADHD? I'm a founder building something but want to learn what's already working."**
  4. Body: 200-300 words. Share founder ADHD identity ("Diagnosed at 31, building the planner I couldn't find"), describe the planning problem you're researching, ask 2-3 open questions ("What's worked? What's broken? What do you wish existed?")
  5. NO product mention, NO CTA, NO link
  6. Respond to every comment within 6 hours for first 24 hours
  7. Track DMs received separately
- **Measure:**
  - Upvotes (proxy for community resonance)
  - Substantive comments (>10 words)
  - DMs received asking what you're building (highest-intent signal)
  - Removal/lock by mods (red flag)
- **Validate:** ≥50 upvotes + ≥10 substantive comments + ≥3 DMs asking what you're building
- **Invalidate:** <10 upvotes OR downvoted OR removed → message/framing problem; rewrite from "asking" stance, not "building" stance, and retry in r/ADHD (1.5M, less strict)

---

#### Experiment 4: Tracy Otsuka / Kristen Carder Outreach Test
- **Tests:** Creator partnership feasibility — does the single largest planned acquisition channel (Tracy = 150K monthly Maya-perfect listeners) respond + fit budget?
- **Cost:** $0 outreach; depends on what comes back (budget cap $1,500 cash)
- **Time:** 30 min email + 1-2 weeks response time
- **How (step-by-step):**
  1. Email tracy@adhdforsmartasswomen.com (primary) AND form on tracyotsuka.com (secondary) — both Day 1
  2. Subject: "A planner built for the Smart Ass Women audience — co-design opportunity"
  3. Body structure:
     - Founder ADHD story (Afek, diagnosed late, solo)
     - Product 1-paragraph description
     - 90-sec Loom demo link (must be ready before email send)
     - 60-sec audio sample (founder voice, podcast-quality)
     - Specific ask: host-read mid-roll slot in 1 episode
     - Hybrid offer: $1,500 cash + 25% lifetime affiliate on attributed signups + Founder's Tier free for Tracy and her coaching cohort + co-designed "Smart Ass Women Weekly" template inside Planny credited to her
  4. Parallel email to Kristen Carder (kristen@ihaveadhd.com) — same structure, $800 single episode ask (fallback)
  5. If no response from Tracy by Day 14, activate Kristen as primary
- **Measure:**
  - Response received Y/N within 14 days
  - Rate quoted (vs $1,500 cap)
  - Willingness to do hybrid cash + affiliate
  - Audience fit confirmation (does she think it fits her listeners?)
- **Validate:** Response within 2 weeks + rate ≤$1,500 cash OR rev-share offer accepted OR Kristen books at $800-1,200
- **Invalidate:** No response from EITHER within 3 weeks OR rate >$2,500 single slot from both → pivot to triple micro-creator gifting (50 → 75 creators) + ADDitude paid newsletter slot ($400-800 small-biz tier)

---

#### Experiment 5: 5-10 In-Person Coffee Conversations (US Trip)
- **Tests:** Maya persona accuracy, pricing acceptance, wedge resonance, friction points — **THE single highest-leverage experiment in the entire playbook** since founder will be in US (~1 month from today)
- **Cost:** $50-150 (coffee tabs $5-15 per person × 5-10 people)
- **Time:** 30 min each × 5-10 = 2.5-5 hours actual interview time; +2-3 hours coordination
- **How (step-by-step):**
  1. Once US trip dates locked, post in r/ADHDWomen [city] subreddit (e.g., r/AskNYC + r/ADHDWomen cross-post per rules): **"ADHD founder visiting [city] [dates]. Buying coffee for 5 ADHD women willing to chat 30 min about planning apps. No sales pitch — just listening."**
  2. Alternative recruitment: DM 20-30 ADHD TikTok creators in target city OR post in NYC/NJ ADHD meetup.com groups OR ask Tracy Otsuka for 2-3 community member intros (if Exp 4 succeeded)
  3. Screen volunteers via 3 questions in DM: (a) When were you diagnosed? (b) What planner apps have you tried? (c) Age + city — confirm Maya fit
  4. Schedule 30-min coffees, batch in 2 days
  5. Interview script (must hit all 4 categories):
     - **Persona accuracy:** Demographics, diagnosis story, current workflow — does 7+/10 match Maya profile in `target-audience.md`?
     - **Pricing acceptance:** Show 3 price points ($9.99/$39.99/$59.99 annual). "Would you pay this? Why/why not?" — watch facial reaction, not just words
     - **Wedge resonance:** Show 90-sec Loom of voice brain-dump → weekly plan. "Does this solve a problem you have? Would you switch from [current tool]?"
     - **Friction:** "Walk me through how you'd use this. Where would you stop or get confused?" — observe, don't lead
  6. Bring printed consent form (you're recording) + offer Planny gift code as thank-you
  7. Transcribe within 24 hours; tag themes
- **Measure:**
  - Persona accuracy: % matching Maya profile (target 7+/10)
  - Pricing acceptance: % willing to pay $9.99/mo OR $59.99/yr
  - Wedge resonance: % who say "voice brain-dump" is the lead feature
  - Friction count: shared bounce points (3+ users mention same = signal)
  - Bonus: 2+ quotes worth using as testimonials on landing page
- **Validate:** ≥6/10 confirm willingness to pay + ≥7/10 resonate with voice wedge + ≥5/10 say they'd actually install + try
- **Invalidate:** <3/10 willing to pay → fundamental hypothesis problem; consider V1 Working Parents pivot (per `mvp-definition.md` soft-kill criteria) OR delay launch by 4 weeks for repositioning

---

### Beta Phase (3-4 weeks before launch — June 5 to June 21)

#### Experiment 6: TestFlight Closed Beta — Usage Behavior
- **Tests:** Aha moment works (<90s to first plan), voice UX is acceptable, calendar connection rate holds, Day-7 retention model is plausible
- **Cost:** $0 (Apple TestFlight free, internal analytics free tier)
- **Time:** 3-4 weeks beta + 1 week analysis = 4-5 weeks total
- **How (step-by-step):**
  1. Email waitlist subset: "TestFlight slots opening. Reply if you want in." Pick 50-100 most-engaged respondents (those who replied within 24hr, opened previous emails)
  2. Send TestFlight invites in batches of 20 (manage support load)
  3. Instrument analytics from day 1: PostHog free tier or Mixpanel free tier
  4. Track funnel events: install → onboarding screen 1 → voice mic tap → voice complete → first plan generated → calendar connection → Day 1 return → Day 7 return → Day 14 return
  5. Day 14 in-app survey (3 questions): (a) Would you recommend? 0-10 NPS; (b) What almost made you leave? (c) What's the ONE thing you'd change?
  6. Founder personal DM to every beta user week 1 ("Hey, how's it going? Stuck anywhere?")
- **Measure:**
  - **Voice brain-dump completion in first session:** target ≥70%
  - **Calendar connection (Google or Apple) in first 7 days:** target ≥60%
  - **Day-7 return rate:** target ≥40%
  - **Day-14 NPS:** target ≥40
  - **Median time install → first plan:** target ≤90 seconds
  - **Transcription accuracy:** ≥90% (test diverse cohort if possible, including 2-3 AAVE/accented English speakers per `mvp-definition.md` yellow flag)
- **Validate:** ≥60% voice completion + ≥50% calendar connection + ≥30% return Day-7 + NPS ≥30
- **Invalidate:** <40% voice completion → onboarding flow needs rework BEFORE public launch; delay 1-2 weeks to iterate F1 (voice brain-dump) and F8 (onboarding)

---

#### Experiment 7: Pricing Page A/B Test (Inside Beta)
- **Tests:** Trial structure (annual-only trial vs trial-on-all-tiers) + tier mix (monthly vs 6mo vs annual)
- **Cost:** $0 (StoreKit configuration only)
- **Time:** 2 weeks within beta + 1 week analysis = 3 weeks total
- **How (step-by-step):**
  1. In beta TestFlight, configure 2 StoreKit variants:
     - **Variant A (founder's preferred):** $9.99/mo monthly, $39.99/6mo, $59.99/yr — 14-day trial on ANNUAL ONLY
     - **Variant B:** Same prices — 14-day trial on ALL tiers
  2. Split beta cohort 50/50 randomly via user ID hash
  3. Show paywall after first plan generated (Aha moment)
  4. Track trial start rate, trial-to-paid conversion at Day 14
  5. Run for minimum 50 trial starts per variant (statistical floor)
- **Measure:**
  - Trial start rate per variant
  - Trial-to-paid conversion rate per variant at Day 14
  - Tier selection distribution (monthly vs 6mo vs annual %)
  - Revenue per visitor (RPV) per variant
- **Validate:** Variant A (annual-only trial) converts within 5% of Variant B's blended rate → founder's preferred structure holds; keep annual-only trial for launch
- **Invalidate:** Variant A converts 20%+ worse than Variant B → reconsider; switch to trial-on-all-tiers for launch (sacrifices some annual lock-in but increases trial starts)

---

### Launch Phase (Week 1-4 post-launch — June 22 to July 20)

#### Experiment 8: Apple Search Ads Productivity Spend Test
- **Tests:** Paid channel viability + CAC reality vs 2025 90% YoY CPI jump (per AppTweak benchmarks in `go-to-market.md`)
- **Cost:** $200-500 over 4 weeks (within $1,500 launch budget)
- **Time:** 2 weeks setup + 4 weeks run = 6 weeks total
- **How (step-by-step):**
  1. Apple Search Ads Basic account set up Week 3 of pre-launch (after App Store submission accepted)
  2. Day 0 of launch: activate $50/day budget cap
  3. Keyword groups (3 separate campaigns for attribution):
     - Group 1 — Brand defensive: "Planny", "planny app", "planny adhd"
     - Group 2 — Long-tail ADHD: "ADHD planner for women", "late diagnosed ADHD planner", "ADHD weekly schedule"
     - Group 3 — Discovery + Search Match: let Apple auto-match relevant queries
  4. Cap CPT at $1.50 per keyword
  5. Pause any keyword group with CAC >$40 for >7 consecutive days
  6. After Week 2, scale best-performing group to $100/day; kill worst-performing
- **Measure:**
  - CPI (Cost Per Install) per keyword group
  - Install-to-trial conversion rate
  - Trial-to-paid conversion rate (full funnel)
  - Blended CAC per paying user attributable to ASA
- **Validate:** CPI <$5 + install-to-paid >20% + blended CAC <$25 (LTV $50 → 2:1 minimum per `projections.md`)
- **Invalidate:** CPI >$10 OR CAC >$40 → kill paid ASA, redirect $200-300 remaining to creator gifting expansion (cheaper per acquisition)

---

#### Experiment 9: Tracy Otsuka Podcast Episode (If Booked)
- **Tests:** Podcast channel effectiveness + attribution clarity + viability of single big-bet creator strategy
- **Cost:** $800-1,500 (Tracy) OR $800-1,200 (Kristen fallback)
- **Time:** 4-6 weeks (Week 1 booking → Week 7-10 air → +4 weeks measure)
- **How (step-by-step):**
  1. Booking confirmed (from Exp 4 success)
  2. Founder records 60-sec audio sample + provides 90-sec Loom for host context
  3. Co-design with Tracy: "Smart Ass Women Weekly" template inside Planny, credited to her
  4. Unique discount code for attribution: **PODCAST25** (25% off year 1) OR **TRACY30** (gives Tracy clear branding)
  5. Air date locked → countdown email to waitlist 48 hours before
  6. On air day: TikTok + Twitter cross-promo from founder; pin tweet
  7. Track for 30 days post-air; expect tail through Day 60
- **Measure:**
  - Code redemptions per day for 30 days
  - Organic mentions in r/ADHDWomen (search Reddit weekly)
  - Direct landing page traffic spike (UTM source = podcast)
  - Cost per paying user attributable to episode
- **Validate:** ≥30 paying users attributable within 30 days = $30-50 CAC (acceptable vs LTV $50)
- **Invalidate:** <10 attributable users → channel doesn't work for Planny at this stage; defer creator-paid strategy entirely; double down on free micro-creator gifting

---

#### Experiment 10: 30-Day Refund Test (Always-On Brand Promise)
- **Tests:** Brand promise viability — does the 30-day refund + 2-tap cancel cause refund rate >15% (which would break unit economics per `mvp-definition.md` kill criteria)?
- **Cost:** Refunds paid out (no marketing cost; lost revenue only)
- **Time:** Ongoing from Day 0; meaningful signal at Month 1, 2, 3
- **How (step-by-step):**
  1. Refund button visible in Settings → Subscription for every paying user
  2. Email confirmation upon cancel + upon refund (per F7 in MVP)
  3. Founder receives Slack/email notification on EVERY refund (learning loop, not retention pressure)
  4. Refund processed <48hr p95
  5. Optional exit survey (1 question, optional): "Why are you cancelling?" — for learning only, NEVER blocks the refund
  6. Track refund rate as % of paying users requesting refund within 30 days, by cohort (weekly)
- **Measure:**
  - % refund rate Month 1
  - % refund rate Month 2
  - % refund rate Month 3
  - Top 3 stated reasons (if exit survey opt-in)
- **Validate:** <12% refund rate sustained across Months 1-3 → brand promise is viable, anti-Inflow positioning holds
- **Invalidate:** >18% refund rate sustained → re-examine onboarding quality; tighten paywall expectations; consider sessions-gated refund (<10 sessions in 30 days protection per `projections.md`)

---

### Day 30 & Day 90 Strategic Validations

#### Experiment 11: Day 30 Cohort Retention Analysis (THE EXISTENTIAL TEST)
- **Tests:** **THE existential variable per `projections.md`** — does anti-shame UX actually keep ADHD users engaged at rates materially above productivity benchmark (4.1%)? If <6%, model breaks within 6-9 months.
- **Cost:** $0 (analytics already instrumented from beta)
- **Time:** 30 days per cohort; first reliable signal Month 2 (July 26); second confirmation Month 3 (August 26)
- **How (step-by-step):**
  1. Define cohort: all users who installed + opened app at least once in given week
  2. Cohort 1: Week 1 of launch (June 22-28)
  3. Cohort 2: Week 5 of launch (post-Tracy episode if Exp 9 succeeded)
  4. Track Day 7 + Day 30 retention per cohort, segmented by acquisition channel (waitlist, ASA, Tracy podcast, Reddit, micro-creator, organic)
  5. Cross-segment by user behavior: voice-completers vs text-only; calendar-connected vs not; paid vs trial
- **Measure:**
  - D30 retention rate per cohort (overall)
  - D30 retention rate per acquisition channel
  - D30 retention rate per behavior segment (calendar-connected users should have 10%+ higher D30 per `mvp-definition.md` F4 hypothesis)
- **Validate:** ≥10% D30 (well above 4.1% productivity benchmark; meaningful differentiation)
- **Invalidate:** <5% D30 sustained → model breaks per `projections.md`; trigger one of:
  1. Engineering retention features (energy mode, weekly review prompt, recovery flow) — ship within 2 weeks
  2. Pivot to V1 Working Parents persona (per soft-kill criteria)
  3. Hard kill — return remaining cash + honor refunds

---

#### Experiment 12: Day 90 NPS + Willingness-to-Recommend
- **Tests:** Long-term loyalty + viral coefficient (free user growth via referrals = Y3 base-case driver per `projections.md`)
- **Cost:** $0 (in-app survey)
- **Time:** 30 days survey collection from Day 90+ users
- **How (step-by-step):**
  1. Trigger in-app NPS prompt for users at Day 90+ (only)
  2. Single screen: "How likely are you to recommend Planny to a friend with ADHD? [0-10 slider]" + optional comment box
  3. Show only ONCE per user (no nag); allow dismiss
  4. Collect 50+ responses minimum for statistical signal
  5. Follow up with high promoters (9-10) via DM: "Would you share your Planny experience publicly? We'd love to feature you."
- **Measure:**
  - NPS score (% promoters [9-10] minus % detractors [0-6])
  - Qualitative reasons (top 3 themes from comments)
  - Conversion of promoter follow-ups → public testimonials (creator content, App Store reviews)
- **Validate:** NPS ≥40 (excellent for B2C app), referral intent ≥30%
- **Invalidate:** NPS <20 → fundamental product gap; review qualitative feedback; ship targeted improvements within 30 days

---

#### Experiment 13: ADHD Coach Affiliate Channel Test
- **Tests:** B2B-lite channel viability — can ADHD coaches act as force-multiplier distribution per `go-to-market.md` Tier-3 strategy?
- **Cost:** Forgone commissions (20-30% rev-share Month 1-3 on attributed signups; no upfront cash)
- **Time:** 6-8 weeks (cold outreach → onboarding → first attribution)
- **How (step-by-step):**
  1. Build outreach sheet: 30 ADHD coaches from ICF / ACO / PAAC directories (Dr. Tamara Rosier intro unlocks 100+ if she accepts advisory)
  2. Email template:
     - Subject: "A planning tool that makes your clients more coachable between sessions"
     - Founder ADHD story + product 1-paragraph
     - Offer: 25-30% rev-share Month 1-3; 10-15% lifetime thereafter; coach-tier Planny free; unique tracking code per coach
     - Soft ask: "If a few of your clients would benefit, here's how to share it"
  3. Track per-coach: code given, signups attributed, conversions
  4. Manual attribution via unique codes (defer Rewardful $49/mo until 5+ active coaches)
  5. Send monthly statement + payout (PayPal/Wise) so coaches feel real partnership
- **Measure:**
  - # coaches responded + accepted code
  - # coaches actively sharing (≥1 attributed signup)
  - # attributable paid users via coach codes
- **Validate:** ≥3 active coaches + ≥10 attributable paid users in 8 weeks
- **Invalidate:** <2 coaches respond + <3 conversions → channel doesn't fit yet; defer to Year-2 (after established brand reduces "who are you?" friction)

---

## Validation Sequence Logic

**Cheapest validations FIRST** (Exp 1-5: waitlist, Twitter poll, Reddit value post, Tracy outreach, US coffee chats) — collect signal in 2-3 weeks for $50-200. If any of these invalidate, **don't launch**; iterate first.

**Mid-cost validations BEFORE LAUNCH** (Exp 6-7: TestFlight beta, pricing A/B) — calibrate the product and pricing structure with real users. Free, takes 3-4 weeks. Locks down the final launch version.

**Paid validations DURING LAUNCH** (Exp 8-10: ASA, Tracy podcast, refund test) — burn $1,000-2,000 on channels we expect to work + always-on brand-promise test. Each has clear kill criteria.

**Strategic validations POST-LAUNCH** (Exp 11-13: D30/D90 cohort retention, NPS, coach affiliate) — drive Year 2 decisions (raise, scale, pivot). Exp 11 is the existential test.

**Critical:** Don't run Experiments 8-13 if Experiments 1-5 invalidate. The funnel exists for a reason — burning $1,500 on ASA when nobody wants the product is the classic founder mistake.

---

## Validation Outcomes → Decision Tree

```
After Experiments 1-5 (Pre-launch validation, ~$200 spent):
├── Strong signal (≥4 of 5 Validate) → Proceed with full launch June 22
├── Mixed signal (2-3 of 5 Validate) → Continue, but tighten positioning copy + reduce ASA spend to $100 test
└── Weak signal (<2 of 5 Validate) → Pivot to V1 Working Parents persona OR delay launch 4 weeks for reposition

After Experiments 6-10 (Launch validation, +$1,000-1,500 spent):
├── Aha works (≥60% voice) + CAC <$25 → Scale via creator partnerships + ASA reinvestment from Month 2
├── Aha works + CAC $25-40 → Pull back paid, double down on organic + Tracy podcast amplification
└── Aha doesn't work (<40% voice completion) → Onboarding rework BEFORE scaling acquisition; pause ASA

After Experiment 11 (Day 30 cohort retention — THE EXISTENTIAL TEST):
├── ≥10% D30 → Confirm GO, accelerate creator partnerships, plan Y2 (Android, Hebrew, partner mode)
├── 5-10% D30 → Engineering retention features (energy mode, weekly review, recovery flow); pause new acquisition spend
└── <5% D30 → HARD KILL — model broken per `projections.md`; consider pivot to V1 Working Parents OR sunset gracefully (honor refunds, shut infrastructure)

After Experiments 12-13 (Day 90 strategic):
├── NPS ≥40 + 3+ active coaches → Y2 plan = scale coach affiliate + referral program + raise optionality
├── NPS 20-40 + 1-2 coaches → Y2 = retention engineering + selective coach expansion
└── NPS <20 → Fundamental product gap; 30-day intervention sprint; reconsider Y2 plan
```

---

## Time + Cost Summary

| Stage | Time | Cost | Top Validations |
|-------|------|------|-----------------|
| Pre-launch (3-4 weeks, May 28 → June 21) | 8-15 hours founder time | $50-200 | Exp 1-5: Waitlist, Twitter poll, Reddit value post, Tracy outreach, US coffee chats |
| Beta (3-4 weeks, June 5 → June 25 — overlaps pre-launch) | 5-10 hours | $0 | Exp 6-7: TestFlight beta, pricing A/B |
| Launch (4 weeks, June 22 → July 20) | 5-10 hours | $1,000-2,000 | Exp 8-10: ASA test, Tracy podcast, refund tracking |
| Post-Launch (8 weeks, July 21 → September 20) | 5-15 hours | $0-500 | Exp 11-13: D30/D90 cohort, NPS, coach affiliate |

**Total validation budget:** $1,050-2,700 (overlaps with $1,500 launch marketing budget per `go-to-market.md`)

**Total validation time:** ~30-50 founder hours across 4 months (manageable within 5% measurement allocation per `go-to-market.md` time table)

---

## Validation-Specific Founder Asks

1. **Are you willing to do 5-10 in-person interviews when you're in the US in ~1 month?** This is the **highest-leverage validation experiment** in the entire playbook. Without it, the Maya persona remains inferred, not validated. **Required commitment: 1 day of US trip dedicated to coffee chats.**

2. **Can you find 2-3 hours to set up the waitlist landing page this week (Week 1)?** This is the cheapest data we'll ever get on Planny. Every day of delay = lost signal window before launch.

3. **Are you OK if Experiment 11 (D30 retention) returns <5% and we hard-kill the project?** That's the deal — kill criteria honored, not rationalized away. The financial model breaks at <6% D30 retention; "let's try harder" is not an option without external capital.

4. **Are you OK skipping ASA paid spend (Exp 8) if Exp 1-5 invalidate?** $200-500 saved on ASA in a "weak signal" scenario buys 3-6 weeks of iteration runway. Discipline > optimism.

5. **Will you read the qualitative DMs from r/ADHDWomen (Exp 3) without arguing back?** The first 10 DMs are the most honest market research you'll ever get. Listen, don't defend.

---

## Strategic Connections

- ראה `risk-analysis.md` (TBD) ל-risk matrix מלא + WWDC contingency planning
- ראה `assumptions-tracker.md` (TBD) ל-all-assumptions inventory cross-referenced to experiments
- ראה `experiment-design.md` (TBD) ל-detailed templates for top 3 experiments (Waitlist, TestFlight beta, D30 cohort)
- ראה `kill-criteria.md` (TBD) ל-decision thresholds per stage + scenario triggers
- ראה `scorecard.md` (TBD) ל-final assessment + Y1 review framework
- ראה `../02-strategy/go-to-market.md` ל-90-day channel calendar that experiments integrate with
- ראה `../04-product/mvp-definition.md` ל-success criteria + validation hypotheses + falsification conditions
- ראה `../05-financial/projections.md` ל-sensitivity analysis (D30 retention as #1 variable)
- ראה `../01-discovery/target-audience.md` ל-Maya persona + channel ROI ranking

---

## Sources

### Internal Phase Documents
- `/home/user/NEW-_PROJECT/startup-validation/02-strategy/go-to-market.md` — 90-day channel calendar, channel ROI ranking, kill criteria
- `/home/user/NEW-_PROJECT/startup-validation/04-product/mvp-definition.md` — success criteria, validation hypotheses, falsification conditions, F1-F10 features
- `/home/user/NEW-_PROJECT/startup-validation/05-financial/projections.md` — sensitivity analysis, D30 retention as existential variable, decision gates
- `/home/user/NEW-_PROJECT/startup-validation/01-discovery/target-audience.md` — Maya persona, channel density ranking, Aha moment definition

### External Benchmarks
- [RevenueCat State of Subscription Apps 2026](https://www.revenuecat.com/state-of-subscription-apps/) — D30 productivity 4.1%, trial-to-paid opt-in 18-25%, NPS B2C benchmarks
- [AppTweak Apple Ads Benchmarks 2025](https://www.apptweak.com/en/aso-blog/apple-ads-benchmarks) — Productivity CPI $3.13, CPA $2.84-$3.76, 90% YoY jump
- [Adapty State of In-App Subscriptions 2026](https://adapty.io/blog/state-of-in-app-subscriptions/) — US productivity avg $15.20/mo
- [Tracy Otsuka — ADHD for Smart Ass Women](https://tracyotsuka.com/podcast) — 8M downloads, 150K monthly listeners
- [ADDitude Advertising](https://www.additudemag.com/contact-us/advertise/) — Newsletter sponsorship rates
- [Apple TestFlight Documentation](https://developer.apple.com/testflight/) — Closed beta best practices
- [Reddit r/ADHDWomen](https://www.reddit.com/r/ADHDWomen/) — 700K members, mod rules reference

---

## Flags

### Red Flags

- **R1 — Founder must commit to executing experiments.** Without execution, validation is theater. The playbook fails if founder runs Exp 1-2 but skips Exp 5 (US coffee chats) — that's the highest-leverage experiment and depends on personal commitment, not budget.

- **R2 — Experiment 11 (D30 retention) is the EXISTENTIAL test.** Per `projections.md`, D30 <6% breaks the financial model within 6-9 months. Founder must agree pre-launch to hard-kill criteria if this fails — no "let's run it longer" exceptions. Without this commitment, the playbook is theater.

- **R3 — WWDC June 8 binary risk is unaddressed in pre-launch experiments.** If Apple announces ADHD-aware AI scheduler, Experiments 1-5 may already have invalidated by Day 11 of playbook execution. Mitigation: monitor WWDC live; pre-build Version B/C messaging per `go-to-market.md`.

- **R4 — US coffee chats (Exp 5) require US trip in ~1 month.** If trip is delayed/cancelled, Exp 5 is non-runnable; persona validation drops from "primary signal" to "inferred only." No remote substitute is equivalent.

- **R5 — Inflow $11M war chest may outbid Planny on ASA keywords (Exp 8)** within first 30 days of launch. If CPI spikes >$10 immediately, Exp 8 invalidates faster than expected; pivot to creator gifting must be ready Day 14.

### Yellow Flags

- **Y1 — Some experiments depend on creator response** (Tracy, Kristen) — out of founder control. Fallback paths exist (micro-creators + ADDitude paid), but cost differential is real.

- **Y2 — Reddit r/ADHDWomen value post (Exp 3) risks ban if mod rules misinterpreted.** Single self-promo violation = permanent ban from THE highest-density Maya channel. Founder must read mod rules carefully + post zero links in body.

- **Y3 — TestFlight beta (Exp 6) may have selection bias** — waitlist users are highest-intent, not representative of cold acquisition users. D7 retention from beta may overstate D7 from ASA/podcast cohorts. Account for this when projecting from beta data.

- **Y4 — Pricing A/B (Exp 7) needs minimum 50 trial starts per variant for statistical signal.** If beta is <100 users, statistical confidence is low; treat as directional, not conclusive.

- **Y5 — Day 90 NPS (Exp 12) collection depends on users surviving to Day 90.** If D30 retention is low (Exp 11 invalidates), NPS sample size collapses; experiment becomes unmeaningful.

- **Y6 — Coach affiliate (Exp 13) requires Dr. Tamara Rosier advisory acceptance for force-multiplier.** Without her network, cold-outreach to 30 coaches may yield <2 responses; experiment risks invalidating by recruitment failure, not channel failure. Disambiguate carefully.

- **Y7 — Refund test (Exp 10) is always-on but only meaningful at scale.** With <50 paying users in Month 1, refund rate has high variance (one refund = 2% swing). Wait for Month 2-3 cohort signal before deciding.

- **Y8 — Spending on Tracy Otsuka (Exp 9) is a $1,500 single bet** that consumes the entire validation cash budget. If Exp 9 invalidates, no cash left for Exp 13 coach affiliate setup tooling. Sequencing matters.
