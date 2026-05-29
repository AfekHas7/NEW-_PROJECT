# Regulatory Landscape: ADHD Productivity App (US + Israel)

**Phase:** Phase 3 — Wave 1 (A3)
**Project:** startup-validation (Planny)
**Date:** 2026-05-28
**Confidence:** Medium-High (core regulatory frameworks are well-documented; ADHD-specific case law is sparse, and some Israeli digital health specifics rely on Tier-2 sources)

---

## Executive Summary (TL;DR)

Planny operates in a **navigable but non-trivial gray zone**. The good news: as a scheduling/productivity tool that does NOT diagnose, treat, or monitor ADHD symptoms, Planny can almost certainly:
- Stay outside FDA SaMD oversight (General Wellness pathway, post Jan 2026 update favorable)
- Stay outside HIPAA (not a covered entity, not a business associate)
- Avoid Apple's March 2026 "regulated medical device status" requirement IF it lists as Productivity (not Health & Fitness / Medical)

The bad news: marketing to "people with ADHD" puts Planny in scope of:
- **Washington My Health My Data Act (MHMDA)** — almost certainly applies, $7,500/violation + private right of action
- **FTC Health Breach Notification Rule (HBNR, expanded 2024)** — applies to any app tracking mental-health-related data, $51,744/violation
- **CCPA/CPRA sensitive personal information** rules
- **Israel Amendment 13 (effective Aug 2025)** — mandatory DPO, ISS (Information of Special Sensitivity) handling
- **GDPR Article 9** — if any EU user accesses the app, explicit consent required

**Regulatory risk: MEDIUM.** Manageable with disciplined marketing language and ~$15-30K compliance spend at launch. Major risk vector is marketing copy drift ("treats ADHD", "improves focus") which would trigger FDA/FTC scrutiny.

---

## Apple App Store Requirements

### Key 2026 Update (CRITICAL FOR PLANNY)
Effective **March 26, 2026**, any app categorized as primary or secondary **Health & Fitness** or **Medical**, OR marked as containing "frequent references to Medical or Treatment Information" in the App Store Connect Age Rating questionnaire, will be required to declare a **regulated medical device status**. [Tier 2 — Telehealth.org / dashsdk; corroborated by Apple Developer News]

**Implication for Planny:** This is the single most important categorization decision. If Planny self-categorizes as Productivity AND avoids "frequent" medical/treatment references in the age rating, it sidesteps this requirement entirely.

### Guideline 1.4.1 (Medical) — what triggers heightened scrutiny
- Apps that "could provide inaccurate data or information, or that could be used for diagnosing or treating patients" face greater review scrutiny.
- Apps making accuracy claims about health measurements without disclosed methodology will be rejected.
- Medical apps must "remind users to check with a doctor in addition to using the app and before making medical decisions."

### Common Rejection Reasons Relevant to Planny
1. **Privacy policy missing or vague** — Apple is consistently strict; #1 rejection trigger for health-adjacent apps. [Tier 2]
2. **Health-related claims without authority backing** — A meditation app was rejected for referencing COVID-19 without a recognized health authority's authorization (example: Apple scrutinizes mental-health messaging tightly). [Tier 2]
3. **Falsely claiming medical functions** — automatic rejection. [Tier 1 — Apple Guidelines]
4. **Data sharing for advertising** — Apps in Health & Fitness / Medical "may not use or disclose to third parties data collected... for advertising, marketing, or data mining purposes."

### Category Recommendation for Planny
**Primary: Productivity. Secondary: (leave blank, or Lifestyle).**

Rationale:
- Planny's core function is scheduling/calendar management. That is textbook Productivity.
- "Health & Fitness" covers "stress management, fitness... yoga, meditation." Planny is not in that family.
- Choosing Health & Fitness would (a) trigger the March 2026 medical device declaration, (b) raise reviewer scrutiny under Guideline 1.4.1, (c) restrict advertising/monetization options, and (d) gain no discoverability benefit since users searching "ADHD planner" search by keyword, not category.
- App description and keywords can still include "ADHD" and "neurodivergent-friendly" — these are user descriptors, not medical claims. Inflow (currently live: id1528183849) does exactly this in the App Store. [Tier 2 — observed]

### Required Disclaimer Language (Apple)
Apple does not mandate a specific verbatim disclaimer for non-medical apps, but for any app marketing to a mental-health condition population, include in app description, onboarding, and ToS:

> "Planny is a productivity and scheduling tool. It is not a medical device and is not intended to diagnose, treat, cure, prevent, or mitigate any medical condition, including ADHD. Consult a qualified healthcare provider for medical advice."

This same line satisfies Google Play's January 2026 requirement (see below).

---

## Google Play Requirements

### January 2026 Health Apps Policy (in effect)
Google Play rolled out major health-app changes effective January 2026. Key requirements (verified across Play Console Help + Tier-2 summaries):

1. **Mandatory disclaimer for non-cleared apps:**
   > "This app is not a medical device and does not diagnose, treat, or prevent any condition."
   Must appear in the **first paragraph** of the store description. Failure = update rejection. [Tier 2 — myappmonitor; high-confidence]

2. **Organization Account verification:** Existing health apps had until **Jan 28, 2026** to migrate to a verified Organization Account. New apps must register as Org Accounts if classified as health. Even if Planny is Productivity, having an LLC/Ltd as the developer account is recommended for liability separation.

3. **Health Connect data justification:** If Planny ever requests `READ_HEALTH_DATA_IN_RECORDS` (blood pressure, sleep, etc.), it must prove the data is essential to primary function. **Planny should NOT request Health Connect data** — it would create a documentation burden with no product benefit.

4. **Medical Device labeling system:** Apps with regulatory clearance (e.g., FDA SaMD) get a verified badge. Apps without clearance must include the disclaimer above. Planny will not have clearance, so disclaimer is mandatory.

### April 2026 Update
Google further clarified prohibited use cases: **sensitive health data may not be used for determining employment or insurance eligibility, or for unauthorized social sharing.** Planny's privacy policy must explicitly prohibit these uses.

### Category Recommendation
**Primary: Productivity.** Same rationale as Apple. Google Play distinguishes Health & Fitness apps narrowly; a scheduling tool that happens to be ADHD-friendly does not belong there.

---

## FDA SaMD Threshold

### The Boundary (Updated Jan 6, 2026)
On **January 6, 2026**, FDA issued final updated guidance for both General Wellness Products and Clinical Decision Support (CDS) Software. The 2026 guidance supersedes 2019/2022 versions and represents a **deregulatory shift** — generally favorable for Planny. [Tier 1 — FDA; Tier 2 — Faegre Drinker, King & Spalding, Ropes & Gray, Latham & Watkins all corroborate]

### General Wellness "Safe Harbor"
A product is a General Wellness Product (NOT a regulated device) if:
1. It is **low risk** to users (non-invasive, no significant safety issues), AND
2. Its intended use is either:
   - **Category 1:** Sustaining/improving general health functions WITHOUT reference to a disease — explicitly includes "stress management, mental acuity, self-esteem, sleep management" [Tier 1 — FDA]; OR
   - **Category 2:** Helping reduce risk of, or help live with, certain chronic conditions where the connection is well-understood and the product does not diagnose/treat/cure.

**Critical 2026 clarification:** Whether something qualifies as general wellness now depends on **how it's advertised and promoted**, not just on inherent function. **Marketing copy is the regulatory trigger.**

### Where Planny Sits
Planny's core function — helping users plan their week — is a productivity feature, not a health intervention. As long as marketing stays in "wellness" / "organization" / "executive function support" language and avoids treatment/diagnostic claims, Planny sits comfortably **outside FDA jurisdiction**.

### Examples of Apps That Crossed the Line
- **EndeavorRx** (Akili Interactive): FDA-cleared digital therapeutic for pediatric ADHD (ages 8-12). Required De Novo clearance. This is the "other side" of the line — they explicitly claim therapeutic benefit, run RCTs, and require a prescription. [Tier 1/2 — well documented]
- **EndeavorOTC** (adult version): cleared under 510(k) in 2024 — same company crossed the line intentionally for the adult ADHD market. They are a regulated medical device.

The lesson: Akili crossed the line **on purpose** to make therapeutic claims. Planny should explicitly NOT.

### Words/Phrases Planny MUST AVOID
- "Treats ADHD" / "Treatment for ADHD"
- "Reduces ADHD symptoms"
- "Improves focus" (clinical claim — improving attention is a treatment effect)
- "Therapy" / "therapeutic"
- "Clinically proven" (unless an actual clinical trial exists)
- "Diagnoses" or anything diagnostic-adjacent
- "Replaces medication" / "alternative to Adderall"
- "Doctor-recommended" (unless documented and substantiated)
- "ADHD coach" (this is FTC territory — see below)

### Words/Phrases Planny CAN Use
- "Designed for adults with ADHD" (descriptive, not therapeutic)
- "ADHD-friendly planning" / "neurodivergent-friendly"
- "Helps you organize your week"
- "Built with executive-function challenges in mind"
- "Supports planning and time-management"
- "May help you stay organized" (carefully hedged)

### How to Structure Planny to STAY in Wellness Category
1. Position as a **scheduling/calendar tool** that is **designed for** (not "treats") ADHD users.
2. Never include "symptom tracking" features (logging hyperactivity, impulsivity, attention scores). The moment Planny tracks ADHD symptoms, it inches toward diagnostic territory.
3. If adding mood/check-in features, scope tightly: "How focused did today feel? 1-5" is borderline OK; "Rate your ADHD symptoms today" is not.
4. Do not produce reports a clinician would use for treatment decisions. (Output for users only.)
5. Keep all in-app copy, marketing site, App Store description, paid ads, and influencer briefs aligned — FDA looks at all promotional channels, including social media.

---

## Data Privacy (US)

### HIPAA — Does it Apply to Planny?
**Almost certainly NO**, with one caveat. [Tier 2 — Focal Point, NYSBA, HHS guidance corroborates]

HIPAA applies only to "covered entities" (insurance companies, healthcare providers, clearinghouses) and their "business associates." A consumer-direct app that users download on their own and into which they enter their own data is generally NOT a covered entity.

**Caveat:** If Planny ever partners with a clinic, ADHD coaching practice, telehealth provider, or insurer to deliver the app to their patients/members, Planny may become a Business Associate and trigger full HIPAA compliance. Avoid B2B2C health partnerships at launch unless prepared for a HIPAA program (~$50-100K+ at scale).

### CCPA / CPRA (California)
Planny WILL be subject to CCPA/CPRA if it has California users AND meets at least one of:
- $25M+ annual revenue, OR
- Buys/sells/shares personal info of 100K+ California consumers, OR
- 50%+ revenue from selling/sharing PI.

Even pre-revenue, **planning ahead** is cheaper than retrofitting.

**Critical:** Mental health information is **"sensitive personal information" (SPI)** under CPRA. This triggers:
- Right to limit use of SPI (the "Limit the Use of My Sensitive Personal Information" link on homepage)
- Heightened consent and disclosure obligations
- 2025-finalized rules add mandatory **cybersecurity audits** and **privacy risk assessments** (phased in 2027-2028 for qualifying businesses)

### Washington My Health My Data Act (MHMDA) — HIGH-PRIORITY RISK
**MHMDA almost certainly applies to Planny.** [Tier 2 — IAPP, Cooley, Accountable HQ; high consensus]

"Consumer health data" under MHMDA is extremely broad: includes "personal information... that identifies past, present, or future physical or **mental health status**, including conditions... and inferences derived from non-health data." An app marketed to "adults with ADHD" inherently identifies users' mental-health status the moment they download it.

Requirements:
- **Separate Health Data Privacy Policy** (in addition to general privacy policy)
- **Separate consent for collection AND separate consent for sharing/selling**
- Honor withdrawal of consent
- Geofencing prohibition around health facilities (irrelevant for Planny)

**Penalties:**
- Up to **$7,500 per violation** via WA Consumer Protection Act
- **Private right of action** — consumers can sue directly, recover actual damages + attorneys' fees
- Courts may award treble damages up to **$25,000**

**Strategic note:** This is enforced more aggressively than CCPA because of the private right of action. Plaintiffs' firms are actively trolling for MHMDA violations.

### Other State Health-Data Laws (Emerging)
Nevada SB 370 and Connecticut's amendments to its data privacy act adopted MHMDA-style provisions. New York's SHIELD Act and the proposed New York Health Information Privacy Act may follow. Planny should architect privacy controls to satisfy MHMDA as the **highest common denominator** — it covers the others.

### FTC Health Breach Notification Rule (HBNR) — APPLIES TO PLANNY
The HBNR (expanded April 2024, effective July 29, 2024) now covers "any online service such as... mobile application... that provides mechanisms to track... mental health" or related conditions. [Tier 1 — FTC; Tier 2 — Wilson Sonsini, Alston & Bird]

**Even though Planny is "just" a planner, the moment it tracks anything resembling mental-health-related data (mood, focus check-ins, ADHD-relevant journaling), HBNR applies.**

Requirements:
- Notify affected consumers, FTC, and (for 500+ users) media within **60 calendar days** of discovering a breach.
- Civil penalties: **$51,744 per violation** (per affected user, per day in some interpretations).
- Includes "unauthorized disclosure" — sharing data with ad networks without explicit consent counts as a breach.

This is the rule under which the FTC went after **BetterHelp ($7.8M, 2023)** and **Cerebral ($7M FTC + $3.6M DOJ, 2024)** — see Marketing Claims section.

---

## Data Privacy (Israel + EU exposure)

### Israel — Amendment 13 (Effective Aug 14, 2025)
[Tier 2 — IAPP, BigID, Safetica, Library of Congress; high consensus]

Amendment 13 is Israel's largest privacy reform in 40 years. Key implications for Planny:

1. **Information of Special Sensitivity (ISS):** Explicitly includes "health and genetic information." Marketing to ADHD users + collecting any related data = ISS handling.

2. **Mandatory Data Protection Officer (DPO):** Required for organizations processing ISS at scale. For a small startup, a fractional/outsourced DPO is acceptable and typically runs **$8K-25K/year**. The threshold for "scale" is data on a "considerable number" of Israeli residents — unclear cutoff but conservative read is once Planny crosses ~10K Israeli users.

3. **Tightened consent:** Must be informed, specific, and documented. Pre-checked boxes don't count.

4. **Civil suits without proof of harm:** Individuals can sue for statutory damages up to **NIS 100,000 (~$27K) per person** without proving damage.

5. **Administrative fines:** Up to several million NIS (~$500K+ per violation), with multipliers for ISS or large-scale processing.

6. **Registration:** Databases containing ISS for >10,000 individuals must be registered with the Privacy Protection Authority (PPA).

**Practical first-launch step:** Register the database with the PPA when Israeli user base approaches 10K; appoint a DPO (or fractional DPO) at the same milestone.

### Israel — Digital Health Specific
There is **no dedicated digital-health law in Israel.** Regulation flows from Ministry of Health (MoH) circulars + the Medical Equipment Law 2012 (AMAR). [Tier 1 — ICLG, Chambers; Tier 2 — Emergo, MedEnvoy]

Planny does NOT require AMAR registration because it is not a medical device — same logic as FDA General Wellness. The MoH circulars on remote care, informed consent, and cloud computing apply to healthcare providers, not to consumer productivity apps.

### GDPR (EU exposure)
GDPR applies extraterritorially to any non-EU service that targets EU residents OR monitors their behavior. If Planny is available on EU app stores OR markets to EU users, **GDPR applies in full.**

Mental-health-related data is "special category data" under **Article 9** — processing is prohibited unless an exception applies. For a consumer app, the only viable exception is **Article 9(2)(a) explicit consent.**

Requirements:
- Explicit, granular, separate consent for processing health-related data
- A generic "I agree to privacy policy" is NOT explicit consent (settled position)
- DPIA (Data Protection Impact Assessment) required for systematic processing of special category data at scale
- EU representative required if no EU establishment (Article 27)

### Estimated Compliance Cost
| Component | Minimum Launch | At Scale (~50K users) |
|---|---|---|
| Privacy policy + ToS + disclaimer drafting | $2K-5K (template + lawyer review) | $10K-15K (full bespoke) |
| App Store + Play Store legal language | $1K-2K | included above |
| MHMDA-compliant Health Data Privacy Policy + consent flows | $3K-7K | $10K-15K |
| CCPA/CPRA compliance (rights link, opt-outs) | $2K-5K | $10K-25K (audits in 2027+) |
| Israel Amendment 13 — fractional DPO | $0 below threshold | $8K-25K/year |
| GDPR (if EU launched) — DPIA + EU rep + consent | $5K-15K | $15K-30K + EU rep ~$500-1500/month |
| FTC HBNR breach-response retainer | $0 if no breach | (insurance ~$2K-5K/year, ~$50K-200K if incident) |
| **Total launch (US-only)** | **~$8K-19K** | **~$30K-80K** |
| **Total launch (US + Israel + EU)** | **~$15K-35K** | **~$60K-160K** |

Tier-2 sources estimate "compliance adds $5K-15K for encryption, legal reviews, and audits" for a mental-health-adjacent app — consistent with our low-end estimate. Cost climbs fast with EU exposure.

---

## Marketing Claims (FTC)

### What Planny CAN Claim
- "Designed for adults with ADHD"
- "ADHD-friendly weekly planner"
- "Helps you organize and prioritize your week"
- "Built with executive-function challenges in mind"
- "May help you build planning habits"
- "An AI scheduling assistant for neurodivergent adults"
- Testimonials describing **personal experience** (with required disclosure: "Individual results vary. This is not a medical claim.")

### What Planny CANNOT Claim
- "Treats ADHD" / "Treatment for ADHD"
- "Reduces ADHD symptoms"
- "Improves focus / attention" (clinical benefit claim)
- "Clinically proven"
- "Doctor-recommended" / "Therapist-approved" (without substantiation)
- "Alternative to medication"
- "Replaces a therapist / coach"
- "Cures procrastination" (FTC will treat as a health claim if procrastination is framed as an ADHD symptom)

### FTC Enforcement Reference Cases
- **BetterHelp (March 2023):** $7.8M settlement. Charges: deceptive privacy claims + sharing mental-health questionnaire data with Facebook, Snapchat, Pinterest, Criteo for ad targeting. Order bans health-data sharing for advertising; mandates affirmative express consent; mandates a privacy program; third-party data deletion. [Tier 1 — FTC]
- **Cerebral (April 2024):** $7M FTC settlement. Charges: sharing data of 3.2M consumers with LinkedIn, Snapchat, TikTok; deceptive "Cancel anytime" claims (ROSCA violation). [Tier 1 — FTC; Tier 2 — MedCity, STAT]
- **Cerebral (Nov 2024):** $3.6M DOJ NPA for prescribing Adderall via telemedicine in violation of the Controlled Substances Act. [Tier 2 — Arnold & Porter advisory]
- **GoodRx ($1.5M, 2023):** HBNR enforcement for sharing health data with Facebook/Google. First HBNR enforcement; signals the FTC's appetite to use it against apps. [Tier 1 — FTC]

**Common pattern:** Every major FTC action against a mental-health app has been about **data sharing with ad networks**, not therapeutic claims. The data-sharing risk is therefore Planny's #1 enforcement risk.

### Practical Rule
Treat any conversion pixel (Meta Pixel, TikTok Pixel, Google Ads tag) on a page that contains the word "ADHD" as a regulatory tripwire. Either (a) don't use pixels on those pages, or (b) use server-side conversion APIs with hashed identifiers and explicit user consent collected separately from sign-up consent. The BetterHelp and Cerebral orders specifically attack the pixel pattern.

---

## Compliance Cost Estimate (Summary)

### Minimum Viable Compliance at Launch (~$10-20K, US-only)
- Privacy policy + ToS + medical disclaimer (lawyer-reviewed, ~$3-7K)
- MHMDA-compliant separate health data policy + consent UX (~$3-5K)
- CCPA opt-out and SPI limitation links (~$1-2K)
- Apple/Google store descriptions with required disclaimer (in-house, ~free)
- Basic security baseline (TLS 1.2+, AES-256 at rest, MFA on admin) — engineering cost, not legal
- Avoid third-party ad pixels on ADHD-related pages (free, requires discipline)
- Tracking: Apple Privacy Manifest + Google Data Safety form

### Add for Israel Launch (~$5-10K incremental)
- Hebrew-language privacy policy + consent flow
- Fractional DPO once Israeli users exceed ~10K (~$8-25K/year)
- Database registration with PPA (~$1-2K legal + filing)

### Add for EU Launch (~$5-15K incremental, plus ongoing)
- GDPR-compliant explicit consent for special-category data
- DPIA (~$3-7K)
- EU representative (~$500-1,500/month)
- Cookie consent (CMP), ~$50-200/month at scale

### Full Compliance at Scale (50K+ users, all three markets): ~$60-160K/year ongoing

### Required Documents/Surfaces
1. Privacy Policy (general)
2. Health Data Privacy Policy (MHMDA-specific)
3. Terms of Service
4. Medical Disclaimer (in onboarding, in app description, in ToS)
5. CCPA "Do Not Sell or Share" + "Limit Use of SPI" links
6. EU cookie consent banner (if EU)
7. Apple Privacy Manifest (PrivacyInfo.xcprivacy)
8. Google Data Safety section
9. Breach response runbook (HBNR-compliant, 60-day clock)
10. Israel DPO appointment + PPA database registration (post-threshold)

---

## Risk Assessment

### Regulatory Risk Level: **MEDIUM**
- **Low** for FDA (clear General Wellness path post Jan 2026 update, as long as marketing discipline holds)
- **Low** for HIPAA (not a covered entity in B2C model)
- **Medium-High** for FTC (BetterHelp/Cerebral precedent makes mental-health-app data practices a known enforcement priority)
- **Medium-High** for WA MHMDA (private right of action makes plaintiff-side risk real, not just regulator-side)
- **Medium** for App Store / Play Store rejection (manageable with correct categorization + disclaimer)
- **Medium** for Israel Amendment 13 (manageable with fractional DPO + register at threshold)
- **Medium** for GDPR (only if EU launched; defer until US/Israel established)

### Specific Risks for Planny
1. **Marketing copy drift.** Founder, marketing hire, growth contractor, or influencer says "treats ADHD" — instantly creates FDA + FTC exposure. **Mitigation:** Written marketing language policy, single-page do/don't list, brand book includes regulatory red-lines.
2. **Ad pixel leakage on ADHD landing pages.** Meta/TikTok pixel on a "Planny for ADHD" landing page → fits the exact pattern FTC sued BetterHelp and GoodRx over. **Mitigation:** Either pixel-free landing pages for health-targeted campaigns, OR move to server-side conversion with hashed IDs + explicit consent.
3. **In-app symptom tracking creep.** Product team adds "log your focus score today." Now Planny has SaMD exposure, MHMDA expanded scope, and HBNR breach surface. **Mitigation:** Product review gate for any feature touching mood/focus/symptoms; requires legal sign-off.
4. **B2B2C partnership with clinic/coach.** Triggers HIPAA Business Associate status. **Mitigation:** Defer B2B2C until prepared, or scope partnerships as referral-only (no PHI flow).
5. **Apple App Store March 2026 health category designation.** If accidentally categorized as Health & Fitness, triggers medical device declaration requirement. **Mitigation:** File as Productivity from day one; document the decision.
6. **WA MHMDA private right of action.** Plaintiffs' firms are actively scanning health-adjacent apps. **Mitigation:** Get MHMDA right at launch (separate consent for collection and sharing, separate Health Data Privacy Policy, easy withdrawal).
7. **Israel DPO threshold creep.** Founder doesn't notice when Israeli user base crosses 10K. **Mitigation:** Quarterly compliance check-in once Israeli market exists.

### Lower-Likelihood Risks
- **Israel MoH inquiry:** Possible if Planny markets aggressively as "for ADHD" in Hebrew media; MoH could request clarification of non-medical status. Low probability, easy to resolve.
- **State AG action (CA/WA/NY):** Possible if breach occurs and notification is mishandled.
- **EU DPA investigation:** Only relevant if EU-launched without DPIA/consent compliance.

---

## Strategic Implications

1. **Categorize as Productivity in both stores. Document this decision in writing.** This is the single highest-leverage compliance choice. It avoids the Apple March 2026 medical device declaration, reduces reviewer scrutiny, preserves monetization flexibility, and aligns with how target users describe what they need (a planner that "gets" their brain, not a treatment).

2. **Write a Marketing Language Policy before the first growth dollar is spent.** One page, two columns (CAN say / CANNOT say). Every founder, marketer, contractor, agency, and influencer must sign-off. This is the cheapest, highest-impact regulatory control Planny will deploy — the FTC/FDA risk surface is 80% marketing copy.

3. **Architect for MHMDA from day one.** Separate Health Data Privacy Policy, separate consent for collection vs. sharing, easy withdrawal UX. Treat MHMDA as the floor; it covers CCPA SPI and most emerging state laws. Retrofit cost is 5-10x build-in cost.

4. **No third-party ad pixels on any page or screen that mentions ADHD/neurodivergent/mental-health.** Use server-side conversion with hashed IDs + explicit, separate consent if growth marketing needs attribution. This single rule eliminates the BetterHelp/Cerebral/GoodRx fact pattern.

5. **Stage international expansion by regulatory cost: US → Israel → EU.** US-only launch keeps compliance at ~$10-20K. Adding Israel adds modest cost (and the home market dynamic helps). EU is the most expensive — defer until Series A unless an EU growth thesis justifies it.

6. **Build a "regulatory tripwire" review for product features.** Any feature touching mood, focus, symptoms, medication, or clinical outputs requires legal/regulatory sign-off. Make this a Notion page or Linear template; it's a $0 control with high leverage.

---

## Source Quality Assessment

### Tier 1 (Government / Primary)
- FDA: 2026 General Wellness + CDS guidance documents
- FTC: BetterHelp order (2023), Cerebral order (2024), HBNR final rule (April 2024), GoodRx case
- Apple Developer: App Review Guidelines (latest)
- Google Play Console: Health Apps policy + Developer Program Policy
- Library of Congress: Israel Amendment 13 effective-date confirmation
- HHS: HIPAA guidance on health apps & APIs
- California OAG / CPPA: CCPA/CPRA materials
- WA RCW 19.373 (MHMDA full text)

### Tier 2 (Legal/Compliance — Generally Reliable)
- IAPP (International Association of Privacy Professionals)
- Cooley, DLA Piper, Wilson Sonsini, Alston & Bird, King & Spalding, Faegre Drinker, Latham & Watkins, Ropes & Gray, Arnold & Porter, Holland & Knight, Akin, Davis Wright Tremaine, Akerman — all major law-firm advisories
- Chambers Digital Healthcare Guide; ICLG Digital Health and Data Protection guides (Israel)
- BigID, Safetica, Accountable HQ (compliance vendors)
- HIPAA Journal; MedCity News; STAT News

### Tier 3 (Used Sparingly)
- myappmonitor.com blog (Google Play 2026 details — cross-checked against Play Console Help)
- dashsdk blog (Apple Health policies — cross-checked against Apple Developer News)
- General app-store-rejection roundups

### Overall Confidence by Section
- Apple/Google policy specifics: **Medium-High** (2026 changes well-documented but rapidly evolving)
- FDA SaMD boundary: **High** (Jan 6, 2026 guidance is final and broadly summarized by 6+ Tier-2 firms)
- HIPAA applicability: **High** (settled law)
- MHMDA: **High** (well-documented; private right of action is the key signal)
- CCPA/CPRA: **High**
- Israel Amendment 13: **Medium-High** (recent law, August 2025 effective; some implementation details still emerging via PPA guidance)
- GDPR Article 9: **High**
- FTC enforcement: **High** (multiple primary-source orders)
- Compliance cost estimates: **Medium** (synthesized from multiple Tier-2 sources; high variance based on legal-service choices)

---

## Data Gaps

1. **No ADHD-specific FDA enforcement letter** identified in this round. The closest analogs are Akili's EndeavorRx/EndeavorOTC (which intentionally pursued clearance) and FDA's silence on apps like Inflow that stay in wellness lane. Useful future search: "FDA warning letter ADHD app" / "FDA untitled letter cognitive app."
2. **No public FTC action against a productivity-marketed-to-ADHD app yet.** The BetterHelp/Cerebral/GoodRx cases are mental-health adjacent but not direct precedent for Planny's exact positioning. This is good (no precedent against us) and ambiguous (less guidance on exact red lines).
3. **Israel PPA enforcement posture under Amendment 13.** Law is only ~9 months in effect; enforcement patterns are still developing. The fractional-DPO market and PPA registration mechanics could shift.
4. **App Store rejection rate for ADHD-labeled apps** is not publicly tracked. Anecdotal evidence (Inflow, Tiimo, Routinery — all live) suggests it is navigable with disciplined positioning.
5. **EU AI Act exposure** for Planny's AI scheduling features was not researched in this round. The AI Act's "limited risk" tier may apply (transparency obligations); a "high-risk" classification is unlikely for a scheduling tool but worth confirming if EU launch nears. **Recommended for a future research round.**
6. **Apple Privacy Manifest specific requirements for ADHD/mental-health metadata** — was not deep-researched; likely needs a developer-side review at app submission.

---

## Flags

### Red Flags (Action Required)
1. **Any marketing copy claim of treatment/improvement of ADHD/focus = automatic FDA/FTC risk.** Build a written marketing language policy BEFORE the first growth dollar.
2. **Third-party ad pixels (Meta, TikTok, Google) on pages mentioning ADHD = BetterHelp/Cerebral fact pattern.** This is the single highest-likelihood enforcement vector. Default position: no pixels on ADHD landing pages.
3. **WA MHMDA private right of action** — plaintiffs' firms are actively trolling. Get separate health-data consent + separate Health Data Privacy Policy at launch, not later.
4. **App Store category Health & Fitness or Medical = triggers Apple March 2026 medical device declaration requirement.** Category as Productivity from day one.
5. **Adding symptom/mood tracking features** could move Planny from General Wellness into SaMD territory. Product gate required.

### Yellow Flags (Monitor)
1. **Israel Amendment 13 enforcement patterns** are still developing — monitor PPA bulletins quarterly.
2. **California 2025 CCPA amendments** add cybersecurity audit and risk assessment requirements phasing in 2027-2028 — budget for this in Year 2-3.
3. **FTC may issue an ADHD-app-specific guidance** given Adderall telehealth scandals (Cerebral, Done). Monitor FTC blog.
4. **Google Play Organization Account verification** — recommended even if categorized as Productivity, for liability separation.
5. **EU AI Act** — transparency obligations may apply to Planny's AI features. Research before EU launch.
6. **B2B2C partnerships** (clinics, coaches, insurers) trigger HIPAA. Defer or scope carefully.

---

## Sources

- [FDA — General Wellness: Policy for Low Risk Devices (2026)](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/general-wellness-policy-low-risk-devices)
- [FDA — Clinical Decision Support Software (2026)](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/clinical-decision-support-software)
- [FDA — Device Software Functions Including Mobile Medical Applications](https://www.fda.gov/medical-devices/digital-health-center-excellence/device-software-functions-including-mobile-medical-applications)
- [FTC — BetterHelp Order, March 2023](https://www.ftc.gov/news-events/news/press-releases/2023/03/ftc-ban-betterhelp-revealing-consumers-data-including-sensitive-mental-health-information-facebook)
- [FTC — BetterHelp Final Order, July 2023](https://www.ftc.gov/news-events/news/press-releases/2023/07/ftc-gives-final-approval-order-banning-betterhelp-sharing-sensitive-health-data-advertising)
- [FTC — Cerebral Refunds Release, May 2025](https://www.ftc.gov/news-events/news/press-releases/2025/05/more-5-million-refunds-sent-consumers-result-ftcs-action-against-cerebral-over-deceptive)
- [FTC — Updated Health Breach Notification Rule, April 2024](https://www.ftc.gov/business-guidance/blog/2024/04/updated-ftc-health-breach-notification-rule-puts-new-provisions-place-protect-users-health-apps)
- [FTC — Health Breach Notification Rule (full)](https://www.ftc.gov/legal-library/browse/rules/health-breach-notification-rule)
- [FTC — Consumer Health Information Blog, April 2024](https://www.ftc.gov/business-guidance/blog/2024/04/consumer-health-information-handle-extreme-care)
- [Apple Developer — App Review Guidelines](https://developer.apple.com/app-store/review/guidelines/)
- [Apple Developer — App Store Categories](https://developer.apple.com/app-store/categories/)
- [Apple — Apple Health App & Privacy Legal](https://www.apple.com/legal/privacy/data/en/health-app/)
- [Telehealth.org — Apple Health App Rules Expand 2026](https://telehealth.org/news/apple-expands-health-app-requirements-as-fda-loosens-oversight-of-wearable-technologies/)
- [Google Play Console — Health Content and Services](https://support.google.com/googleplay/android-developer/answer/16679511?hl=en)
- [Google Play Console — Health App Categories](https://support.google.com/googleplay/android-developer/answer/13996367?hl=en)
- [My App Monitor — Google Play Health Apps Update Jan 2026](https://myappmonitor.com/blog/google-play-health-apps-update-2026-requirements)
- [Google Play Policy Announcement, April 15, 2026](https://support.google.com/googleplay/android-developer/answer/16926792?hl=en)
- [HHS — The Access Right, Health Apps, and APIs](https://www.hhs.gov/hipaa/for-professionals/privacy/guidance/access-right-health-apps-apis/index.html)
- [NYSBA — Mental Health Apps and HIPAA](https://nysba.org/telehealth-via-tiktok-is-not-protected-under-hipaa-but-zoom-is-what-attorneys-need-to-know-about-mental-health-apps/)
- [CA OAG — CCPA](https://oag.ca.gov/privacy/ccpa)
- [CPPA — FAQs](https://cppa.ca.gov/faq.html)
- [IAPP — CPRA Sensitive Data Opt-Out](https://iapp.org/news/a/new-categories-new-rights-the-cpras-opt-out-provision-for-sensitive-data)
- [WA RCW 19.373 — My Health My Data Act](https://app.leg.wa.gov/RCW/default.aspx?cite=19.373&full=true)
- [IAPP — Washington MHMDA Overview](https://iapp.org/resources/article/washington-my-health-my-data-act-overview)
- [Cooley — MHMDA FAQ Part One](https://cdp.cooley.com/washington-states-my-health-my-data-act-faq-part-one-applicability-and-scope/)
- [EFF — How to Build on Washington's My Health My Data Act](https://www.eff.org/deeplinks/2025/06/how-build-washingtons-my-health-my-data-act)
- [Library of Congress — Israel Amendment 13 Goes Into Effect](https://www.loc.gov/item/global-legal-monitor/2025-11-17/israel-amendment-to-privacy-protection-law-goes-into-effect/)
- [IAPP — Israel Amendment 13 Reform](https://iapp.org/news/a/israel-marks-a-new-era-in-privacy-law-amendment-13-ushers-in-sweeping-reform)
- [Safetica — Israel Amendment 13 Explained](https://www.safetica.com/resources/guides/israel-s-amendment-13-what-the-new-data-protection-law-means-for-your-business)
- [BigID — Israel Amendment 13](https://bigid.com/blog/what-israel-amendment-13-means-for-businesses-in-2025/)
- [ICLG — Digital Health Israel 2025](https://iclg.com/practice-areas/digital-health-laws-and-regulations/israel)
- [ICLG — Data Protection Israel 2025-2026](https://iclg.com/practice-areas/data-protection-laws-and-regulations/israel)
- [Chambers — Digital Healthcare 2025 Israel](https://practiceguides.chambers.com/practice-guides/digital-healthcare-2025/israel)
- [Emergo by UL — Israel Medical Device Registration](https://www.emergobyul.com/services/medical-device-registration-and-approval-israel)
- [GDPR-info — Article 9 Special Categories](https://gdpr-info.eu/art-9-gdpr/)
- [Faegre Drinker — Key Updates in FDA's 2026 Guidance](https://www.faegredrinker.com/en/insights/publications/2026/1/key-updates-in-fdas-2026-general-wellness-and-clinical-decision-support-software-guidance)
- [King & Spalding — FDA Updates 2026](https://www.kslaw.com/news-and-insights/fda-updates-general-wellness-and-clinical-decision-support-guidance-documents)
- [Ropes & Gray — FDA Adapts on Digital Health](https://www.ropesgray.com/en/insights/alerts/2026/01/fda-adapts-with-the-times-on-digital-health-updated-guidances-on-general-wellness-products)
- [Latham & Watkins — FDA Loosens Digital Health Approach](https://www.lw.com/en/insights/fda-issues-updated-guidance-loosening-regulatory-approach-to-certain-digital-health-tools)
- [Akin — FDA Issues Key Guidance Updates](https://www.akingump.com/en/insights/blogs/eye-on-fda/fda-issues-key-guidance-updates-for-digital-health-and-wellness)
- [Arnold & Porter — Telehealth Enforcement Advisory Dec 2024](https://www.arnoldporter.com/en/perspectives/advisories/2024/12/government-enforcement-of-telehealth-providers)
- [Wilson Sonsini — FTC HBNR Final Rule](https://www.wsgr.com/en/insights/ftc-final-rule-officially-broadens-health-breach-notification-rule-targets-health-and-wellness-apps.html)
- [Alston & Bird — FTC HBNR Now in Effect](https://www.alston.com/en/insights/publications/2024/08/ftc-updated-health-breach-notification-rule)
- [Holland & Knight — Lessons from BetterHelp Enforcement](https://www.hklaw.com/en/insights/publications/2023/03/lessons-learned-from-ftc-enforcement-action-against-betterhelp)
- [STAT — Cerebral $7M Fine](https://www.statnews.com/2024/04/15/ftc-fines-cerebral-telehealth-health-data-sharing/)
- [MedCity News — Cerebral $7M Fine Analysis](https://medcitynews.com/2024/04/cerebral-data-privacy-mental-health/)
