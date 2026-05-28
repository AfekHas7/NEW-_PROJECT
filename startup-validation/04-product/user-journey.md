# User Journey — Planny (Maya)

**Phase:** Phase 6 — Product (User Journey)
**Project:** startup-validation (Planny)
**Date:** 2026-05-28
**Confidence:** Medium-High — ה-journey מבוסס על persona Maya המאומתת ב-`01-discovery/target-audience.md` (35+ ציטוטים verbatim, decision-cycle V-shape יום 0-1 או יום 13-14, מסלול awareness→trial 1-7 ימים), על Aha moment שהוגדר במפורש ("render her chaotic week back in <60 seconds without setup"), ועל microcopy rules ב-`03-brand/tone-of-voice.md`. אי-ודאות: (1) `mvp-definition.md` עדיין לא קיים — features F1-F10 שאוזכרו במשימה הומרו לרשימה מתוקפת מ-`02-strategy/value-proposition.md` (15 must-haves + 6 nice-to-haves); (2) זמני שלב מדויקים ב-screens (5/30/3/15/10/5 sec) הם אומדן UX, לא נתוני telemetry; (3) Apple WWDC ב-8 ביוני (10 ימים מהיום) עלול לשנות את ה-onboarding flow אם Apple שולחת voice→calendar ב-iOS 27.

---

## תקציר

Maya עוברת מ-awareness ל-loyal user דרך 7 שלבים שהמשותף להם הוא מאבק יחיד: "אל תיתן לי להרגיש כמו failure עוד פעם". ה-journey מתחיל ב-TikTok / Tracy Otsuka podcast / r/ADHDWomen ומסתיים — אם הכל עובד — ב-365 ימים אחר כך כששוב חוייבה ב-$59 (annual) בלי לדחות, וכשהיא מספרת על Planny ל-3 חברות. בין לבין יש שלושה drop-off cliffs מסכני-קיום: **(1) ה-90 שניות הראשונות מההורדה** — אם voice→week לא מתרנדר מתחת ל-60 שניות, churn 70%+ (מאומת ב-`target-audience.md`); **(2) Day 13-14 trial decision window** — V-shape conversion שמכריע אם annual נסגר; **(3) Day 30-60 retention** — אם Maya לא פתחה במשך 14 ימים, היא תבטל (אם תזכור), או — גרוע יותר אתית — תשאיר את ה-subscription כ-"ADHD tax" שלנו.

**ה-Aha Moment הוא Step 4 ב-onboarding:** Maya מקליטה 20-45 שניות של דיבור כאוטי על השבוע שלה, רואה pulse של "Thinking with you...", ואז השבוע מופיע מתרחב על המסך — עם המשימות מפוזרות לפי ימים, buffers, ו-"first thing" מודגש. **התחושה היחידה שיש למדוד היא**: "מישהו עשה את ה-executive function עבורי". אם זה לא קורה ב-session הראשון, כל ה-funnel נופל. כל יתר ה-journey — push notifications gentle, weekly voice check-in, partner mode, refund flow — בנוי לשמור את אותה הבטחה: **לעולם לא ליצור bushה, לעולם לא להכריח דיוק, ולעולם לא לחסום את הביטול**. ה-anti-positioning מול Tiimo (visual setup-heavy), Inflow (clinical + cancellation traps), ו-Motion (executive performance) לא רק חי ב-marketing — הוא חי בכל touchpoint של ה-journey הזה.

הסיכונים הגדולים בסדר חומרה: (א) ה-voice→plan pipeline נופל מתחת ל-90 שניות median ב-real-world latency (LLM + transcription + UI render); (ב) WWDC ב-8 ביוני מציגה voice→calendar native ו-Maya תוהה למה לשלם $9.99; (ג) ה-Day 5 honest "still using?" message מוריד conversion ב-5-10% — נחושים שזה brand cost שווה; (ד) founder voice ב-touchpoints מסוימים (push notifications) עלול להרגיש bait-and-switch כשהאפליקציה עוברת ל-"we" — תורגם לכללי dual-voice ברורים בהמשך.

---

## Journey Phases

### Phase 1: Awareness (Day -30 עד Day 0 — לפני הורדה)

**Trigger context:** Maya קרסה ב-Sunday night. פתחה TikTok ב-11:47pm ב-doom-scroll, אחרי שלא הצליחה לסגור את הציור של השבוע הבא בראש שלה ("washing machine of thoughts"). אחת מהאפשרויות הבאות קורית:

- **Path A — TikTok organic:** רואה reel של Afek (60 שניות, founder POV) שמספר על Tiimo שכבה לו את המוח ב-week 2. או creator mid-tier (50K-300K) שעם annual חינמי שעשתה brain-dump.
- **Path B — Tracy Otsuka podcast:** סופ"ש מקשיבה ל-"ADHD for Smart Ass Women" ושומעת host-read של 60-90 שניות.
- **Path C — r/ADHDWomen:** ב-Reddit thread "what actually helps?" מישהי כותבת "I just downloaded Planny — voice your week thing. First app I didn't quit in week 1."
- **Path D — ADDitude newsletter sponsorship slot** — open rate 40%, sponsorship slot ראשון בליסט.
- **Path E — חברה / אחות / מטפלת המליצה.** Highest-trust path, lowest volume.

**Touchpoints:**

- TikTok reel (founder POV, 30-60 sec, captions on, hook in first 1.2 sec)
- Tracy Otsuka host-read midroll ad
- r/ADHDWomen thread comment (Afek כ-`u/afek_planny`, disclosed)
- ADDitude newsletter sponsorship + co-branded "what late-diagnosed women actually need" piece
- Friend DM screenshot of Planny home screen
- App Store search "ADHD planner" / "ADHD weekly schedule"
- Apple Search Ads brand defensive + long-tail "ADHD weekly schedule"

**Emotions (ranked by likelihood):**

- **Skeptical** ("another planner that won't work") — 100% present, default state
- **Subscription-fatigued** ("I have 30 of these already") — verbatim Maya language
- **Curious** ("voice my week? interesting") — 60-70% if hook lands
- **Hopeful** ("maybe THIS one") — 20-30%, fragile
- **Late-diagnosis-grief activated** ("why didn't I have this when I was 22") — if Afek's late-dx-at-28 disclosure surfaces
- **Pre-shame** ("I'll download it and forget it like the others") — 80% present

**Drop-off Risks:**

- TikTok thumb-scroll past in 1.5 sec — hook didn't land → bounce
- Tracy Otsuka ad sounds like generic productivity pitch → tune out
- r/ADHDWomen thread reader sees ad-spam vibes → downvote, brand burn on persona-critical sub
- App Store tap reveals $9.99/mo subscription → sticker shock, exit
- Privacy nutrition label shows "Data Used to Track You" → close (Maya post-Cambridge-Analytica)
- "In-App Purchases" warning → assumes paywall everywhere

**Mitigation:**

- TikTok hook: **"POV: your fifth planner this year"** (meme-aware, persona-fluent — `tone-of-voice.md` line 415)
- Tracy Otsuka ad copy leads with **"I built this because I couldn't use any of the planners you've tried"** — founder personal, not product
- App Store first screenshot headline: **"Voice your week in 60 seconds. Built by an ADHD adult, for ADHD adults."** (verbatim from `tone-of-voice.md`)
- App Store second screenshot: **"14-day free trial on annual. 30-day refund. Cancel in 2 taps."** — addresses 3 top objections in one card
- Privacy nutrition label engineered to show **"Data Not Linked to You"** category by category
- App Store description opens with **"Made by an ADHD adult who got tired of planners that punished him for being one."** (verbatim from `tone-of-voice.md` line 154)
- Reddit: zero promotion, only **"I have ADHD too — happy to answer Qs if useful"** replies; AMA scheduled for week 2 of launch

**KPIs for Phase 1:**

- TikTok hook retention ≥50% at 3 sec (industry benchmark for D2C apps)
- Tracy Otsuka attributed installs ≥150 per episode (at $800-1,500 spend)
- App Store conversion rate (impressions → installs) ≥35% (Apple median is 25-30%; persona-tuned screenshots should beat)

---

### Phase 2: Discovery → Install (Day 0)

**Trigger:** Maya הקישה "Get" ב-App Store. כעת היא מחכה 4-12 שניות לתחילת ההורדה, מסתכלת בעניינים אחרים, אולי קוראת עוד 2 reviews.

**Touchpoints:**

- App Store listing (5-7 screenshots + 30-sec video preview)
- App Store reviews block (target ≥4.5 stars from day 1, seeded by 20+ beta testers from r/ADHDWomen)
- Privacy nutrition label
- "Developer Response" replies (signed `— Afek`, per `tone-of-voice.md` line 412)
- App icon on home screen (post-download)

**Emotions:**

- **Cautious optimism** ("the screenshots looked honest")
- **Anticipatory subscription guilt** ("I shouldn't be downloading another one")
- **Self-doubt** ("will I actually use it this time?")
- **Pre-emptive relief** at refund promise ("at least I can get my money back")
- **Slight curiosity-spike** when seeing founder photo

**Drop-off Risks:**

- "In-app purchases" warning re-triggers subscription fatigue → close pre-install
- Review reader hits a 1-star "billing trap" review → exit (Inflow PTSD — verbatim concern from `target-audience.md`)
- Privacy label shows tracking → close
- Download stalls / fails → loses moment of impulse (Maya decisions are 1-7 days but execution is 1-second; lose the second, lose the install)
- App icon downloaded but never tapped → silent abandonment (object permanence risk starts pre-onboarding)

**Mitigation:**

- App Store reviews seeded pre-launch: 20+ beta testers from r/ADHDWomen briefed to write honest, specific reviews (not 5-star spam; 4.5-5.0 with specifics is more credible)
- Every negative review gets a signed reply from Afek within 24 hours: **"Thanks for the report — Afek"** (`tone-of-voice.md` line 412)
- App Store description opens with founder-voice paragraph + immediate refund promise (`tone-of-voice.md` line 154)
- **Post-install push within 8 minutes:** none — first push must come from inside the app after user opens it. Premature push burns trust.
- App icon design: clean, non-clinical, doesn't scream "ADHD app" (avoid the Tiimo "kid-coded" pattern flagged in `target-audience.md`)

**KPIs for Phase 2:**

- App Store install-to-open rate ≥75% within 24 hours (industry median 60-65%)
- Review baseline ≥4.5 stars on day 1 (seeded), maintained ≥4.5 in week 1
- Privacy nutrition label engineered to "Data Not Linked to You" — no tracking categories

---

### Phase 3: Onboarding (First 60-90 Seconds — THE AHA MOMENT)

**Trigger:** Maya tapped the Planny icon. App opens. The clock starts. **Internal SLA: voice-to-first-plan ≤75 seconds median** (`value-proposition.md` line 404). Promise to user: 60 seconds. Buffer of 15 seconds for the 90-second copy claim.

**Screen-by-screen (English microcopy — user-facing strings):**

#### Screen 1: Welcome / Founder intro (target 5-8 sec)

```
[Founder photo of Afek — natural, non-corporate]

Hi. I'm Afek.

I built Planny because Tiimo broke my brain at week 2
and Motion is built for executives.

Want to plan your week in 60 seconds?
Tap and hold the button below — tell me what's going on this week.

Don't organize it. Just say it.

[Tap-and-hold mic button]
[Skip — I'll type instead]
```

*(Verbatim from `tone-of-voice.md` line 167. Note: NO "Welcome to Planny!" / "Let's get you set up" pattern — that is the explicit `NOT Planny` anti-pattern at line 177.)*

#### Screen 2: Voice permission prompt (target 3 sec)

iOS native dialog precedes; before showing it, Planny preempts with context:

```
We use voice only to plan your week. We don't store recordings.
The text stays on your device until you tap "Save week."

[Continue → iOS permission dialog]
```

*(This preempts the iOS denial spiral. Maya is post-Cambridge-Analytica; bare iOS dialog feels intrusive.)*

#### Screen 3: Voice brain-dump (target 20-45 sec — Maya's actual speech time)

```
[Big circle in center, slow pulse animation]

Hold to talk. Release when you're done.

[Below, smaller:]
Things like: "I have a dentist Wednesday at 10,
mom called about Sunday, three meetings Thursday,
want to start that book club..."
```

Maya speaks. As she speaks, a soft waveform animates. NO transcript appears in real-time (would induce self-editing and break flow — ADHD brains will start cleaning up their words).

#### Screen 4: Processing (target 3-5 sec)

```
Thinking with you...

[Subtle 3-dot pulse. No spinner. No "AI working" copy. No progress bar.]
```

*("Thinking with you" — not "AI processing", not "Analyzing your input". The verb is collaborative, calm, peer-voice. Banned: "Our AI is...", "Algorithm running...".)*

#### Screen 5: First plan reveal — **THE AHA MOMENT** (target 10-15 sec)

```
Here's your week. Move anything.

[Week view appears with soft entrance animation —
items fade in sequentially over 1.2 sec, Mon→Sun.]

[Items are auto-placed with:
- Buffers around appointments (time-blindness aware)
- "First thing" tag on Monday morning item
- Confidence indicator (small dot) on items the AI inferred —
  tap to confirm or correct]
```

**This is the Aha.** Maya sees her chaotic spoken week now visible, structured, on her phone. The internal monologue Planny is engineering for: *"Someone did the executive function for me."*

**Critical UX rules at this moment:**

- NO modal popup blocking the reveal
- NO "Tap here to learn more" overlay
- NO confetti / streak celebration (banned per `tone-of-voice.md`)
- NO "great job!" copy (rescuer dynamic, banned per Trait 4 Capable)
- Just the week, visible, hers, editable

#### Screen 6: Calendar connect prompt (target 5-8 sec, OPTIONAL)

After Maya has had ~10 seconds to look at her week:

```
Two-way sync with Google or Apple Calendar?
Means edits here update there — and back.

[Connect Apple Calendar]
[Connect Google Calendar]
[Skip for now — I can do this later]
```

*(NOT a modal. Inline card at top of week view. Skip is visually equal weight to Connect — not greyed-out. Two-way sync is the wedge vs Tiimo, per `value-proposition.md` line 90.)*

#### Screen 7: Notifications opt-in (target 3-5 sec, OPTIONAL, LAST)

Only after Maya has interacted with the week (moved an item, tapped one to expand, or 30 seconds elapsed):

```
Want gentle reminders?

You can turn them off anytime. No daily summary spam.
First thing tomorrow + one evening check — that's the default.

[Sure, gentle is fine]
[Not now — I'll come back to this]
```

*(Last because of compounding ask-fatigue. Permission-strategy: voice → calendar → notifications, in order of decreasing trust-cost. Per Trait 4: Maya knows herself; we don't push.)*

#### Screen 8: First plan complete (target 0 sec — implicit)

Maya is now in the app, looking at her week. The onboarding has no completion screen. No "You're all set!" No "Welcome aboard!" The week IS the welcome.

---

**Emotions through the 60-90 seconds:**

- Screen 1: **Relief** at founder face + ADHD disclosure ("oh, he gets it") + **slight wariness** ("but is this just marketing?")
- Screen 2-3: **Surprise** at voice-only ask ("no forms?") + **mild discomfort** speaking out loud ("I feel weird talking to my phone")
- Screen 4: **Tense hope** ("please be good please be good")
- Screen 5: **AHA** — relief, surprise, a small involuntary inhale, the thought *"oh."*
- Screen 6: **Trust extension** ("okay I'll give it Apple Cal access") OR **defensive skip** ("not yet")
- Screen 7: **Boundary-setting** ("gentle is fine") OR **declined** ("not yet")
- Final: **Cautious excitement** + **already-mourning** ("I'll probably stop using this in 3 weeks") — the pre-emptive grief is Maya's default

**Drop-off Risks (ranked by severity):**

1. **Voice permission denied (15-25% of users).** Blocks Screen 3 entirely. → Mitigation: text input ALWAYS available via "Skip — I'll type instead" on Screen 1. Text-flow renders same Aha at Screen 5, ~30 sec slower.
2. **Voice transcription fails / Maya's accent or AAVE not handled (5-10%, demographic-skewed).** → Mitigation: diverse beta testing (`value-proposition.md` line 417); text-fallback one tap away; confidence indicators on parsed items so low-confidence ones are visibly editable.
3. **Maya speaks for >60 sec, AI gets confused.** → Mitigation: at 60 sec recording, gentle "I have enough to start — tap to continue or keep going" prompt. NO hard cutoff.
4. **AI parses incorrectly (wrong day, wrong time, mishears a name).** → Frustration → "this is broken" exit. → Mitigation: confidence dots on low-confidence items; tap to confirm/correct; **honest copy: "Sometimes the AI plans too much. Tap and slide to fix."** (`tone-of-voice.md` line 28)
5. **Calendar connect feels like a sales push.** → Skipped. → That's OK — re-offer at Day 3 once value is established.
6. **Notifications opt-in feels intrusive at end of onboarding.** → Declined. → OK; re-offer at Day 2 with context: "You said yes to gentle reminders — want to turn them on now?"
7. **Maya gets a phone call mid-onboarding / context-switches.** → Returns to app cold, doesn't remember where she was. → Mitigation: state-preservation; cold-open returns to the last screen with **"You were saying... [first 5 words of transcript]. Continue?"**
8. **First plan looks wrong** (e.g., she mentioned "Thursday meetings" and they got placed on Wednesday). → Aha breaks. → Mitigation: every item has 1-tap edit; confidence indicators visible; AI is calibrated to under-place rather than over-place (better to leave items in inbox than wrong-slot them).
9. **Maya doesn't have time for full brain-dump.** → Closes app at Screen 3, never returns. → See "Aha Moment Backup" section below.

**Mitigation summary:**

- Internal latency SLA: voice-end-to-plan-render ≤8 sec (target ≤5 sec)
- Voice permission preempt copy (`tone-of-voice.md` style)
- Text fallback always available, equal visual weight to mic
- Confidence indicators on every parsed item
- State preservation across interrupts
- ALL prompts after Screen 5 are OPTIONAL with visible skip

**The Aha Moment — defined:**

> Maya speaks 20-45 seconds about her week. Planny shows her week structured on the screen ≤8 seconds later. She sees her own chaos rendered back to her — with first-thing tagged, buffers added, days laid out — without having made a single setup decision. The internal feeling: *"Someone did the executive function for me."*

**Why THIS is the Aha (not "weekly review" or "partner mode"):**

- Solves Pain #1 (Setup overwhelm — "downloaded 30 apps, abandoned 28") in 60 seconds. The pain Maya has never had solved by any planner.
- Demonstrates voice-first capability — the wedge vs every competitor (Tiimo, Sunsama, Motion, Inflow all require multi-screen typed setup).
- Shows AI competence without LLM-hype copy. The output IS the evidence.
- Differentiates from Apple Intelligence (whenever WWDC ships) — Planny's Aha is ADHD-tuned (buffers, energy-awareness, first-thing tag), not generic schedule-fill.
- It's the only Aha that can happen on Day 0 in <90 seconds. Weekly review needs a week. Partner mode needs a partner. Energy mode needs multiple data points. Aha must happen NOW.

**KPI for Aha:**

- **≥70%** of installs complete the voice brain-dump in first session (or text equivalent)
- **≥80%** of completions see a structured plan output
- **Time from app-open to first-plan-visible: ≤75 sec median, ≤90 sec p75**
- **Day 1 return rate ≥55%** (proxy for Aha quality — if Aha worked, she comes back)

**If Aha is broken:**

- <60% voice completion → Screen 3 friction analysis required (likely permission flow or microphone discoverability)
- >90 sec median → latency analysis required (LLM, transcription, network, render)
- Day 1 return <40% → plan output quality issue (LLM prompt engineering)
- High edit-rate on items immediately post-render → AI parsing accuracy issue

---

### Phase 4: Day 1-7 (First Week — Trial Honeymoon)

**Trigger:** Maya woke up Monday. Yesterday's onboarding happened Sunday night. She does NOT remember to open Planny first thing — object permanence is Pain #4. The question of the entire week is: does Planny stay alive in her field-of-view, or does it slide off the home screen into the app graveyard?

**Touchpoints by day:**

| Day | Push (if opted in) | In-app event | Email |
|-----|--------------------|--------------|-------|
| 1 (Mon) | Morning: "**Mon. First thing — 25 min on the Q3 deck. Want a head start?**" | Open app, see today | None |
| 2 (Tue) | Morning gentle: "**Tomorrow at 10 — dentist. Want to add 30 min for travel?**" | (Maybe doesn't open) | None |
| 3 (Wed) | Re-prompt: "**Things changed? Tap to re-voice your week.**" | (Re-engage) | None |
| 4 (Thu) | Morning only | Open app for re-plan | None |
| 5 (Fri) | None | Maya may open or not | **Honest email from Afek: "You haven't opened in 2 days. That's allowed. Trial cancels in 9 days. Tap to keep or cancel — no survey." — Afek** |
| 6 (Sat) | Silent (default — weekends opt-in only) | — | None |
| 7 (Sun) | **Weekly voice check-in: "Sunday voice — how did this week go?"** | Voice prompt | Optional weekly recap email |

**Emotions arc:**

- **Day 1: Cautious optimism.** Plan from last night is on her phone when she wakes up. First-thing tag tells her exactly what to start. Small dopamine hit.
- **Day 2: Validation OR drift.** Did Monday's plan hold? If yes: trust building. If Monday was hyperfocus-derailed: frustration risk, OR re-trust-opportunity if Planny's re-plan is gentle.
- **Day 3: Habit-formation moment.** Third open = pattern starting. Three-Sundays threshold mentioned in `tone-of-voice.md` line 34 ("The AI gets better as it learns your week. Give it three Sundays.")
- **Day 4: Hyperfocus crash risk.** If Maya hyperfocused on a side project Tue-Wed, Thu is meltdown. Planny must NOT shame the missed Tue-Wed items.
- **Day 5: Subscription guilt + honest check-in moment.** This is the most controversial design choice. The honest email may reduce conversion 5-10%. Accepted as brand cost.
- **Day 6: Weekend silence.** No push, no email. Maya gets the weekend off.
- **Day 7: Sunday voice check-in.** Highest-intent moment of the week. If Maya does this, she's likely to convert.

**Drop-off Risks:**

- **Day 2: Forgets to open.** Object permanence pain — Planny falls off home screen visibility. → Mitigation: widget (iOS 17+ Interactive Widgets) shows today's first-thing without opening app.
- **Day 3: Monday plan was wrong.** Frustration. → Mitigation: Day 3 re-prompt "Things changed? Tap to re-voice your week" — gives explicit permission to throw away last week's plan.
- **Day 4: Hyperfocus crash, missed everything.** Shame risk. → Mitigation: in-app copy on return: "**Tuesday was rough. That happens. Tomorrow can be different — or also rough. Either is fine.**" (verbatim from `tone-of-voice.md` line 63)
- **Day 5: Subscription guilt creeping** ("am I really using this?"). → Mitigation: HONEST email. Yes this costs conversions. Yes it's the brand promise.
- **Day 6: Saturday silence interpreted as "they forgot about me".** → Actually OK; weekend silence builds Sunday-anticipation.
- **Day 7: Hasn't opened in 3+ days → likely abandon.** → Mitigation: Sunday voice check-in push, soft language: "**Sunday voice — how did this week go?**" (NOT "you missed 5 days!" — that is the explicit `NOT Planny` anti-pattern, `tone-of-voice.md` line 189)

**Microcopy guardrails for Phase 4 push notifications:**

- ALL pushes follow `tone-of-voice.md` Trait 2 (Calm): no caps, no alarm emoji, no urgency
- Verbs: "**Want to**", "**Tap to**", "**Carry to**" — never "Don't forget!", "ACT NOW", "Missed!"
- Missed-task framing: "**Didn't get to laundry. Carry to today, or move to the weekend?**" (verbatim `tone-of-voice.md` line 195)
- Never use the words: `Overdue`, `Missed`, `Failed`, `Streak`, `Just` (per banned vocabulary line 332-347)
- Founder voice ONLY at Day 5 email — NOT in pushes (pushes are Planny voice, signed nothing)

**KPIs for Phase 4:**

- **Day 1 return rate ≥55%**
- **Day 3 return rate ≥40%**
- **Day 7 return rate ≥30%** (critical signal — if Day 7 falls below 25%, the cohort will not convert)
- **Sunday voice check-in completion ≥20%** of Day 7 returners
- **Push opt-in retention** (didn't disable pushes): ≥80% of those who opted in

---

### Phase 5: Trial Day 7-14 (Conversion Decision Window)

**Trigger:** Trial timer says 7 days left. Maya is consciously evaluating: keep paying for this? V-shape decision per `target-audience.md` line 243: she converts either on Day 0-1 (impulse) or Day 13-14 (deliberate). This phase is for the Day 13-14 deciders.

**Touchpoints:**

| Day | Channel | Message | Voice |
|-----|---------|---------|-------|
| 7 | In-app banner | "Trial ends in 7 days. Keep going or cancel — both are easy." | Planny |
| 10 | Push | "Trial ends in 4 days. Want to keep? Tap to confirm — same price as today." | Planny |
| 12 | Email | "**Hey — quick note from Afek. Trial ends in 2 days. We'd love to keep you, but no pressure. Two-tap cancel here if it's not working: [link]. Or annual at $39 (33% off) here: [link]. Either is fine. — Afek**" | Founder |
| 13 | Email | "**Final day. Tomorrow we'll charge for annual ($39 early-bird / $59 regular). If you'd rather cancel: [2-tap link]. If you'd rather keep: do nothing. — Afek**" | Founder |
| 14 | (Charge processes — 30-day refund still active) | App banner: "**You're in. 30-day refund still active if it doesn't work.**" | Planny |

**Emotions arc:**

- **Day 7: Evaluating.** "Did this actually help me last week?" Honest self-assessment.
- **Day 10: Wavering OR committed.** If used 4+ times in trial: committed. If <2 times: wavering toward cancel.
- **Day 12: Decision-forced.** Founder email forces conscious choice. Honest tone may swing both ways — some convert because of the honesty, some cancel because they were honest with themselves.
- **Day 13: Decision moment.** The "do nothing = charge" framing is fair (it's the legal default), but the explicit reminder removes the "I forgot trial was ending → annoyed auto-charge → refund" scenario that destroys trust.
- **Day 14: Charged.** Anxiety spike about the charge, immediately defused by "30-day refund still active" banner.

**Drop-off Risks:**

- **Day 7: Sticker shock realized.** "$59/year? I just used this for 7 days." → Mitigation: Day 12 email explicit price + 33% early-bird discount available.
- **Day 10: Found something else** (Saner, Indy by Shimmer — free competitor risk). → Mitigation: roadmap transparency, founder DM, Indy-anti-positioning ready ("Planny is not a coaching funnel — no conflict-of-interest").
- **Day 13: Forgot trial was ending → annoyed auto-charge → refund within 48 hours.** → Mitigation: Day 12 + Day 13 explicit reminders make "I didn't know" impossible. If she still doesn't cancel, she chose to keep.
- **Day 14: Charged but doesn't realize for 5 days.** → Sees charge on Amex statement, panics. → Mitigation: charge email is signed "**— Afek**" with refund link. "**You're charged. Here's how to refund within 30 days if it's not working: [link]. No questions.**"

**Refund flow (in-app, accessible from Settings → Subscription):**

```
Cancel and refund?

- Tap "Cancel and refund" below.
- Full refund within 48 hours.
- We'll keep your week's data for 30 days in case you come back. After that, deleted.
- That's it. No survey. No exit interview. No "are you sure?" three times.

[Cancel and refund]

If you want to tell me what didn't work — only if you want —
DM @planny on TikTok or email founder@planny.app.
I read every one. No reply expected back from you.

— Afek
```

*(Verbatim from `tone-of-voice.md` line 209. This is THE anti-Inflow moment. The explicit absence of friction is the brand promise.)*

**KPIs for Phase 5:**

- **Trial-to-paid conversion ≥35%** (industry median for productivity apps is 20-25%; persona-tuned + founder honesty should beat — but Day 5 honest email may cap upside)
- **Day 12 email open rate ≥50%** (founder-signed personal emails typically beat brand emails)
- **Day 13 cancel rate ≤10%** of remaining trialers (high cancel-after-Day-13 reminder = brand integrity intact)
- **30-day refund rate ≤5%** of paid (industry standard for honest products)
- **Cancel flow completion time ≤30 sec** (proof of 2-tap promise)

---

### Phase 6: Day 14-30 (Habit Formation OR Quiet Cancel)

**Trigger:** Maya is paid. Now what? Day 14-30 is the cohort-shaping window. By Day 30 she's either using Planny 4+ times/week or she's drifting.

**Touchpoints:**

- Daily push (morning first-thing only, if opted in)
- Weekly Sunday voice check-in
- Mid-week re-plan moment (Tuesday-Wednesday)
- Day 21 partner mode announcement (when shipped per `value-proposition.md` line 224)
- Day 28 "still working for you?" check-in
- Apple Watch widget glance (if she set up the widget)

**Emotions arc:**

- **Day 14-17: Honeymoon over, real-life test.** First real-life chaos test — kid sick, work crisis, partner conflict. Does Planny help re-plan or feel useless?
- **Day 18-21: Identity-shift moment.** If she's using Planny consistently: small pride. "**I have a system.**" If not: ADHD-tax guilt creeping.
- **Day 22-28: Pattern locks in OR breaks.** This is where 70% of users either become daily-openers or fade to weekly-only.
- **Day 29-30: Subconscious renewal check.** "Did this earn its place on my home screen?" Honest answer determines Day 60 outcome.

**Drop-off Risks:**

- **Day 17: First real chaos test fails.** Planny's re-plan suggestion was wrong / felt mechanical. → Frustration. → Mitigation: re-plan flow uses voice ("Tap to re-voice your week") rather than typed edit — voice = lower friction = re-engagement.
- **Day 21: Found "better" app** (Saner shipping new feature, Tiimo adding two-way sync, Apple Intelligence shipped at WWDC and feels magical). → Mitigation: founder DM open ("@planny on TikTok — I read every one"); roadmap transparency (public Notion roadmap).
- **Day 25: Hasn't opened in 5+ days → quiet drift.** → Mitigation: Day 25 trigger email — "**You haven't opened in a week. That's allowed. Want me to pause your billing for 30 days? Reply 'pause'. — Afek**" — this is the explicit anti-ADHD-tax position (`target-audience.md` line 132).
- **Day 30: Subscription guilt becomes load-bearing.** Maya wants to cancel but can't bring herself to. → This is the ethical line Planny WILL NOT cross (`target-audience.md` line 245). The Day 25 pause-offer prevents the silent-tax outcome.

**Mitigation summary:**

- Day 21 partner mode announcement (when shipped) — feature reactivation event
- Day 25 "want me to pause your billing?" — proactive anti-tax (loses revenue, builds brand)
- Day 28 "still working for you?" — last honest check before Day 30 renewal-conditioning
- Roadmap transparency (public Notion roadmap with what's coming)

**KPIs for Phase 6:**

- **Day 30 retention ≥40%** (apps opened 4+ times in last 7 days at Day 30) — *existential metric*
- **Sunday voice check-in completion ≥30%** by Day 30
- **Calendar connect rate ≥60%** by Day 30 (those who skipped at onboarding, came back to connect)
- **Cancel rate Day 14-30 ≤15%** of paid

---

### Phase 7: Day 30-365 (Long-term Retention / Referral / Renewal)

**Trigger:** Maya has been on Planny for a month. She's either a loyal user or a polite churner. The math of the business depends on the loyal cohort.

**Touchpoints:**

- Daily/weekly app opens (now habitual or not)
- Occasional founder DM exchanges (if she's a fan)
- Recommendations to friends in r/ADHDWomen, group chats, comorbidity therapy groups
- Day 90 retention checkpoint
- Day 180 mid-year usage report
- Day 330 renewal reminder
- Day 365 renewal charge

**Emotions arc:**

- **Day 30-60: Identity attachment.** "I'm a Planny person now." Small pride, slight relief.
- **Day 60-120: Routine integration.** Sunday voice check-in becomes ritual. Morning glance is automatic.
- **Day 120-240: Quiet utility.** Maya stops noticing Planny — it just works. THIS IS THE GOAL.
- **Day 240-330: Recommendation peak.** When a friend mentions ADHD, Maya brings up Planny unprompted. This is the viral expansion window.
- **Day 330-360: Renewal anxiety low-grade.** "Wait — when does this renew?" Pre-emptive Settings → Subscription check.
- **Day 365: Renewal moment.** If Day 320 communications were honest, this is anti-climax. If not, this is brand-damage event.

**Drop-off Risks:**

- **Day 45: Apple Intelligence iOS 27 ships powerful native AI scheduler.** Maya tries it. → Maybe leaves. → Mitigation: ADHD-tuned features Apple won't ship (buffers calibrated to time-blindness, energy-aware planning, "no streaks" promise, founder accessibility); WWDC war-room plan ready (`value-proposition.md` line 403).
- **Day 60: Tiimo adds two-way sync.** Wedge erodes. → Mitigation: partner mode shipped by Day 60; weekly voice check-in shipped; founder voice still uncontested.
- **Day 90: Maya enters life transition** (job change, pregnancy, breakup). Routine disrupted → Planny falls out. → Mitigation: gentle re-engagement: "**Hey — haven't seen you in a bit. Want to re-voice your week? — Afek**"
- **Day 200: Indy by Shimmer raises Series A, marketing surge.** → Mitigation: Maya is now a 6-month-loyal user; switching cost (her history, her trained AI) is real.
- **Day 330: Renewal email lost in inbox.** → Mitigation: Day 330 + Day 350 + Day 360 reminders, all founder-signed.
- **Day 365: Maya forgot the renewal, sees Amex charge, refund spiral.** → Mitigation: 30-day refund window stays active on renewal too; in-app banner Day 365: "**You renewed for another year. 30-day refund window starts today. — Afek**"

**Mitigation summary for long-term:**

- Founder DM accessibility — verbatim from `tone-of-voice.md` line 168: "**I read every email**"
- Public Notion roadmap (every shipped feature has a "you asked for this" note)
- Annual renewal email is humane: "**Want to keep going? Same price. Or cancel here: [link]. — Afek**"
- Refund window resets on renewal
- WWDC war-room plan active (`value-proposition.md` line 403) — 3 response scenarios prepped

**Referral KPIs (Day 30+):**

- **Day 90 NPS ≥50** (productivity app benchmark is 30-40; Maya cohort should exceed if Aha worked)
- **Day 180 organic referral rate ≥15%** of installs cite "friend recommended" (verbatim survey on download)
- **Day 365 renewal rate ≥75%** (productivity annual benchmark is 60-70%; honest brand should beat)
- **Founder DM volume** (proxy for brand attachment): ≥5% of MAU sends at least one DM in any given month

---

## End-to-End Journey Map (Visual)

```
                Day -30 to Day 0
[TikTok reel / Tracy Otsuka pod / r/ADHDWomen / ADDitude / friend DM]
                       │
                       ▼ (1-7 day decision cycle — V-shape)
              [App Store listing]
       (sees: founder photo, 30-day refund,
        "voice your week 60 sec", anti-shame copy)
                       │
                       ▼  ← FIRST DROP: subscription fatigue / sticker shock
                  [Install]
                       │
                       ▼  ← SECOND DROP: install-but-never-open (object permanence)
                Day 0, ~75-90 sec
        ┌──────────────────────────────┐
        │       ONBOARDING (90 sec)    │
        │  Screen 1: Founder intro     │
        │  Screen 2: Voice permission  │
        │  Screen 3: Voice brain-dump  │
        │  Screen 4: "Thinking with you"│
        │  Screen 5: ★ AHA MOMENT ★    │ ← "Someone did the EF for me"
        │  Screen 6: Calendar (opt)    │
        │  Screen 7: Notifications (opt)│
        └──────────────┬───────────────┘
                       │
                       ▼  ← THIRD DROP: voice permission denied / AI parse fail
              [Day 1-7: Trial honeymoon]
       (morning first-thing pushes; gentle copy;
        Day 3 re-prompt; Day 5 honest "still using?")
                       │
                       ▼  ← FOURTH DROP (BIGGEST): Day 7 hasn't returned
        ┌──────────────────────────────┐
        │  Day 7-14: Conversion window │
        │  Day 12: Founder email       │
        │  Day 13: Final reminder      │
        │  Day 14: Annual charged      │
        └──────────────┬───────────────┘
                       │
                       ▼  ← FIFTH DROP: cancel during trial
             [Day 14-30: Habit formation]
        (Day 21: partner mode; Day 25: pause-offer;
         Day 28: still-working check; Day 30 retention)
                       │
                       ▼  ← SIXTH DROP: Day 30 retention <40%
             [Day 30-365: Loyal user]
       (Sunday voice ritual; mid-week re-plan;
        founder DM; partner mode; widget; Apple Watch)
                       │
                       ▼  ← SEVENTH DROP: life transition / competitor / Apple ships
                [Day 365: Renewal]
       (honest renewal email + 30-day refund still active)
                       │
                       ▼
              [Loyal multi-year + referrer]
```

---

## Touchpoint × Emotion × Risk × Mitigation Table

| # | Touchpoint | Day | Emotion (primary) | Risk | Mitigation |
|---|-----------|-----|-------------------|------|------------|
| 1 | TikTok reel (founder POV) | -7 to 0 | Skeptical → Curious | Thumb-scroll past in 1.5 sec | Hook: "POV: your fifth planner this year" |
| 2 | Tracy Otsuka host-read | -3 to 0 | Hopeful → Wary | Sounds like generic ad | Founder-personal opener, not product-led |
| 3 | r/ADHDWomen comment | -7 to 0 | Curious | Reads as spam → brand burn | Zero promotion; only respond to questions |
| 4 | App Store listing | 0 | Hopeful → Cautious | Sticker shock + subscription fatigue | "30-day refund" + founder photo in screenshot 1 |
| 5 | App Store reviews | 0 | Scanning for red flags | 1-star billing-trap review unaddressed | Founder-signed reply within 24h to every negative review |
| 6 | Install → first open | 0 | Anticipation + guilt | Install-but-never-open (object permanence) | Icon prominence + no premature push |
| 7 | Onboarding Screen 1 | 0 | Curious → Trusting | Skip due to "another welcome screen" | Founder face + first-person "Hi. I'm Afek." |
| 8 | Voice permission | 0 | Slight discomfort | Denied (15-25%) | Preempt copy + text fallback equal weight |
| 9 | Voice brain-dump | 0 | Surprise → Relief | Speaks >60 sec, AI confused | 60-sec soft prompt, no hard cutoff |
| 10 | "Thinking with you" | 0 | Tense hope | Latency >8 sec → exit | Internal SLA ≤5 sec; no progress bar |
| 11 | **First plan reveal** | **0** | **★ AHA ★** | **Plan wrong → Aha broken** | **Confidence dots + 1-tap edit + under-place AI calibration** |
| 12 | Calendar connect | 0 | Reserved | Feels like sales push | OPTIONAL, equal-weight skip |
| 13 | Notifications opt-in | 0 | Boundary-setting | Declined | OK; re-offer Day 2 with context |
| 14 | Day 1 morning push | 1 | Sleepy → Engaged | Wakes up before push lands | Send 15 min after typical wake time (learned) |
| 15 | Day 2 silence | 2 | Object permanence drift | Forgets app | Widget surfaces first-thing without opening |
| 16 | Day 3 re-prompt | 3 | Reflective | Plan was wrong → frustration | Voice re-plan ("Tap to re-voice your week") |
| 17 | Day 4 hyperfocus recovery | 4 | Shame risk | "I missed everything" guilt | Copy: "Tuesday was rough. That happens." |
| 18 | Day 5 honest email | 5 | Surprised by honesty | -5-10% conversion accepted | Founder-signed; explicit cancel link |
| 19 | Day 7 Sunday voice | 7 | Reflective → Validated | Skipped → drift | Soft prompt: "Sunday voice — how did this week go?" |
| 20 | Day 10 trial-ending push | 10 | Wavering | Confused about price | Same price as today messaging |
| 21 | Day 12 founder email | 12 | Decision-forced | Cancels because of honesty | Brand cost accepted; conversion offset by retention quality |
| 22 | Day 13 final email | 13 | Decision moment | Forgot → annoyed auto-charge | Explicit reminder + 2-tap cancel |
| 23 | Day 14 charge + refund banner | 14 | Anxiety → Relief | Refund spiral | Banner: "30-day refund still active" |
| 24 | Day 21 partner mode launch | 21 | Curiosity | Partner refuses to install | Read-only share works without partner install |
| 25 | Day 25 pause offer | 25 | Surprised relief | Pauses instead of canceling | Net loss but anti-tax brand promise honored |
| 26 | Day 28 still-working check | 28 | Honest self-assessment | "No it's not" → cancel | OK; brand integrity > short-term retention |
| 27 | Day 30 retention checkpoint | 30 | Identity formation | App opens trickling | Survey: "What's missing?" — feedback collection |
| 28 | Day 90 NPS | 90 | Loyalty → Advocacy | Apple Intelligence shipped → trial it | Founder DM + roadmap transparency + ADHD-specific features |
| 29 | Day 330 renewal reminder | 330 | Pre-anxiety | Lost in inbox | 3 reminders (Day 330, 350, 360), founder-signed |
| 30 | Day 365 renewal | 365 | Anti-climax | Renewal-shock spiral | 30-day refund resets on renewal |

---

## Founder vs Brand Voice in Journey

הכלל הקבוע (`tone-of-voice.md` lines 422-436): ב-90 ימי launch הראשונים, **founder voice = brand voice**. אבל ב-journey יש 8 הקשרים שונים, וביניהם יש diff עדין בין "Afek כותב" לבין "Planny אומרת":

| Touchpoint | Voice | Pronoun | Sample copy |
|-----------|-------|---------|-------------|
| TikTok reel | Founder ("Afek") | "I" | "I built this because Tiimo broke my brain..." |
| Tracy Otsuka ad | Founder | "I" | "Hey — I'm Afek. I have ADHD too..." |
| App Store description | Founder | "an ADHD adult" | "Made by an ADHD adult who got tired of planners that punished him for being one." |
| App Store review reply | Founder | "I" | "Thanks for the report — Afek" |
| Onboarding Screen 1 | Founder | "I" | "Hi. I'm Afek." |
| In-app microcopy | Planny | "you" / no signature | "Tap to voice your week" |
| Push notifications (default) | Planny | implicit "we" / no signature | "Tomorrow at 10 — dentist. Want prep time?" |
| Push notifications (milestone) | Founder | "I" — rare, special | "Day 30 — you've used Planny 23 times. Just wanted to say hi. — Afek" |
| Email Day 5 honest check | Founder | "I" | "Hey — quick note from Afek..." |
| Email Day 12 trial-ending | Founder | "I" / "we" | "We'd love to keep you, but no pressure. — Afek" |
| Email Day 365 renewal | Founder | "I" | "Renewed for another year. Refund window open. — Afek" |
| Cancel flow copy | Founder | "I" | "I read every one. — Afek" |
| Bug apology email | Founder | "I" / "That's on me" | "That's on me. Voice capture broke between 9-11am. Fixed. — Afek" |
| Roadmap update | Founder | "I" / "we" | "Hey all — here's what's next..." |
| In-app today view | Planny | "you" | "First thing — 25 min on Q3 deck. Want a head start?" |
| Widget | Planny | implicit | "First thing — Q3 deck (25 min)" |

**The dual-voice rule:**

- **Founder voice** = transactional moments + emotional milestones + accountability moments. Always signed "— Afek".
- **Planny voice** = operational moments + daily utility. Never signed.
- **Crossover risk:** if Planny voice slips into "we'd love to" or "we're excited" — that's corporate-plural drift, banned by `tone-of-voice.md` line 364.

---

## "Aha Moment" Deep Dive

### Definition

**Maya speaks 20-45 seconds of unstructured chaos about her week. ≤8 seconds later, Planny shows her week structured on screen — first-thing tagged, buffers in place, items per day — with zero setup decisions made.**

The internal feeling Planny engineers for: *"Someone did the executive function for me."*

### Why this is THE Aha (and not the alternatives)

| Candidate | Why it's not THE Aha |
|-----------|---------------------|
| Weekly voice review (Sunday) | Requires a full week to land. Aha must happen Day 0. |
| Partner mode | Requires a partner installed. v1.1 feature. |
| Energy-aware re-plan | Requires multiple data points (a few days of usage). |
| Two-way calendar sync | Functional value, not emotional revelation. |
| 30-day refund | Trust signal, not value experience. |
| Founder DM | Community-building, not product value. |
| **Voice → week render** | **Day 0. Zero setup. Solves Pain #1. Differentiates from every competitor. The wedge.** |

### KPIs for Aha

- **≥70%** of installs complete voice brain-dump (or text equivalent) in first session
- **≥80%** of completions see a structured plan output
- **Time from app-open to first-plan-visible: ≤75 sec median, ≤90 sec p75**
- **Day 1 return rate ≥55%** (proxy for Aha quality)
- **Item edit-rate within 5 min of plan render ≤25%** (proxy for AI parsing accuracy)

### If Aha is broken

- **<60% voice completion** → onboarding flow rework: voice permission preempt copy, mic discoverability, or fallback prominence
- **>90 sec median time-to-plan** → latency analysis: LLM, transcription, network, render. Hardest to fix; may require on-device transcription.
- **Day 1 return <40%** → plan output quality issue: LLM prompt engineering, item placement logic, "first thing" tagging
- **Item edit-rate >40%** → AI parsing is over-confident; recalibrate to under-place

---

## Aha Moment Backup (Second-Chance UX)

If Maya doesn't have time for full brain-dump on first install (got called away, dropped the phone, walked into a meeting):

1. **State preservation:** cold-open returns to last screen. If she was on Screen 3 (mic), prompt: **"You were saying... [first 5 words of transcript]. Continue?"**
2. **Quick Start fallback (if she actively skipped voice):** Show pre-populated example week ("**Here's what a Maya-week looks like. Try editing this — then voice your real one.**"). After 30 sec exploration, prompt: **"Want to voice your real week now?"**
3. **Mini-Aha:** if she still skips, give her a single-item Aha. Tap "+", say "dentist tomorrow at 10", item appears in slot in 3 sec. Smaller Aha, same mechanic, proves the value.
4. **Day 2 push (if opted in):** "**Yesterday we didn't finish setting up. Want to voice your week now? (Takes 60 sec.)**"

The backup flow exists so the Aha can happen on Day 1 or Day 2, not just Day 0. Window must close by Day 3 — after that, install is effectively churn.

---

## Strategic Connections

- ראה `01-discovery/target-audience.md` ל-Maya persona מלאה + decision-cycle V-shape + cancellation triggers
- ראה `02-strategy/value-proposition.md` ל-15 must-have features ול-pain-relievers mapping
- ראה `02-strategy/positioning.md` ל-anti-positioning מול Tiimo / Inflow / Motion
- ראה `02-strategy/go-to-market.md` ל-Phase 1 (Awareness) channel ranking ול-Tracy Otsuka / ADDitude / TikTok briefs
- ראה `03-brand/tone-of-voice.md` ל-microcopy rules בכל touchpoint (founder voice / Planny voice / banned vocabulary)
- ראה `03-brand/mission-vision-values.md` ל-4 pillars (Honest / Calm / Real / Capable) שמכוונים כל מילה ב-journey
- TBD `04-product/mvp-definition.md` — F1-F10 feature spec (להשלים — קבצי MVP טרם נכתבו)
- TBD `04-product/feature-prioritization.md` — RICE order

---

## Founder Input Requested

1. **האם ה-onboarding flow ב-7 מסכים תואם למה שתכננת ב-90% UI?** במיוחד: Screen 4 ("Thinking with you" — 3-5 sec animation) קיים? Screen 5 (entrance animation 1.2 sec sequential) קיים?
2. **Calendar connect — אופציונלי או חובה ב-onboarding?** ההמלצה החזקה כאן: אופציונלי לעבור Aha קודם. כפיית calendar connect לפני first-plan render = -30% completion (השערה).
3. **Voice prompt window — תוכל לעמוד ב-20-45 sec real speech + 8 sec render = 75 sec total?** או שצריך לבדוק חלון 60 sec הדוק יותר?
4. **Aha moment definition — האם זה הרגע שאתה גם רואה?** או שאתה רואה Aha אחר? (Weekly review, partner mode, energy-aware re-plan — אני טוענת שאף אחד מאלה לא מתאים ל-Day 0, אבל אם אתה רואה אחרת — נשנה.)
5. **Default view — day view או week view אחרי Aha?** Maya כנראה רוצה week ב-overview, day לפרטים. ההמלצה: week view default, tap day → expanded day view.
6. **Day 5 honest email — מסכים לקבל את ה-5-10% conversion cost?** זה ה-brand-defining moment. אם לא — צריך להגדיר מחדש את ה-positioning vs Inflow.
7. **Day 25 pause-offer — מסכים לבנות?** Net revenue cost מובהק, אבל זה ה-anti-tax position שמפריד את Planny מ-Inflow ב-r/ADHDWomen narrative.
8. **WWDC June 8 — האם יש war-room ערוך?** 10 ימים מהיום. אם Apple שולחת voice→calendar native, ה-Aha של Planny עלול להיראות commodity. תלוי בתגובה תוך 72 שעות.

---

## Sources

**Internal (Phase 1-5 docs):**

- `/home/user/NEW-_PROJECT/startup-validation/01-discovery/target-audience.md` (Maya persona; decision-cycle V-shape; cancellation triggers; daily workflow snapshot; Aha definition lines 347-360)
- `/home/user/NEW-_PROJECT/startup-validation/02-strategy/value-proposition.md` (15 must-have features; pain-reliever mapping; Aha-moment business case lines 247-265; WWDC risk line 403)
- `/home/user/NEW-_PROJECT/startup-validation/02-strategy/positioning.md` (anti-positioning vs Tiimo / Inflow / Motion)
- `/home/user/NEW-_PROJECT/startup-validation/02-strategy/go-to-market.md` (Phase 1 channel ranking; Tracy Otsuka ad copy; TikTok creator briefs)
- `/home/user/NEW-_PROJECT/startup-validation/03-brand/tone-of-voice.md` (microcopy rules per touchpoint; founder voice = brand voice 90-day rule; banned vocabulary; 8 writing samples)
- `/home/user/NEW-_PROJECT/startup-validation/03-brand/mission-vision-values.md` (4 personality pillars)

**External (UX frameworks):**

- McKinsey CJM methodology (touchpoint × emotion × moment-of-truth model)
- Nir Eyal *Hooked* (Trigger → Action → Variable Reward → Investment loop; mapped to Phases 1-7)
- Reforge "Aha Moment" definition (single most impactful product action correlated with retention)
- Jobs-to-be-Done outcome map (Christensen / Klement) — mapped to Phase 3 Aha definition
- Andrew Chen "PMF retention curve" — Day 30 retention as existential metric (Phase 6 KPI)

---

## Flags

### Red Flags

- **Aha moment (≤90 sec, ≤75 sec internal SLA) is technically aggressive.** Voice transcription + LLM parsing + UI render in 8 seconds requires low-latency stack — possibly on-device transcription + streaming LLM responses + pre-rendered week skeleton. If real-world median exceeds 12 sec, the Aha cliff breaks. **Mitigation:** beta test latency with 20+ Maya-persona users before launch; if median >10 sec, ship with a placeholder week skeleton that fills in as data arrives (perceived latency < actual).

- **Day 30 retention is unknown for ADHD audience.** The entire business model hinges on it. Industry productivity benchmarks (40% Day 30) may not transfer to ADHD population (31.6% mHealth abandonment baseline per `target-audience.md` line 422). **Mitigation:** Day 30 cohort tracking from Day 1 of launch; alarm at <30% Day 30 retention triggers immediate UX deep-dive.

- **Onboarding flow assumes voice permission granted.** Denied flow (15-25%) is critical fallback path that often gets de-prioritized. **Mitigation:** text input must be ALWAYS visible (equal weight to mic) on Screen 1; text-flow must render the SAME Aha at Screen 5; QA text-flow with same rigor as voice-flow.

- **WWDC June 8, 2026 (10 days from today) — Apple Intelligence iOS 27 calendar AI.** If Apple ships voice→calendar with high quality, Planny's Aha may look like commodity. **Mitigation:** war-room week starting June 5; 3 response scenarios (heavy/light/delayed) drafted; positioning shift ready to "ADHD-specific layer on top of Apple Intelligence" if needed.

- **Day 5 honest email + Day 25 pause-offer are revenue-negative but brand-defining.** Combined cost: -10-15% conversion + -3-5% retention. If founder loses nerve and removes these, the brand collapses into "Inflow-lite". **Mitigation:** commit these into product spec, not marketing decisions — make them non-negotiable architecture.

### Yellow Flags

- **Aha quality depends on LLM output.** If AI parses messy speech poorly (especially non-white-American-English speakers, AAVE, code-switching), Aha fails differentially across demographics — equity risk + brand-reputation risk. **Mitigation:** diverse beta testing (`value-proposition.md` line 417); confidence indicators visible; text fallback one tap away.

- **Founder voice ≠ Brand voice handoff in journey is delicate.** Touchpoints alternate (TikTok = founder, push = Planny, email = founder, in-app = Planny). If user perceives bait-and-switch ("Afek welcomed me, now a corporate brand is texting me"), trust breaks. **Mitigation:** dual-voice table above; train-the-team document with 50+ samples per voice per touchpoint type.

- **Day 7 weekly Sunday voice check-in completion is the leading indicator of Day 30 retention.** If users don't return for the Sunday ritual by week 2, Day 30 cohort will be small. **Mitigation:** Sunday push at the user's typical Sunday-evening time (learned per user); microcopy: "**Sunday voice — how did this week go?**" — NOT "you missed 5 days!"

- **Founder DM accessibility ("I read every email") is not scaleable past $10K MRR.** At 1,000 paying users, 5% DM rate = 50 DMs/month = 25-30 hours/month of founder time. **Mitigation:** at $10K MRR, transition to "**Afek + team**" signature with founder spot-checking; before then, lean into it as a brand asset.

- **Partner mode is named in journey (Day 21) but is v1.1 feature — not yet shipped.** If shipped >6 months after launch, Day 21 reactivation moment doesn't exist. **Mitigation:** ship partner mode by Day 60 of launch per `value-proposition.md` line 415; publish public roadmap with date commitment.

- **Day 25 pause-offer copy ("Want me to pause your billing for 30 days?") is operationally complex.** Requires billing system that supports pause (Stripe does; App Store IAP does NOT support pause natively — must be implemented as cancel + re-subscribe nudge). **Mitigation:** coordinate with finance on operational feasibility before committing to copy. Worst case: "**Want me to cancel and remind you in 30 days to re-subscribe?**" — less elegant but operationally clean.

- **Refund window resetting on renewal (Day 365)** sets a legal/financial expectation. If operations can't deliver 48-hour refunds reliably, the promise is a lie. **Mitigation:** verify with finance + support team before launch; build refund automation in Stripe; have a 48-hour SLA dashboard internal.

- **Push notification frequency (Day 1 morning + Day 3 re-prompt + Day 7 Sunday) may feel high to some users.** Maya's notification-blindness threshold is low. **Mitigation:** progressive disclosure — Day 1 push only if she opted in; Day 3 push only if she hasn't opened since Day 1; Sunday push only if she completed Week 1 voice check-in OR if she's been silent for 3+ days. Adaptive frequency > fixed frequency.
