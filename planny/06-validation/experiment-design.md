# Experiment Design — Top 3 (Planny)

**Phase:** Phase 8 — Validation (Experiment Design)
**Project:** startup-validation (Planny)
**Date:** 2026-05-28
**Confidence:** Medium-High — שלושת הניסויים נבחרו ישירות מ-`validation-playbook.md` לפי קריטריון ROI (cost-per-learning ÷ time-to-signal ÷ decision-impact). Experiment 1 (Waitlist) הוא ה-cheapest signal עם הכי הרבה optionality; Experiment 5 (US Coffee Chats) הוא ה-highest-signal-to-noise חלון זמן (טיסה עוד חודש); Experiment 6 (TestFlight) הוא ה-only product-validation gate לפני public launch. סיכון עיקרי: כל השלושה תלויים ב-founder execution discipline, לא בכסף.

---

## תקציר

שלושת הניסויים האלה — Waitlist, US Coffee Chats, ו-TestFlight Beta — הם **ה-validation funnel המינימלי** שצריך להריץ ב-4-6 השבועות הקרובים לפני launch בסוף יוני. הם נבחרו מתוך 13 הניסויים של ה-playbook כי הם עונים על שלוש שאלות שונות לחלוטין: **(1) האם יש demand?** (Waitlist — quantitative, broad signal), **(2) האם Maya היא באמת Maya?** (Coffee Chats — qualitative, deep signal, חד-פעמי כי הטיסה לארה"ב היא time-bounded window), ו-**(3) האם המוצר עובד?** (TestFlight — behavioral, pre-launch product gate). ביחד הם מכסים את הסיכון העיקרי של pre-launch — שאתה משקיע 6 שבועות וגיוס כסף בערוץ שאף אחד לא רוצה את המוצר שלך, או רוצה אבל לא ב-price point הזה, או נרשם אבל לא משלים את ה-onboarding.

ה-deliverables: (1) Carrd landing page חי + 200+ emails ב-ConvertKit + attribution per channel; (2) 5-10 transcribed interviews + persona match scorecard + 2-3 verbatim quotes ל-testimonials; (3) TestFlight cohort של 50-100 משתמשים + funnel events ב-Mixpanel + NPS Day 14 + Day 7 retention number. כל deliverable מזין ישירות החלטה GO/NO-GO ל-launch ב-22 ביוני.

כל הניסויים תוכננו עם **kill criteria מפורשים** — אם Waitlist <100 emails, אם <3/10 בקפה אומרים willing-to-pay, או אם <40% משלימים voice ב-beta — עוצרים, מנתחים, ומשקלים pivot (V1 Working Parents per `mvp-definition.md` soft-kill) או delay של 4 שבועות. אסור "let's run it longer." המודל הפיננסי דורש decision discipline, לא founder optimism.

---

## Top 3 Selected Experiments (ranked by ROI)

1. **Experiment 1: Waitlist Landing Page Demand Test** — cheapest ($0-50), fastest (2-3 weeks), lowest friction, broadest signal. עונה: "האם יש בכלל demand?"
2. **Experiment 5: In-Person Coffee Conversations (US Trip)** — highest signal-to-noise per dollar ($50-200), time-bounded (חלון הטיסה לארה"ב, ~חודש מהיום, לא חוזר). עונה: "האם Maya היא Maya, ובאיזה price?"
3. **Experiment 6: TestFlight Closed Beta** — only pre-launch product gate ($0), 3-4 שבועות, גזר ישיר ל-Aha-moment hypothesis. עונה: "האם המוצר עובד לפני שאני שורף $1,500 על ASA?"

**Why not Experiment 11 (D30 Retention) in top 3?** הוא ה-existential test, אבל הוא **post-launch** — אי אפשר להריץ אותו ב-pre-launch. הוא מופיע ב-playbook כ-#1 strategic experiment אבל בסדר זמן הוא בא רק אחרי שיש cohorts אמיתיים ב-app.

---

## EXPERIMENT 1: Waitlist Landing Page Demand Test

### Hypothesis

**H1 (primary):** Late-diagnosed US women 25-40 with ADHD will sign up for a waitlist for "Planny — voice your week, by an ADHD adult, for ADHD adults" at a rate of **>2% from organic traffic** and **>15% from targeted DM outreach**, with **≥200 total emails captured in 2-3 weeks**.

**H1 invalidate:** <0.5% organic conversion **AND** <5% DM conversion **AND** <50 total emails in 3 weeks → positioning is not landing OR audience cannot be reached at this distribution scale → re-examine positioning copy + channel choice **before** launch.

**Sub-hypotheses:**
- **H1a:** Source attribution will show r/ADHDWomen + creator DMs convert at 3-5x higher rate than founder Twitter cold posts (validates community-first GTM)
- **H1b:** Pricing visibility ($9.99/mo, $59.99/yr, 30-day refund) on landing page does **not** depress conversion (vs. price-hidden variant) — Maya values transparency over surprise

### Method

1. **Build** single-page landing site in Carrd Pro ($19/yr) or Framer free tier
2. **Distribute** via 4 channels in parallel with UTM tracking:
   - Founder Twitter/X organic (UTM: twitter)
   - r/ADHDWomen value post (UTM: reddit — link in user bio only, NOT post body)
   - 20 DMs to ADHD micro-creators with personal note (UTM: dm)
   - Twitter/X poll on current planner usage (UTM: poll)
3. **Collect** emails into ConvertKit free tier (<1,000 subs free)
4. **Measure** for 14-21 days
5. **Analyze** + decide

### Metrics

- **Primary:** Total emails captured (target ≥200 in 2-3 weeks)
- **Secondary:** Conversion rate per channel (visit-to-email)
- **Tertiary:** Source attribution distribution (which channel delivers Maya, not just emails)
- **Qualitative:** Comments / DMs / quoted responses (testimonial candidates + objection patterns)

### Success Criteria

| Outcome | Threshold | Decision |
|---------|-----------|----------|
| **Validate** | ≥200 emails + ≥2% organic conversion + ≥15% DM conversion | Proceed to launch June 22; use waitlist as TestFlight beta recruitment pool (Exp 6) |
| **Mixed** | 100-200 emails OR organic conversion 1-2% | Continue, but tighten messaging per source attribution; reduce paid ASA Exp 8 to $100 test |
| **Invalidate** | <100 emails + organic conversion <1% | Halt launch trajectory; positioning re-examination; consider 4-week delay OR V1 Working Parents pivot (per `mvp-definition.md` soft-kill) |

### Timeline

- **Day 1-2:** Register domain (planny.app already in budget), build Carrd landing page, ConvertKit setup, UTM links built
- **Day 3:** Distribute across 4 channels (batch in single morning)
- **Day 4-21:** Collect emails + monitor + reply to comments/DMs daily
- **Day 22-23:** Analyze attribution + conversion + qualitative signal; decide

### Cost

- Carrd Pro: $19/yr (or free tier OK — Pro adds custom domain)
- Domain planny.app: $12/yr (already in Week 1 GTM budget)
- ConvertKit free tier: $0 (under 1K subs)
- Optional Loom Pro for 90-sec demo: $0 (free tier sufficient)
- **Total: $0-50**

### TEMPLATES (Ready to Use)

#### Landing Page Copy Outline

```
[Hero Section]
Your week, voiced.

The AI weekly planner built by an ADHD adult, for ADHD adults.

- Voice brain-dump → realistic week in 60 seconds
- Two-way sync with Google + Apple Calendar
- No streaks. No red dots of shame.
- 30-day refund if it doesn't work. Cancel in two taps.

Coming late June 2026.

[Email Capture Form]
Join the waitlist — first 100 get 50% off year one.
[email field] [Join button]

---

[Founder Section — photo + ADHD disclosure]
Hi. I'm Afek.

I built Planny because Tiimo broke my brain at week 2 of setup, Motion is built for executives, and Sunsama won't let me plan from my phone.

I have ADHD. Late-diagnosed. Like a lot of you, probably.

So I made the planner I wanted. Voice it, don't type it. Weekly, not daily. Mobile-first. No shame UI.

If it works for you, great. If it doesn't, 30-day refund, no questions, no co-founder emailing you to take down your review.

---

[Social Proof — populate once available]
"Tiimo doesn't sync both ways with Google. Planny does." — [first beta user, July]
"Finally a planner that doesn't punish me for being ADHD." — [r/ADHDWomen DM]

---

[FAQ]
**When does Planny launch?** Late June / early July 2026, right after Apple WWDC.

**How much?** $9.99/mo, $39.99 for 6 months, $59.99 for a year. 14-day free trial on annual. 30-day refund, no questions.

**Who is it for?** Adults with ADHD who want a realistic weekly plan, not a 47-app stack. Especially women who got diagnosed in their 20s, 30s, or later.

**Is it iOS or Android?** iOS first. Android in year two.

**Do you have ADHD?** Yes. Late-diagnosed. Built this for me first.

**What if it doesn't work for me?** 30-day refund, two-tap cancel from settings. That's the whole promise.

---

[Footer]
Made by Afek (@plannyapp on Twitter / TikTok).
Email: hello@planny.app
```

#### r/ADHDWomen Post Template (NOT promotional — link in bio only)

```
Title: How do you actually plan your week with ADHD? Building something and want to learn what's already working.

Body:
Hi friends —

I'm building a weekly planner specifically for ADHD adults. I have ADHD too — late-diagnosed in my late twenties, made me cry, made me make this.

Before I launch I want to understand what's actually working for you right now — not what should work, not what looks pretty in screenshots, what you actually open on a Tuesday morning at 9am.

Three questions, answer any or all:

1. What do you currently use to plan your week? (Apple Reminders, paper, Tiimo, Sunsama, Notion, just survival mode?)
2. What's the #1 thing that's broken about every planner you've tried?
3. If a magic planner existed and was designed for your brain specifically, what would it do?

I'll DM the first 20 people who reply with a free year of access when we launch (no strings, just want feedback later).

Thank you in advance for the honesty — including the hard truths. Especially the hard truths.

— Afek
(I have ADHD. Link in my bio if you want to see what I'm building. Mods, happy to remove if not in line with rules.)
```

#### Micro-Creator DM Template (20 sends, personalized)

```
Hi [Name] —

I'm Afek. I have ADHD. I'm building Planny — a weekly planner where you voice your week in 60 seconds and the AI builds you a realistic plan. Two-way sync with Google and Apple Calendar. No streaks. By an ADHD adult, for ADHD adults.

I follow your [TikTok / podcast / Substack] and your [specific post — name it] hit me hard. I think your audience would actually get what I'm building.

We launch late June. Would you be open to a free year of access in exchange for an honest review — positive, critical, whatever you actually think? I'd rather hear "this isn't for me" than fake hype.

If yes, reply with your email and I'll send TestFlight access in 2-3 weeks.

If not, no worries — appreciate what you're doing for the community either way.

— Afek
@plannyapp
hello@planny.app
```

#### Twitter/X Poll Template

```
ADHD adults — which planner app are you actually using right now?

- Tiimo
- Sunsama
- Apple Reminders
- Paper / nothing

24-hour poll. Building something. Want to learn what's in use, not what gets recommended.

(I have ADHD. Late-dx. Replies welcome — especially "I gave up and use post-its.")
```

#### Twitter/X Context Tweet (paired with poll)

```
Building Planny — a weekly planner for late-diagnosed ADHD adults. Voice your week in 60 seconds. Two-way Google + Apple sync. No streaks.

By an ADHD adult, for ADHD adults.

Trying to understand what people actually use today before I tell anyone what they should switch to. Poll below.

planny.app
```

---

## EXPERIMENT 5: In-Person Coffee Conversations (US Trip)

### Hypothesis

**H5 (primary):** When Maya (late-diagnosed US ADHD woman 25-40) describes her current planning struggle in her own words, **≥7/10 her language will match the customer voice research** (verbatim language map — "washing machine", "setup overwhelm", "red dot of shame", "I felt like the failure"). When shown the Planny concept via 60-90-sec Loom demo, **≥6/10 will say "I would pay $9.99/mo OR $59.99/yr for this"** with audible conviction (not polite hedging).

**H5 invalidate:** <3/10 indicate genuine willingness to pay → fundamental hypothesis problem with either persona definition, price point, OR wedge → consider V1 Working Parents pivot per `mvp-definition.md` soft-kill criteria OR delay launch 4 weeks for repositioning.

**Sub-hypotheses:**
- **H5a:** ≥7/10 will identify voice brain-dump (not two-way sync, not refund, not no-streaks) as the lead "I'd switch for this" feature
- **H5b:** ≥5/10 will name Tiimo, Sunsama, OR Apple Reminders specifically as their app graveyard — confirms competitor framing in positioning is accurate, not invented
- **H5c:** ≥7/10 will respond to "by an ADHD adult, for ADHD adults" with visible recognition ("oh thank god", "finally", or similar) — validates founder credential as moat, not just feature

### Method

1. Once US trip dates locked (target month: July, ~5 weeks from today), post recruitment in r/ADHDWomen [city] or city-specific ADHD subreddit
2. Alternative recruitment: DM 20-30 city-local ADHD TikTok creators OR ask Tracy Otsuka for 2-3 community member intros (if Exp 4 succeeded)
3. Screen volunteers via 3-question DM: (a) When were you diagnosed? (b) Which planner apps have you tried? (c) Age + city — confirm Maya fit
4. Schedule 5-10 30-min coffees, batch in 2 days where possible
5. Bring printed consent form (recording disclosure) + Planny gift code as thank-you
6. Run structured interview (script below)
7. Transcribe + score within 24 hours

### Metrics

- **Primary:** % who indicate genuine willingness to pay $9.99/mo OR $59.99/yr (with conviction, not politeness)
- **Secondary:** Persona match accuracy score (1-10 per interview vs Maya profile in `target-audience.md`)
- **Tertiary:** Wedge resonance — which feature "lights them up" (Voice / Sync / Refund / Founder ADHD / No-streaks)
- **Qualitative:** 2-3 verbatim quotes per interview, usable as testimonials OR as language refinement signal

### Success Criteria

| Outcome | Threshold | Decision |
|---------|-----------|----------|
| **Validate** | ≥6/10 willing to pay + ≥7/10 persona match (Maya 7+/10) + ≥7/10 voice wedge resonance | Confirms positioning + price + wedge; proceed to launch with confidence; harvest quotes for landing page social proof |
| **Mixed** | 3-5/10 willing to pay OR persona match 4-6/10 | Continue but adjust — possibly lower price to $7.99/mo OR shift wedge framing OR tighten persona to "diagnosed 28+" specifically |
| **Invalidate** | <3/10 willing to pay OR persona match <4/10 | Pivot consideration: V1 Working Parents OR repositioning sprint (4-week delay) — do NOT launch on weak signal |

### Timeline

- **Month:** When in US (target July 2026)
- **Pre-trip (2 weeks before):** Post recruitment, screen volunteers, schedule
- **In-trip:** 30-45 min per interview + 10 min notes immediately after
- **Total in-trip founder time:** 6-10 hours over 1-2 days
- **Post-trip (1 week):** Transcribe, score, synthesize themes, update positioning if needed

### Cost

- Coffee tabs: $50-150 ($5-15 × 5-10 people)
- Travel within city: minimal (walking distance / public transit)
- Recording device: phone (free)
- Printed consent forms: $5 at FedEx
- Thank-you Planny gift codes: $0 (free access tokens)
- **Total: $50-200**

### TEMPLATES

#### Recruitment Post (r/ADHDWomen + city subreddit cross-post per rules)

```
Title: ADHD founder visiting [city] [dates] — buying coffee for 5-7 ADHD women willing to chat 30 min about planning apps. Not a sales pitch — listening.

Body:
Hi —

I'm Afek, an ADHD adult building a weekly planner app (by an ADHD adult, for ADHD adults). I'm visiting [city] from [start date] to [end date] and would love to learn from 5-7 local ADHD women.

What I'm asking:
- 30-min coffee chat (my treat — pick the spot)
- I'll ask about your current planning workflow + what's broken
- I'll show you what I'm building (60-sec demo)
- You tell me honestly if it solves a problem you have — or doesn't

Who I'm looking for:
- ADHD diagnosis (any time — but late-diagnosis especially welcome)
- Age 25-40
- You've tried at least 1-2 planner apps (Tiimo, Sunsama, Notion, Apple Reminders, anything)
- Based in [city] or commutable

Honesty is the gift. "This is useless to me" is more valuable than "yeah this is cool I guess."

DM me with your availability + which apps you've tried. First 5-7 confirmed get the coffee.

Thanks — Afek
(I have ADHD. Late-dx. Not selling anything to you specifically — just learning before I launch.)
```

#### DM Screening Template (3 questions before scheduling)

```
Hi [Name] — thanks for reaching out!

Three quick questions before we lock in a time (so I know I'm using your 30 min well):

1. When were you diagnosed with ADHD? (Ballpark age fine — just helps me know if you fit the persona I'm researching.)
2. Which planner apps have you tried in the past year? (Tiimo, Sunsama, Notion, Apple Reminders, paper, anything else?)
3. What city are you currently in, and are you 25-40?

If yes to all three, I'll send 2-3 time slots that work for me. Coffee shop of your choice — I'll buy.

— Afek
```

#### 30-Min Interview Script (Structured)

```
[0:00-0:05] Intro + Consent

"Hey [Name] — thanks for meeting me. I'm Afek.

I have ADHD too — diagnosed at [age]. I built [app name] because every planner I tried made me feel like the failure.

I'm recording this on my phone — voice only, just for my notes, won't be shared publicly. You okay with that? [Sign consent form.]

Couple ground rules:
- No right answers. I want what you actually think, not what's polite.
- 'I don't know' is a real answer.
- Critical feedback is the gift. I'd rather you say 'this is useless' now than write a 1-star review later.

Sound good? Cool. Let's start."

---

[0:05-0:15] Current State (open-ended — listen, don't lead)

Questions (ask in order, don't skip):

1. "Tell me about your week. How do you currently plan it — or do you?"
   [LET THEM TALK. Don't interrupt. Write down EXACT phrases.]

2. "What worked this week? What broke?"

3. "Walk me through the last planner app you tried. What made you download it? What made you delete it?"

4. "If you could wave a magic wand and have any tool you wanted for planning your week — what would it do?"

[LISTENING TIPS:
- Don't fill silence — let them think
- When they say "ADHD-friendly" or similar cliché, ask "what does that mean to you specifically?"
- Write down VERBATIM phrases — not paraphrased
- Watch for emotional words: "shame", "failure", "exhausted", "give up", "useless"]

---

[0:15-0:20] Pain Drill-Down (specific incident, not abstract)

"When you said [their exact phrase, e.g. 'I just gave up on Tiimo'] — can you describe a specific time that happened? Like, what day was it? Where were you? What did you do next?"

[GOAL: one concrete pain story they can recall in detail. This is the gold — abstract pain is uninteresting, specific pain is testimonials.]

Follow-ups:
- "What did you wish had happened instead?"
- "What did you do as a workaround?"
- "How long until you tried the next app?"

---

[0:20-0:27] Demo + Reaction (60-90 sec Loom on phone)

"Okay — I want to show you what I built. 60 seconds. Just watch, then tell me what you think — no need to be nice."

[Show Loom OR live phone demo of: voice brain-dump → AI weekly plan → calendar view]

[WATCH THEIR FACE. Note when they:
- Lean forward
- Smile
- Frown
- Pull out their own phone (highest-intent signal)
- Say "wait, what?" (confusion = friction point)]

After demo, ask in this order:

1. "First reaction — be honest. What do you think?"
2. "What part, if any, solved a problem you have?"
3. "What part felt off or confusing?"
4. "If I gave you this app today, would you pay $9.99/month for it? Why or why not?"
5. "What if it was $59 for a year — would that change your answer?"
6. "What would I have to change for you to pay full year up front?"

[CRITICAL: For pricing question, watch their FACE not just their words. "Yes" with a flinch = not really yes. "Hmm, maybe" with a lean-in = real interest.]

---

[0:27-0:30] Wrap

1. "Most surprising thing about what I showed you?"
2. "Anything I should have asked but didn't?"
3. "Can I follow up with TestFlight beta access when it's ready in 2-3 weeks?"
4. "Would you be willing to share your honest reaction publicly once you've used it — even if critical?"

"Thanks so much. I'll send a calendar invite for TestFlight + your free year code by Friday."

[Pay tab. Walk out. Don't keep talking — let them go.]

---

[0:30-0:40] Immediate Notes (within 10 min, while fresh)

Capture in phone notes or notebook BEFORE you do anything else:

- Verbatim quotes (3-5 best): ____
- Persona match (Maya 1-10): ____
- Willingness to pay $9.99/mo (1-10 with conviction, not just yes/no): ____
- Willingness to pay $59/yr (1-10): ____
- Wedge resonance — which lit them up? Voice / Sync / Refund / Founder-ADHD / No-streaks: ____
- Their #1 unmet need (in their words): ____
- One specific thing they'd change: ____
- Body language note (e.g. "leaned in at voice demo", "looked away at price"): ____
- Would they share publicly? Y/N: ____
- Follow-up sent? Y/N: ____
```

#### Post-Interview Data Capture (Google Sheet template)

| # | Date | City | Age | Dx age | Persona Match (1-10) | WTP $9.99/mo Y/N | WTP $59/yr Y/N | Voice (1-10) | Sync (1-10) | Refund (1-10) | Founder-ADHD (1-10) | Top quote | #1 change | Public share? |
|---|------|------|-----|--------|----------------------|-------------------|------------------|--------------|-------------|---------------|---------------------|-----------|-----------|---------------|
| 1 | 7/15 | NYC | 32 | 30 | 8 | Y | Y | 9 | 7 | 8 | 9 | "Voice it? Oh thank god, I can't type at 9am." | "Make the AI ask about my energy" | Y |
| 2 | 7/17 | NJ | 28 | 27 | 6 | N | Y | 7 | 9 | 6 | 8 | "Two-way sync would save my marriage" | "Lower price for monthly" | Maybe |
| ... | | | | | | | | | | | | | | |

**Aggregate at end:** persona match avg, WTP %, top 3 unmet needs, top 3 changes requested, top 5 quotes.

---

## EXPERIMENT 6: TestFlight Closed Beta

### Hypothesis

**H6 (primary):** Voice brain-dump → first weekly plan completion within **90 seconds** for **≥70% of TestFlight users**, **calendar connection (Google or Apple) within 7 days for ≥60%**, and **Day-7 return rate ≥40%** with **Day-14 NPS ≥30**.

**H6 invalidate:** <40% voice completion in first session OR <15% Day-7 return → onboarding flow needs rework BEFORE public launch; delay launch 1-2 weeks to iterate F1 (voice brain-dump) and F8 (onboarding).

**Sub-hypotheses:**
- **H6a:** Calendar-connected users will retain at Day-7 at ≥10 percentage points higher than non-connected (validates F4 sync as retention driver per `mvp-definition.md`)
- **H6b:** Voice transcription accuracy will hold ≥90% across cohort (test diverse accents if cohort allows — yellow flag per `mvp-definition.md`)
- **H6c:** Median time install → first plan generated ≤ 90 seconds (the Aha moment claim in positioning is empirically defensible)

### Method

1. Email waitlist subset (from Exp 1): "TestFlight slots opening. Reply if you want in." Pick 50-100 most-engaged respondents.
2. Send TestFlight invites in batches of 20 (manage support load).
3. Instrument analytics from day 1: PostHog or Mixpanel free tier.
4. Track funnel events (full list in template below).
5. Founder personal DM to every beta user week 1: "How's it going? Stuck anywhere?"
6. Day 14: in-app NPS survey (3 questions + 1 optional).
7. Day 21-28: cohort retention measurement (Day 7, Day 14).
8. Day 28-35: iterate based on funnel drop-offs + qualitative feedback.

### Metrics

- **Primary:** % voice brain-dump completion in first session (≥70%)
- **Secondary:** % calendar connection rate within 7 days (≥60%)
- **Tertiary:** Day-1 return rate, Day-7 return rate (≥30%), Day-14 return rate
- **Quality:** Day-14 NPS from beta cohort (≥30)
- **Funnel:** Drop-off points install → onboarding → voice → plan → calendar → return
- **Speed:** Median time install → first plan (≤90s)

### Success Criteria

| Outcome | Threshold | Decision |
|---------|-----------|----------|
| **Validate** | ≥60% voice completion + ≥50% calendar connect + ≥30% Day 7 return + NPS ≥30 | Launch June 22 with confidence; harvest top-NPS users as App Store launch-day reviewers |
| **Mixed** | 40-60% voice completion | Minor onboarding tweak; launch on schedule with v1.0.1 patch queued for Week 2 |
| **Invalidate** | <40% voice completion OR <15% Day-7 return | Onboarding rework BEFORE public launch; delay launch 1-2 weeks; iterate F1 + F8 |

### Timeline

- **Day 0:** Build TestFlight ready (1 week after Google OAuth approval — gating dependency)
- **Day 1-7:** First cohort batch (20 users) — close monitoring + DMs
- **Day 8-14:** Second + third batches (20 + 20 users)
- **Day 14:** NPS survey triggered for cohort 1
- **Day 21:** Cohort 1 Day-7 retention measurable
- **Day 28:** Cohort 1 Day-14 + cohort 2 Day-7 measurable
- **Day 30-35:** Analyze + iterate based on feedback
- **Total elapsed:** 4-5 weeks (overlaps with Exp 1 collection window)

### Cost

- TestFlight: Free (Apple)
- Mixpanel / PostHog: Free tier (under 100K events/mo)
- Typeform for NPS (or in-app modal): Free tier
- Loom for founder personal videos to beta users: Free tier
- **Total: $0**

### TEMPLATES

#### TestFlight Welcome Email

```
Subject: Planny TestFlight — you're in. Read this first (90 seconds).

Hey [Name] —

Thanks for being one of the first 50 to try Planny. Genuinely. This is the cohort that shapes v1.

Three things, then I'll get out of your way:

1. **Download TestFlight if you haven't:** [link]
2. **Install Planny:** [TestFlight invite link]
3. **First thing the app does:** asks you to voice your week. Just tap and hold the mic button. Talk for 30-60 seconds about your week — work stuff, life stuff, the thing you've been avoiding. Then let go. Watch what happens.

That's the Aha moment I'm testing. Either it lands or it doesn't. I want to know either way.

What I'm specifically watching for:
- Did the voice brain-dump feel natural — or weird?
- Did you connect your Google or Apple Calendar? Did it work?
- Did you come back on Day 2 or Day 3 without me poking you?

If you have 15 min for a Zoom this week to walk me through what's working and what's broken, reply YES and I'll send a Calendly. Free year of Planny when we launch, regardless.

If something breaks — please email me direct at founder@planny.app. I read every one. Usually replies same day.

Thanks for helping me build this right. Not just well — right.

— Afek
founder@planny.app
@plannyapp

P.S. If you decide it's not for you after 5 minutes, that's also useful data. Just reply with a sentence on what didn't click. No hard feelings.
```

#### Day-14 NPS Survey (in-app modal OR Typeform)

```
Hey [Name] — quick check-in. Two weeks in.

Six questions. Should take 3 min. No questions are required — skip anything.

1. On a scale of 0-10, how likely are you to recommend Planny to a friend with ADHD?
   [0 — definitely not] [1] [2] [3] [4] [5] [6] [7] [8] [9] [10 — definitely yes]

2. Why did you give that score? (open text — be honest)
   [____________]

3. What's the #1 thing you'd change about Planny right now?
   [____________]

4. Did you connect your calendar?
   [ ] Yes — Google
   [ ] Yes — Apple
   [ ] Tried but it failed
   [ ] No — didn't try

5. Have you used the voice brain-dump more than once?
   [ ] Yes — multiple times
   [ ] Yes — once
   [ ] No — I type instead
   [ ] No — never used it

6. Would you pay $59.99 for a year of Planny today?
   [ ] Yes
   [ ] No
   [ ] Maybe — depends on: ___________

7. Anything else I should know? (open text — totally optional)
   [____________]

Thanks for being in this with me.

— Afek

P.S. If you said "no, I would not pay" in Q6 — please tell me why. That's the most useful feedback you can give me right now. No defensiveness, no follow-up sales pitch. Just want to know what's broken.
```

#### Internal Funnel Tracking (Mixpanel / PostHog Events)

```
// Install + onboarding
event_install                          // Auto from App Store / TestFlight
event_onboarding_started               // First launch, first screen shown
event_onboarding_completed             // Reached main app view
event_mic_permission_requested
event_mic_permission_granted

// Voice brain-dump (the Aha moment)
event_voice_brain_dump_started         // tap-and-hold mic pressed
event_voice_brain_dump_completed       // released + transcription returned
event_voice_brain_dump_abandoned       // released early (<3s) or never released
event_transcription_received           // text returned from STT
event_first_plan_generated             // LLM response with weekly plan
event_first_plan_viewed                // user reached weekly view

// Calendar connection
event_calendar_connect_prompted
event_calendar_connect_google_started
event_calendar_connect_google_completed
event_calendar_connect_apple_started
event_calendar_connect_apple_completed
event_calendar_connect_failed          // log error type

// Notifications + first actions
event_notification_permission_requested
event_notification_permission_granted
event_first_task_added                 // any method
event_first_task_voiced                // voice quick-add specifically
event_first_task_typed                 // text entry

// Retention markers
event_day_1_return                     // 18-30 hrs since first session
event_day_3_return                     // 60-84 hrs
event_day_7_return                     // 144-192 hrs
event_day_14_return                    // 312-360 hrs
event_day_30_return                    // 696-744 hrs

// Monetization
event_paywall_viewed
event_trial_started                    // annual only per pricing-strategy
event_trial_converted                  // trial → paid
event_subscription_purchased           // direct purchase (monthly / 6mo)
event_refund_requested
event_subscription_cancelled

// Survey
event_nps_survey_shown
event_nps_survey_submitted             // include score as property
event_nps_promoter_followup_sent       // for 9-10 scorers

// Properties to attach (set globally per user):
- acquisition_source (waitlist / asa / podcast / reddit / dm / organic)
- cohort_week (date of install rounded to week)
- diagnosis_age_bucket (if collected: <25 / 25-30 / 30-35 / 35+ / unknown)
- voice_completed_first_session (boolean)
- calendar_connected_d7 (boolean)
```

#### Founder Personal Week-1 DM Template (per beta user)

```
Hey [Name] —

Day [X] of your Planny beta. Quick check — anything broken yet? Confused? Want to throw your phone?

The 2 things I'm specifically curious about:
1. Did the voice brain-dump feel okay, or weird?
2. Did the calendar sync work for you?

15 sec reply is plenty — even just "fine" or "broken" tells me what I need to know.

— Afek

(If you want to do a 15-min Zoom this week to walk me through it live, reply with "yes" and I'll send a Calendly. Otherwise no pressure.)
```

#### Day-14 NPS Promoter Follow-Up DM (for 9-10 scorers)

```
Hey [Name] —

You gave Planny a [9/10 or 10/10] on the NPS survey — thank you. That means a lot.

Two asks, both totally optional:

1. **Would you share your Planny experience publicly?** A tweet, a TikTok, an App Store review when we launch, a r/ADHDWomen comment when someone asks "what planner do you use?" — whatever feels natural. I'd love a quote I can use too if you're game.

2. **Mind if I send you a TestFlight build of a new feature in 2-3 weeks for early eyes?** You're exactly the user I want feedback from.

No pressure on either. Just grateful you're here.

— Afek
```

---

## Cross-Experiment Learnings Plan

After all 3 experiments complete (~6 weeks), consolidate findings into a single GO/NO-GO scorecard:

| Experiment | Primary Learning | Feeds Into |
|------------|------------------|------------|
| 1 Waitlist | Demand exists? At what price? Which channels deliver Maya specifically? | GTM channel allocation; ASA bidding strategy (Exp 8); waitlist → TestFlight recruitment pool (Exp 6) |
| 5 Coffee chats | Maya persona accuracy? Wedge resonance? Pricing acceptance? Verbatim language refinement? | Positioning copy refinement; landing page social proof; testimonial harvest; pricing structure confirmation (Exp 7) |
| 6 TestFlight | Aha moment delivers <90s? Onboarding works? Retention floor realistic vs 4.1% productivity benchmark? | Launch GO/NO-GO decision; D30 retention hypothesis (Exp 11 post-launch); paywall A/B (Exp 7) |

**Decision matrix:**

| Outcome | Action |
|---------|--------|
| **All 3 validate (GREEN)** | Launch June 22 as planned. Confident proceed to Exp 8 (ASA) + Exp 9 (Tracy podcast). |
| **2 validate, 1 mixed (YELLOW)** | Launch June 22 with explicit adjustments per mixed outcome. Reduce paid spend by 50% pending Week 2 cohort data. |
| **2 validate, 1 invalidate (YELLOW-RED)** | Delay launch 1-2 weeks for targeted fix to invalidated experiment. Do not proceed to Exp 8-10 yet. |
| **1 validate, 2 invalidate (RED)** | Pause launch. 4-week repositioning sprint OR pivot to V1 Working Parents per `mvp-definition.md` soft-kill. |
| **0 validate (HARD RED)** | Hard kill consideration. Return remaining cash. Founder retrospective before next project. |

---

## Founder Time Allocation

| Experiment | Total Founder Time | Per-Week Breakdown |
|------------|-------------------|---------------------|
| 1 Waitlist | 8-12 hours over 3 weeks | 3-4 hr/wk (setup Day 1-2, then 2-3 hr/wk replies + monitoring) |
| 5 Coffee chats | 6-10 hours over 1-2 weeks (in US) | Concentrated: 2 hr recruiting pre-trip + 5-8 hr in-trip + 2 hr post-trip transcription |
| 6 TestFlight | 8-12 hours over 4-5 weeks | 2 hr setup + 1-2 hr/wk monitoring + 2 hr Day-14 NPS analysis + 2 hr iteration planning |

**Total founder time for top 3 experiments: ~25-35 hours over 6-10 weeks.**

This is achievable within the 5% measurement allocation per `go-to-market.md` time table — but **only if founder commits to it**. The single most common failure mode in solo-founder validation is starting Exp 1, getting busy with engineering, and skipping Exp 5 + Exp 6 because they require "people work" that feels less productive than coding. Per the playbook's R1 flag: **without execution, validation is theater.**

---

## Strategic Connections

- ראה `validation-playbook.md` ל-full experiment list (13 experiments, sequenced funnel)
- ראה `assumptions-tracker.md` (TBD) ל-mapped assumptions per experiment + cross-reference
- ראה `kill-criteria.md` (TBD) ל-decision thresholds + scenario triggers per stage
- ראה `scorecard.md` (TBD) ל-final integration + Y1 review framework
- ראה `../02-strategy/positioning.md` ל-banned vocabulary + onliness statement (templates align with these)
- ראה `../03-brand/tone-of-voice.md` ל-4 pillars (Honest/Calm/Real/Capable) + reading-level 7 (templates follow these rules)
- ראה `../04-product/mvp-definition.md` ל-F1-F10 features + success criteria mapped to TestFlight events
- ראה `../05-financial/projections.md` ל-D30 retention as #1 sensitivity variable (informs Exp 6 → Exp 11 handoff)
- ראה `../02-strategy/go-to-market.md` ל-90-day channel calendar that experiments integrate with

---

## Sources

### Internal Phase Documents
- `/home/user/NEW-_PROJECT/startup-validation/06-validation/validation-playbook.md` — source of all 3 experiments (Exp 1, Exp 5, Exp 6 selected from 13)
- `/home/user/NEW-_PROJECT/startup-validation/02-strategy/positioning.md` — landing page copy + interview script language aligned to onliness statement, persona narrowing, banned vocabulary
- `/home/user/NEW-_PROJECT/startup-validation/03-brand/tone-of-voice.md` — all templates follow 4 pillars (Honest/Calm/Real/Capable), reading-level 7, em-dash-friendly, founder-signed
- `/home/user/NEW-_PROJECT/startup-validation/04-product/mvp-definition.md` — F1 (voice brain-dump), F4 (calendar sync), F8 (onboarding) success criteria mapped to TestFlight events
- `/home/user/NEW-_PROJECT/startup-validation/05-financial/projections.md` — D30 retention sensitivity (informs Exp 6 NPS + retention thresholds)
- `/home/user/NEW-_PROJECT/startup-validation/01-discovery/target-audience.md` — Maya persona (informs Exp 5 screening + scoring)
- `/home/user/NEW-_PROJECT/startup-validation/01-discovery/raw/customer-voice.md` — verbatim language map (informs Exp 5 listening prompts + scoring)

### External Tools + Benchmarks
- [Carrd](https://carrd.co/) — landing page builder, $19/yr Pro tier
- [ConvertKit](https://convertkit.com/pricing) — free tier <1,000 subscribers
- [Mixpanel free tier](https://mixpanel.com/pricing/) — 100K monthly events
- [PostHog free tier](https://posthog.com/pricing) — alternative analytics
- [Apple TestFlight](https://developer.apple.com/testflight/) — closed beta best practices
- [Loom free tier](https://www.loom.com/pricing) — demo video recording
- [Typeform free tier](https://www.typeform.com/pricing/) — NPS survey
- [Reddit r/ADHDWomen mod rules](https://www.reddit.com/r/ADHDWomen/about/rules/) — referenced for Exp 1 + Exp 5 recruitment posts

### Frameworks
- Steve Blank — *The Four Steps to the Epiphany* (customer discovery interview structure underlying Exp 5 script)
- Rob Fitzpatrick — *The Mom Test* (Exp 5 listening principles — specific past behavior over hypothetical future)
- Eric Ries — *The Lean Startup* (validate-or-invalidate kill criteria across all 3 experiments)
- April Dunford — *Obviously Awesome* (positioning language used in Exp 1 landing copy)

---

## Flags

### Red Flags

- **R1 — Experiment 5 (in-person interviews) requires founder discipline + willingness to hear hard truths.** This is the experiment most likely to be skipped under "I'm too busy with engineering" pressure. Per the playbook R1 flag: without execution, validation is theater. **Founder commitment required pre-trip — block calendar now.**

- **R2 — Experiment 6 (TestFlight) requires functional product + Google OAuth approval.** Google OAuth verification can take 4-6 weeks; if not started by Week 1 of validation, TestFlight launch slips and breaks the 6-week timeline. **Critical dependency — start OAuth submission today.**

- **R3 — Experiment 5 US trip is single-window, non-recurring.** If trip is delayed/cancelled, Exp 5 becomes non-runnable for ~6 months. No remote substitute equivalent. **If trip slips >2 weeks, run as Zoom interviews with reduced signal weight (persona match scoring becomes harder without in-person body language).**

- **R4 — All 3 experiments depend on founder execution.** Solo-founder bandwidth = single point of failure. If founder runs Exp 1 well but skips Exp 5 + Exp 6, launch proceeds blind on persona accuracy and product readiness. **Tracking commitment: founder must self-report weekly progress to a peer / advisor; no progress = pause launch.**

- **R5 — WWDC June 8 is a binary risk event during Exp 1 window.** If Apple announces ADHD-aware AI scheduler, Exp 1 results may already be invalidated by Day 11. **Mitigation: monitor WWDC live; pre-build messaging Variant B (Apple-Intelligence-coexist) and Variant C (pivot to "ADHD layer on top of Apple Intelligence") per `go-to-market.md`.**

### Yellow Flags

- **Y1 — Experiment 1 (Reddit value post) sensitive to mod rules.** Single self-promo violation = permanent ban from r/ADHDWomen (THE highest-density Maya channel). Founder must read mod rules carefully + post zero links in post body (bio link only).

- **Y2 — Experiment 5 recruitment may yield <5 volunteers** in some cities. Backup: DM 20-30 ADHD TikTok creators in city + ask Tracy Otsuka for 2-3 intros (if Exp 4 succeeded per playbook). Plan recruitment 2 weeks before trip, not last-minute.

- **Y3 — Experiment 6 TestFlight cohort is highest-intent waitlist users, not representative of cold acquisition.** D7 retention from beta may overstate D7 from ASA/podcast cohorts. **Account for selection bias: treat beta retention as upper bound, not point estimate, when projecting to launch cohort.**

- **Y4 — Voice transcription accuracy must be tested across accents** (yellow flag from `mvp-definition.md`). If beta cohort is 100% native-English-speaking white women, that's not the launch audience. **Try to recruit 2-3 AAVE/accented English speakers explicitly during TestFlight Batch 2 or 3.**

- **Y5 — Landing page conversion benchmarks are persona-dependent.** "2% organic" is industry-typical but ADHD audience may have higher (community-bonded) OR lower (subscription-fatigued) baseline. **Treat first week as calibration; adjust threshold if needed by Day 10 — but only down, not up.**

- **Y6 — Founder Twitter cold-channel conversion will be weak** until Twitter audience is warmed up (per playbook Exp 2 invalidate condition). Most Exp 1 conversion will come from r/ADHDWomen + DMs, not Twitter. **Set expectations: Twitter is for poll signal + social proof, not for waitlist conversion volume.**

- **Y7 — TestFlight NPS sample size depends on Day-14 survivors.** If <30 users remain at Day 14, NPS is directionally indicative only, not statistically significant. **Need 50+ Day-14 active users for meaningful NPS — that's why batch size targets 50-100 install minimum.**

- **Y8 — Coffee chat WTP signal is verbal, not behavioral.** People say "I'd pay" in person more often than they actually pay. **Discount WTP claims by 30-40% when projecting to actual conversion. Real validation comes at Exp 6 paywall + post-launch.**
