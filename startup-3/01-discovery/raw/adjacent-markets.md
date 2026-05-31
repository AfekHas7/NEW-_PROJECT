# Adjacent Markets & Expansion — Research Agent A4

**Startup context:** AI-native service company that prepares companies for ISO 9001 audits (beachhead). Israel-first, then global.
**Core question:** Which adjacent certifications/verticals are the best expansion paths after ISO 9001, and where is the whitespace?
**Date of research:** 2026-05-31
**Method:** 8 WebSearch queries across 4 sequential rounds. Figures cross-referenced where possible; all are vendor/market-research estimates unless from the ISO Survey (the authoritative count).

---

## Headline numbers (anchor data)

**ISO Survey — global valid certificates (authoritative, from ISO/IAF CertSearch):**

| Standard | Domain | 2023 certs | 2024 certs | Trend |
|---|---|---|---|---|
| ISO 9001 | Quality | 837,052 | ~830k (flat) | Mature, huge installed base; flat-to-slight-decline (China data gap distorts) |
| ISO 14001 | Environmental | 300,410 | ~300k | Mature, steady |
| ISO 45001 | Occupational H&S | 185,166 | ~190k | Steady growth |
| ISO/IEC 27001 | Information security | 48,671 | **96,709** | **~doubled YoY**; 179,877 certified sites; CAGR 20.3% (2018-24) |
| ISO/IEC 42001 | AI management | (n/a, pub. Dec 2023) | ~100+ orgs | Brand-new, explosive interest |

Key fact: **ISO 27001 nearly doubled in one year (48.7k → 96.7k)** while ISO 9001 (10x larger base) is flat. This is the single most important demand signal in the dataset.

**Market-size estimates (vendor reports — treat as directional, wide variance):**
- ISO 27001 *certification market*: ~USD 18.6B (2025) → USD 74.6B (2035), CAGR ~15.2% (Business Research Insights).
- Overall ISO certification *services* market: ranges wildly across firms — USD 10.3B (2024, Cognitive, 15% CAGR) to USD 13.1B (2025, ~11.6% CAGR) to USD 35.6B (2025, 6.5% CAGR). **Data gap / low confidence** — see below.
- Medical devices market (downstream of ISO 13485): USD 536B (2023) → USD 800B (2030), ~14% CAGR.
- AI governance software market: → USD 15.8B by 2030, ~30% CAGR.

---

## 1. Adjacent Standards Profiles

### ISO/IEC 27001 — Information Security — **TIER 1**
- **Market size:** Hottest growing standard. ~96.7k certs (2024), doubled YoY; cert-services market ~USD 18.6B (2025) at ~15% CAGR. Driven by cyber threat escalation, NIS2 (EU supply-chain enforcement), AI regulation, and GDPR.
- **Competition:** **Intense.** Vanta, Drata, Secureframe, Scytale, Sprinto — well-funded automation platforms saturate this space. They lead with SOC 2 + ISO 27001 + HIPAA + GDPR.
- **Regulatory risk:** Low/manageable; mandatory migration to 27001:2022 closed Oct 31 2025 (a one-time demand pulse, now passed).
- **Fit with AI-native model:** High — heavily documentation- and evidence-driven; but incumbents already own the AI-automation narrative here.
- **Sequencing:** First expansion, BUT enter as a *cross-sell to existing 9001 clients* rather than head-to-head with Vanta/Drata. Israel angle is strong: Check Point, Mobileye ecosystem; startups need 27001 for VC + EU contracts.

### SOC 2 — (AICPA attestation, not ISO) — **TIER 1 (adjacent, US-facing)**
- **Market:** SOC 2 is the *default first request* in US B2B procurement; ISO 27001 preferred by EU/international buyers. SMBs can hit SOC 2 Type I in months — lighter org change than 27001.
- **Competition:** Same incumbents (Vanta/Drata born here). Extremely crowded.
- **Fit:** High, but this is the incumbents' home turf. Relevant mainly because Israeli SaaS selling to US needs it. Treat as a bundled add-on, not a standalone wedge.

### ISO/IEC 42001 — AI Management System — **TIER 1 (whitespace play)**
- **Market:** Published Dec 2023; ~100+ orgs certified within 18 months (Microsoft, Google Cloud, AWS, SAP, KPMG). AI governance software → USD 15.8B by 2030 (~30% CAGR). 76% of orgs in a CSA 2025 benchmark plan to pursue it.
- **Competition:** **LOW — early, fragmented.** No dominant automation player yet. This is genuine whitespace.
- **Regulatory risk:** Tailwind, not risk — EU AI Act + AI procurement requirements pull demand.
- **Fit with AI-native model:** **Exceptional / on-brand.** An "AI-native company that certifies your AI management system" is a coherent, defensible story. Strong narrative fit for an AI-native services startup.
- **Sequencing:** High-priority *parallel* bet alongside 27001. Highest strategic optionality.

### ISO 13485 — Medical Device QMS — **TIER 2 (high-value vertical)**
- **Market:** High-value, regulatory-mandated. **FDA adopts ISO 13485 into its QMSR rule (effective Feb 2026)** — a major US demand catalyst. Certified firms 40% more successful at international market approvals (Deloitte 2024 MedTech). Downstream medtech market ~USD 800B by 2030.
- **Competition:** Specialist consultancies (MasterControl, Qualityze, etc.); fewer AI-native players. Moderate.
- **Regulatory risk:** **High** — life-safety, FDA/MDR oversight; errors carry liability. Demands deep domain expertise; harder to fully automate.
- **Fit:** Medium — 13485 is built on the ISO 9001 QMS backbone (natural adjacency), but the regulatory depth limits pure-AI automation. Best as expert-augmented AI.
- **Israel angle:** Strong — Israel has a dense med-tech/biotech cluster. Good local beachhead-within-beachhead.

### ISO 14001 (Environmental) + ISO 45001 (OH&S) — **TIER 2 (cluster cross-sell)**
- **Market:** Mature, steady (~300k and ~185k certs). Not high-growth.
- **Competition:** Commoditized consulting.
- **Fit:** **High structural fit** — share the ISO High-Level Structure (HLS) with 9001, so an Integrated Management System (IMS) is the natural cross-sell. Low growth but high attach-rate to existing 9001 clients = revenue expansion, not new logos.
- **Sequencing:** Cross-sell, not a standalone wedge.

### ISO 22000 (Food Safety), IATF 16949 (Automotive), AS9100 (Aerospace) — **TIER 3 (vertical extensions)**
- All sit *on top of* an ISO 9001 QMS foundation — "ISO 9001 is a non-negotiable prerequisite" in automotive/aerospace/medical.
- Niche, deep-domain, slower-growing. Defer until the QMS engine is proven and a vertical pulls demand. ISO 22000 relevant to Israel's agrifood/beverage sector.

### GDPR / Privacy (ISO 27701) — **TIER 2 (compliance-doc adjacency)**
- Documentation-heavy, EU-driven, pairs with 27001. Good AI-native fit; bundled add-on for Israeli firms selling into EU.

---

## 2. Cross-sell Clustering

**The IMS (Integrated Management System) thesis is the core cross-sell engine.** Since 2015 all ISO management standards share a common High-Level Structure (context, leadership, planning, support, operation, evaluation, improvement) — clause numbers and core requirements align. An org running 9001+14001+45001+27001 can use *one* leadership statement, *one* risk methodology, *one* internal-audit programme, *one* management review.

**Implication for the AI-native model:** Once you have a client's QMS documented for ISO 9001, ~60-70% of the structural scaffolding for 14001/45001/27001/42001 is reusable. This is a powerful land-and-expand motion and a real moat — the AI keeps the client's "document graph," which competitors entering at a single-standard level cannot match.

**Natural cluster groupings observed:**
- **Quality/Ops cluster:** 9001 → 14001 → 45001 (+ IATF 16949 / AS9100 / 22000 by vertical). Same buyer (Ops/Quality manager). Easiest cross-sell.
- **Security/Trust cluster:** 27001 → SOC 2 → 27701/GDPR → 42001. Different buyer (CISO/CTO), but the hottest growth.
- **Israel reality:** Tech firms "combine ISO 9001 + ISO 27001" routinely (operational excellence + data security). IQC, Israel's largest private cert body, has ~7,000 customers across standards — confirms multi-standard demand locally.

---

## 3. Whitespace Analysis

**Verified whitespace #1 — ISO 9001 itself is the underserved beachhead (CONFIRMED).** The compliance-automation incumbents (Vanta, Drata, Secureframe, Scytale, Sprinto) target **SOC 2, ISO 27001, HIPAA, GDPR**. **ISO 9001 (quality) is notably absent from both Vanta's and Drata's core offerings.** Meanwhile ISO 9001 has the largest installed base by far (~830k certs vs 27001's ~97k). The startup's beachhead choice is validated: huge market, no AI-native incumbent.

**Verified whitespace #2 — ISO 42001 (AI management).** Brand-new (Dec 2023), exploding interest, no dominant automation platform. An AI-native vendor certifying AI management systems is uniquely credible. Strongest *forward* whitespace.

**Underserved-SMB pain (CONFIRMED).** ISO 9001 consulting runs USD 2,500-10,000+ for a consultant and USD 5,000-15,000+ total; consultants bill USD 300-1,000/hr. SMBs distrust consultants ("more adept at spending their money than getting a working system") and believe certification needs big budgets/teams. This is the exact wedge for an AI-native, outcome-priced service — and the pain repeats across *every* standard, so the whitespace is replicable as you expand.

**Comparable proof points (AI-native services replacing professional services):**
- VC Cafe (May 2026): "AI-Native Services: The New Startup Playbook" — companies that look like accounting/legal/compliance firms but are software selling *outcomes, not seats*.
- Harvey (legal AI): ~USD 190M ARR (Jan 2026), USD 11B valuation (Mar 2026).
- Minerva (YC): AI-native accounting firm aiming to replace SMB bookkeeping/tax.
- YC 2025 RFS explicitly: "start your own law firm, staff it with AI agents."
- Thesis: AI-native services are "especially powerful for SMBs — too big to ignore compliance work, too small to hire full-time experts." **Directly matches the ISO 9001 SMB wedge.**

---

## 4. Expansion Sequencing Recommendation

**Phase 0 (now):** ISO 9001 beachhead. Confirmed whitespace, largest base, no AI-native incumbent. Build the reusable "document graph" engine.

**Phase 1 (first expansion, 6-18 mo) — IMS cross-sell within existing accounts:** Add **ISO 14001 + ISO 45001**. Same buyer, shared HLS, ~60-70% scaffold reuse, low competition, low regulatory risk. Revenue expansion with minimal new GTM. *Israel:* manufacturing/construction/logistics demand.

**Phase 2 (parallel high-growth bet) — ISO/IEC 27001 + SOC 2 + ISO/IEC 42001:**
- 27001/SOC 2: enter as a *cross-sell to 9001 clients*, NOT head-to-head with Vanta/Drata. Leverage Israeli tech/cyber density and VC/EU-contract demand.
- **42001 is the priority within this phase** — genuine whitespace, perfect AI-native narrative fit, regulatory tailwind. Highest strategic optionality.

**Phase 3 (vertical depth, 18-36 mo) — ISO 13485 (med-device):** High value, FDA QMSR tailwind (Feb 2026), dense Israeli med-tech cluster — but high regulatory risk; deploy as expert-augmented AI, not full automation. Defer until QMS engine and risk controls are mature.

**Phase 4 (opportunistic verticals):** IATF 16949, AS9100, ISO 22000, ISO 27701/GDPR — pulled by specific customer demand only. All sit on the 9001 foundation, so technically cheap to add; gate on demand, not capability.

**One-line strategy:** Win 9001 (whitespace), expand via IMS cluster (cheap, sticky), bet on 42001 (future whitespace + brand fit), go deep on 13485 (high value) only when ready for regulatory rigor.

---

## 5. Data Gaps & Caveats

1. **ISO cert-services market size is unreliable.** Vendor estimates range from USD 10.3B to USD 35.6B for roughly the same year with CAGRs from 6.5% to 16%. These are syndicated-report figures, not audited. Treat all dollar TAMs as directional only. The **ISO Survey certificate counts are the trustworthy anchor.**
2. **2024 ISO Survey for 9001/14001/45001 not cleanly captured** — 2023 figures used; 2024 likely flat/slightly down, distorted by missing China accreditation data. ISO 9001's real installed base is larger than reported.
3. **ISO 42001 certification counts are nascent** ("100+ orgs") — no formal ISO Survey line yet. Growth is qualitative/anecdotal but consistent across sources.
4. **No hard data on % of companies holding multiple ISO certs simultaneously** — IMS demand is well-documented qualitatively (shared HLS, IQC's ~7,000 multi-standard customers) but no clean overlap statistic found.
5. **Israel-specific certificate counts not isolated** — only qualitative (strong cyber/medtech/tech demand; IQC largest local body). Recommend a follow-up pull from the ISO Survey country breakdown for Israel-specific 9001/27001 counts.
6. **ISO 13485 standalone market size not isolated** from the broader ISO/medical-device markets; used downstream medtech market (~USD 800B by 2030) as a proxy.
7. WebSearch is US-only; Israel/EU-specific demand signals are under-sampled and should be validated with local primary research (IQC, SII/Standards Institution of Israel).

---

## Sources

- [ISO 27001 Certification Market — Business Research Insights](https://www.businessresearchinsights.com/market-reports/iso-27001-certification-market-120318)
- [ISO Certification Market — 360 Research Reports](https://www.360researchreports.com/market-reports/iso-certification-market-205579)
- [ISO 13485 Certification 2026 / FDA QMSR — Pacific Cert](https://blog.pacificcert.com/iso-13485-certification-medical-devices-components/)
- [Future Trends in ISO 13485 — Smithers (Nov 2025)](https://www.smithers.com/resources/2025/november/trends-in-iso-13485-for-medical-device-suppliers)
- [SOC 2 vs ISO 27001 — Sprinto](https://sprinto.com/blog/soc-2-vs-iso-27001/)
- [SOC 2 vs ISO 27001 (2026) — soc2auditors.org](https://soc2auditors.org/insights/soc-2-vs-iso-27001/)
- [Integrated Management Systems — Standarity](https://standarity.com/blog/integrated-management-systems-ims)
- [Integrated ISO 9001/14001/45001/27001 IMS — CCS Risk](https://ccsrisk.com/iso-ims)
- [What the 2023 ISO Survey Tells Us — simpleQuE](https://www.simpleque.com/what-does-the-2023-iso-survey-tell-us-about-iso-9001-iso-14001-and-iso-45001-certifications/)
- [A Look at the 2024 ISO Survey — simpleQuE](https://www.simpleque.com/a-look-at-the-2024-iso-survey-and-iso-9001-iso-14001-and-iso-45001-certifications-worldwide/)
- [ISO 27001 Certifications Nearly Double in 2024 — HEIC](https://heic.eu/iso-27001-certifications-nearly-double-in-2024-as-global-organizations-prioritize-cybersecurity/)
- [Best ISO 27001 Compliance Software — Vanta](https://www.vanta.com/resources/best-iso-27001-compliance-software)
- [Best AI Compliance Tool for ISO 27001 — Scytale](https://scytale.ai/resources/best-ai-compliance-tool/)
- [ISO 9001 Certification Cost for Small Businesses — BPRHub](https://www.bprhub.com/blogs/iso-9001-certification-cost-for-small-businesses)
- [ISO 9001 for Small Business — NQA](https://www.nqa.com/en-us/resources/blog/april-2026/iso-9001-for-small-businesses)
- [ISO Certification Service Market — Dataintelo](https://dataintelo.com/report/iso-certification-service-market)
- [ISO/IEC 42001:2023 Certification Trends — Certiget](https://www.certiget.eu/en/guides/iso-42001-2023-certification-aims)
- [KPMG first Big Four to attain ISO 42001 — KPMG (Dec 2025)](https://kpmg.com/xx/en/media/press-releases/2025/12/kpmg-international-first-to-attain-iso-certification-for-ai-management-systems.html)
- [ISO 42001 — ANAB/ANSI](https://anab.ansi.org/accreditation/iso-iec-42001-artificial-intelligence-management-systems/)
- [AI-Native Services: The New Startup Playbook — VC Cafe (May 2026)](https://www.vccafe.com/2026/05/06/ai-native-services-the-new-startup-playbook/)
- [Harvey valued at $11B — CNBC (Mar 2026)](https://www.cnbc.com/2026/03/25/legal-ai-startup-harvey-raises-200-million-at-11-billion-valuation.html)
- [Minerva: AI native accounting firm — Y Combinator](https://www.ycombinator.com/companies/minerva)
- [ISO Certifications in Israel — Pacific Certifications](https://blog.pacificcert.com/iso-certifications-in-israel/)
- [IQC — Institute of Quality & Control (Israel)](https://www.iqc.co.il/?categoryId=134565)
- [Cognitive Market Research — ISO Certification Market](https://www.cognitivemarketresearch.com/iso-certification-market-report)
