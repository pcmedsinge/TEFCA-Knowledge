# CONTENT.md — Verified Facts for TEFCA + FHIR + Clinical AI Hub

> Every claim that appears in `index.html` must originate here, with a source. If it's not sourced, it's not published.

> **Last verified:** April 23, 2026
> **Next re-verification:** Before Phase 1 publication, then before every v0.x release

---

## Section 1 — Governance & Oversight

### 1.1 Oversight body naming (current as of April 2026)
- Current name: **ONC** — Office of the National Coordinator for Health Information Technology
- Effective **March 31, 2026**, HHS reinstated ONC and dropped the "ASTP/ONC" dual title that had been in place since July 2024
- The National Coordinator role was also un-merged from the Assistant Secretary for Technology Policy role
- CTO, CAIO, CDO roles moved back under HHS OCIO
- **Source:** DistilINFO Publications, "HHS Reinstates ONC, Ends ASTP Dual Title", April 2026 — https://distilinfo.com/2026/04/06/hhs-reinstates-onc-ends-astp-dual-title/
- **Also confirmed:** ONC/TEFCA official page — https://healthit.gov/policy/tefca/ (refers to ONC)
- **Historical note for the app:** From July 2024 to March 2026, the office was "ASTP/ONC" (Assistant Secretary for Technology Policy / Office of the National Coordinator for Health IT). Many 2024–2025 documents still use this title.

### 1.2 Recognized Coordinating Entity (RCE)
- **The Sequoia Project** — reselected August 2025 to continue as RCE
- Operates under contract with ONC; 5-year contract originally awarded August 2023
- **Source:** https://rce.sequoiaproject.org/ and https://healthit.gov/policy/tefca/

### 1.3 Governing documents (current versions)
- **Common Agreement v2.1** — released November 2024
  - Source: https://rce.sequoiaproject.org/tefca/
  - v2.0 was originally published in the Federal Register May 1, 2024; v2.1 superseded it November 2024
- **QHIN Technical Framework (QTF) v2.1** — current
  - Source: TEFCA Glossary (Jan 2026) — https://rce.sequoiaproject.org/wp-content/uploads/2026/01/TEFCA-Glossary_Jan-2026-v2_508.pdf
- **Participant/Subparticipant Terms of Participation v1.0**
  - Source: TEFCA Glossary (Jan 2026)

---

## Section 2 — QHINs (Qualified Health Information Networks)

### 2.1 Current count
- **11 Designated QHINs** as of November 2025 / early 2026
- **Source:** "New Designated QHIN, New SOPs, and More" — RCE — https://rce.sequoiaproject.org/new-designated-qhin-new-sops-and-more/

### 2.2 Designated QHINs list (all 11 confirmed; verified against RCE Designated QHINs page on 2026-04-23)

Listed in chronological order of designation. Note: the RCE page lists alphabetically; the chronological order below was reconstructed from individual designation announcements.

| # | QHIN | Designated |
|---|---|---|
| 1 | eHealth Exchange | Dec 2023 |
| 2 | Epic Nexus | Dec 2023 |
| 3 | Health Gorilla | Dec 2023 |
| 4 | KONZA | Dec 2023 |
| 5 | MedAllies | Dec 2023 |
| 6 | CommonWell Health Alliance | Feb 2024 |
| 7 | Kno2 | Feb 2024 |
| 8 | eClinicalWorks (Prismanet) | Jan 16, 2025 |
| 9 | Surescripts | April 2025 |
| 10 | Netsmart | Aug 6, 2025 |
| 11 | Oracle Health Information Network | November 2025 (4th and final designated in 2025) |

**Naming variations on the RCE page (for reference):** CommonWell Health Alliance appears as "CommonWell Alliance"; KONZA as "Konza Health"; MedAllies as "Medallies"; Kno2 as "KNO2"; Epic Nexus as "Epic (Epic Nexus)"; Surescripts as "Surescripts (Health Information Network/Interconnect)"; eClinicalWorks as "eClinicalWorks (Prismanet)".

- **Source (list):** https://rce.sequoiaproject.org/designated-qhins/ (authoritative, live list — verified 2026-04-23)
- **Sources (dates):**
  - Dec 2023 launch: TEFCA "Big Bang" go-live Dec 12, 2023
  - Feb 2024 CommonWell + Kno2: HCI Innovation Group — https://www.hcinnovationgroup.com/interoperability-hie/trusted-exchange-framework-and-common-agreement-tefca/news/53096295/list-of-tefca-qhins-grows-to-seven
  - eClinicalWorks Jan 2025: RCE press release — https://rce.sequoiaproject.org/astp-and-the-sequoia-project-designate-eclinicalworks-as-qhin/
  - Surescripts April 2025, Oracle Nov 2025: Healthcare Dive — https://www.healthcaredive.com/news/oracle-health-qhin-designation-tefca/806217/
  - Netsmart Aug 2025: RCE press release — https://rce.sequoiaproject.org/astp-and-the-sequoia-project-designate-netsmart-as-qhin/

### 2.3 Candidate QHINs
- Additional organizations are in the onboarding/testing phase at any given time
- **Source:** https://rce.sequoiaproject.org/candidate-qhins/
- **Action:** Check this page during Phase 0 for current candidate list

---

## Section 3 — Exchange Purposes (all 6)

The six Exchange Purposes (XPs) currently recognized under TEFCA:

1. **Treatment** — 45 CFR § 164.501 definition
   - XP Implementation SOP: Treatment v1.2 (released 1/16/2026)
2. **Payment**
3. **Health Care Operations**
4. **Public Health**
5. **Individual Access Services (IAS)** — services to individuals so they can access their own records
   - IAS Provider Requirements SOP v2.1 (released 3/17/2026)
6. **Government Benefits Determination** — NEW, released 2025
   - XP Implementation SOP: Government Benefits Determination v1.0
   - Supports SSA disability determination (SSDI title II, SSI title XVI)
   - Goal: replace weeks/months of record retrieval with minutes/seconds
   - **Source:** https://healthit.gov/blog/insights-updates/tefca-government-benefits-determination-implementation-is-here/
   - **Also:** https://rce.sequoiaproject.org/new-designated-qhin-new-sops-and-more/

---

## Section 4 — Technical Reality (2026)

### 4.1 Document-based exchange is still the dominant mode
- **Critical honesty point for the app:** Most TEFCA exchange in 2026 is still **document-based (C-CDA XML), not native FHIR**
- Quote-source (paraphrased): The current exchange through TEFCA is document-based. Records are exchanged as CDA and C-CDA XML documents, not native FHIR resources.
- **Source:** Dynamic Health IT recap of 2026 ASTP Annual Meeting — https://dynamichealthit.com/post/2026-astp-annual-meeting/

### 4.2 FHIR migration in progress (Facilitated FHIR)

**Document trail:**
- **Facilitated FHIR Implementation SOP v2.0** released as DRAFT 3/8/2026
- An earlier draft of v2.0 was published in October 2025
- Older Facilitated FHIR Implementation Guide drafts go back to 2022 (Draft 1 in October 2022, Draft 2 pilot in December 2022)
- **Sources:**
  - SOP v2.0 Draft (March 2026): https://rce.sequoiaproject.org/wp-content/uploads/2026/02/SOP-Facilitated-FHIR-Implementation-2.0-Draft-508.pdf
  - SOP v2.0 Draft (October 2025 — earlier iteration): https://rce.sequoiaproject.org/wp-content/uploads/2025/10/SOP-Facilitated-FHIR-Implementation-2.0-Draft-October_508.pdf
  - 2026-02-19 ONC TEFCA Updates Presentation: https://www.healthit.gov/wp-content/uploads/2026/02/2026-02-19_TEFCA_Updates_Presentation.pdf
  - RCE "TEFCA on FHIR" overview page (verified 2026-04-24): https://rce.sequoiaproject.org/rce-tefca-on-fhir/

**What Facilitated FHIR enables:**
- Allows organizations to conduct FHIR transactions directly with other TEFCA participants **without a prior bilateral connection** — that's the "facilitated" part
- Network-scaled trust establishment via UDAP-based client registration (vs the per-pair manual onboarding required for legacy direct integrations)

**Security framework:**
- **Required spec:** "HL7 UDAP Security for Scalable Registration, Authentication, and Authorization Implementation Guide" — the formal name used in the RCE TEFCA on FHIR page; sometimes shortened to UDAP SSRAA in industry coverage
- **Flow:** The Initiating Node uses a TEFCA-issued certificate to assert identity, registers as a UDAP Trusted Client (gets a `client_id`), authenticates, receives an access token, then queries the Responding Node's FHIR server
- **Permission window:** UDAP-based registration / authentication / authorization permitted through **2027** per SOP v2.0 Draft
- **Note on unverified claim:** Search summaries occasionally describe a "January 1, 2026 HL7 FAST deadline for QHINs to implement FAST security protocols for FHIR." This claim is **not corroborated** by the RCE TEFCA on FHIR page. Treat as unverified — do not cite without primary-source confirmation.

**Endpoint discovery:**
- FHIR endpoints are registered in the **RCE Directory Service** (operated by The Sequoia Project)
- Initiating Nodes look up Responding Node endpoints via the Directory before initiating exchange
- Quote (RCE): "facilitated by usage of the RCE® Directory Service for scalable endpoint discovery"

**FHIR baseline:**
- **FHIR Release 4** with **HL7 FHIR US Core Implementation Guide v3.1.1** required (per RCE TEFCA on FHIR page)

**Typical FHIR resources used in TEFCA flows** (per US Core v3.1.1 Treatment scenarios):
- `Patient` — identification and demographics, anchor of every query
- `DocumentReference` — pointer to clinical documents (often C-CDA documents wrapped as binary attachments — bridges the document/FHIR worlds)
- `Consent` — patient consent records (referenced in `consent_reference` arrays in some IAS flows)
- `Bundle` — packaging multiple resources for a single response
- `MedicationRequest`, `AllergyIntolerance`, `Condition`, `Observation`, `ImagingStudy`, `DiagnosticReport`, `Encounter` — domain resources commonly returned for Treatment-purpose queries

**Methodology note:** Resource list above reflects standard US Core v3.1.1 usage patterns for Treatment-purpose exchanges. The Facilitated FHIR SOP v2.0 PDF could not be text-extracted in this environment (binary encoding); for Phase 3 publication, a manual review of the SOP is recommended to confirm any specific resource subsets, profiles, or extensions mandated.

### 4.3 USCDI requirement
- **Effective January 1, 2026:** all data created or captured and sent via TEFCA must conform to **USCDI v3**
- Prior requirement was USCDI v1 for data on/after Dec 31, 2024
- For FHIR exchange: **HL7 FHIR US Core Implementation Guide v3.1.1 or higher**
- **Source:** TEFCA RCE FAQs — https://rce.sequoiaproject.org/rce/faqs/

### 4.4 IHE profiles currently used (verified against QTF v2.1 references, 2026-04-24)

**XCPD — Cross-Community Patient Discovery**
- "QHINs MUST implement the IHE XCPD profile for QHIN Patient Discovery."
- Function: locate the communities that hold relevant patient health data; correlate patient identifiers across communities holding the same patient's data
- This is the patient-matching layer — what makes cross-QHIN queries possible at all

**XCA — Cross-Community Access**
- Function: query and retrieve patient health data held by other communities, in the form of documents
- Inputs: requires knowledge of patient identity (from XCPD result) and the HomeCommunityID of the Responding Node when querying for and retrieving clinical documents
- This is the document-fetch layer — once XCPD says "patient X has records in community Y," XCA fetches them

**Together:** XCPD + XCA are the backbone of TEFCA's current document-based (C-CDA) exchange. Both profiles are formally required by the QTF.

**Source (authoritative):** QHIN Technical Framework (QTF) v2.1, Draft dated December 4, 2025 — https://rce.sequoiaproject.org/wp-content/uploads/2025/12/QTF-2.1-Draft-12.04.25-clean1.pdf

**Methodology note:** The QTF v2.1 PDF was reviewed via search-engine summaries quoting the document's MUST-statements rather than direct text extraction (PDF text extraction was not available in the Phase 0 environment). For Phase 3 publication, a manual read of the QTF v2.1 PDF is recommended to confirm exact section numbers and surface any additional IHE profiles (e.g., ATNA for audit logging, XUA for user assertion) that may also be required by the QTF but were not surfaced in the secondary-source review.

---

## Section 5 — Adoption Stats

### 5.1 Current numbers (verified 2026-04-23)

**Authoritative figures for Phase 1 use** (RCE homepage, fetched 2026-04-23):

- **21,086** organizations live on TEFCA (QHINs, Participants, and Subparticipants)
- **81,000+** unique connections to clinicians, hospitals, clinics, post-acute/long-term care facilities, public health authorities, and more
- **889 million** documents shared since go-live in December 2023

- **Source:** https://rce.sequoiaproject.org/ (the RCE is the network's operator-of-record; numbers are updated periodically)

**Historical progression** (useful for showing the growth curve):

| As of | Orgs | Connections | Documents | Source |
|---|---|---|---|---|
| Aug 6, 2025 | 9,000+ | — | — | RCE Netsmart designation announcement |
| Nov 17, 2025 | 10,600+ | 60,000+ | 115M | RCE blog "Winter Update" |
| Feb 2026 | — | — | ~500M | DistilINFO + DynamicHealthIT (milestone, see §5.2) |
| Apr 23, 2026 | 21,086 | 81,000+ | 889M | RCE homepage |

**Methodology note:** RCE counts "organizations" as QHINs + Participants + Subparticipants. "Connections" are downstream endpoints reached through those orgs (clinicians, hospitals, clinics, etc.). All RCE-published figures use this definition.

**Discrepancy note (excluded figure):** The DynamicHealthIT recap of the 2026 ASTP Annual Meeting (Feb 25, 2026) states "over 71,000 organizations participating nationwide." This figure is excluded from the authoritative table because the trajectory it implies — 10,600 orgs (RCE, Nov 2025) → 71,000 (Feb 2026) → 21,086 (RCE, Apr 2026) — is mathematically impossible. The likeliest explanation is that the recap mislabeled a connections-style figure as organizations. RCE is the operator-of-record and its numbers are internally consistent across dates.
- Source of excluded figure: https://dynamichealthit.com/post/2026-astp-annual-meeting/

### 5.2 Milestone
- **February 2026:** TEFCA surpassed **half a billion (500M)** health records exchanged
- **Source:** https://distilinfo.com/2026/04/06/hhs-reinstates-onc-ends-astp-dual-title/

---

## Section 6 — Regulatory Landscape (2026)

### 6.1 ASTP/ONC Deregulatory Proposed Rule (Dec 2025)
- **Proposes to remove:** Subpart D of 45 CFR part 171, which includes the **TEFCA Manner Exception (§ 171.403)**
- **Rationale given:** TEFCA's continued implementation and maturation; deregulatory posture (EO 14192)
- **Comment deadline:** February 27, 2026
- **Context:** The TEFCA Manner Exception previously allowed actors to limit EHI access requests to TEFCA-only channels without being considered information blocking, provided specific conditions were met
- **Source:** Federal Register — https://www.federalregister.gov/documents/2025/12/29/2025-23896/health-data-technology-and-interoperability-astponc-deregulatory-actions-to-unleash-prosperity
- **Implication for the app:** This is real policy turbulence to cover honestly in Phase 5 (Road Ahead). The regulatory incentive to route through TEFCA may be changing.

### 6.2 HTI-4 Final Rule (Aug 2025)
- Published as part of FY2026 CMS Hospital IPPS Final Rule
- Effective October 1, 2025
- Electronic prior auth, e-prescribing, real-time prescription benefit criteria
- **Source:** https://www.healthitanswers.net/whats-happening-at-the-astp-onc-jan-2026/

### 6.3 CMS Health Tech Ecosystem
- Trump administration initiative, announced 2025
- Voluntary information-sharing blueprint; many healthcare/tech company participants
- Early Humana + Epic data-sharing features launched 2025
- **Interaction with TEFCA:** Still being determined — tensions between voluntary CMS ecosystem and mandatory/incentivized TEFCA pathways
- **Source:** https://www.healthcaredive.com/news/oracle-health-qhin-designation-tefca/806217/

---

## Section 7 — Gaps & Limitations (honest analysis)

### 7.1 Patient matching
- No national patient identifier in the US; patient matching remains a known weak point
- **Headline stats from Pew 2018 report** (Pew compiles multiple primary sources):
  - **Within organizations:** match rates can be as low as **80%** (1 in 5 patients not matched to all their records); high-quality organizations achieve 90%+
  - **Between organizations:** match rates can be as low as **50%**, even between organizations using the same EHR vendor (citing Audacious Inquiry research)
  - **Duplicate records within organizations:** average **18%** (Black Book Market Research 2018 survey, cited in Pew report)
  - **Cost of duplicate records:** $96 per record (Children's Medical Center Dallas); **$1,950 per patient per hospital stay** in repeated services (Black Book survey)
  - **Patient harm:** **1 in 5** hospital CIOs reported patient harm from mismatches in the prior year (CHIME 2012 survey, cited in Pew report)
  - **Clinical impact:** **4%** of confirmed duplicate records result in negative clinical care (delays, missed diagnostics, duplicated tests) — 2016 report cited in Pew
- **Source:** Pew Charitable Trusts, "Enhanced Patient Matching Is Critical to Achieving Full Promise of Digital Health Records" (October 2, 2018) — https://www.pew.org/en/research-and-analysis/reports/2018/10/02/enhanced-patient-matching-critical-to-achieving-full-promise-of-digital-health-records
- **Note on sourcing:** The numbers above are compiled by Pew from their listed primary sources. For Phase 1 publication, cite Pew as the secondary aggregator unless we independently verify each primary (Black Book, CHIME, Audacious Inquiry).
- **Relevance to TEFCA:** Patient matching is the gating problem for cross-organization data exchange. TEFCA's QHIN framework relies on accurate matching across organizational and EHR boundaries — exactly the cross-org context where Pew shows match rates degrade most.

### 7.2 Consent granularity
- IAS Provider Requirements SOP v2.1 addresses individual transparency into consent choices
- **[GAP]** Need to cite how granular consent actually works in practice for non-IAS flows

### 7.3 Adoption unevenness
- 14K organizations is a fraction of the ~6,000 hospitals + ~200K+ clinician practices in the US
- Specialty coverage is uneven; behavioral health and LTPAC lag
- **[GAP]** Need specific stats on segment adoption

### 7.4 Document-to-FHIR transition burden
- Dual pipeline reality for implementers until Facilitated FHIR reaches critical mass
- UDAP registration path is still maturing (supported through 2027 per SOP v2.0 draft)

---

## Section 8 — Clinical AI References (to complete in Phase 0)

### 8.1 RAG in clinical settings

**Amugongo et al. 2025 — PLOS Digital Health systematic review (verified anchor):**
- **Type:** Systematic review (PRISMA), 70 studies selected from 2,139 retrieved articles, published June 2025
- **Clinical domains covered:** medical QA, clinical diagnosis & phenotyping, radiology, clinical trial patient matching, drug development, ENT, hepatology, arrhythmia/sleep apnea, ophthalmology
- **Headline accuracy gains from RAG (medical QA tasks):**
  - GPT-4: **73.44% → 79.97%**
  - GPT-3.5: **60.69% → 71.57%**
  - LLaMA-2-70B on PubMed-based datasets: **42.20% → 50.40%**
  - SPOKE knowledge-graph RAG with LLaMA-2: **+71% improvement** from baseline
  - AI agents with RAG: GPT-4 reaches **~95% accuracy**
- **Workflow time savings:** Clinical trial patient screening reduced from approximately **one hour per patient to seconds**
- **Critical gap finding:** only **3 of 70 studies evaluated safety concerns**; 69 evaluated accuracy. Standardized evaluation frameworks for clinical RAG do not yet exist.
- **Geographic scope:** International (78.9% English-language datasets, 21.1% Chinese; authors are Germany-based). Cite as methodology evidence rather than US deployment.
- **Citation:** Amugongo LM, Mascheroni P, Brooks S, Doering S, Seidel J. "Retrieval augmented generation for large language models in healthcare: A systematic review." *PLOS Digital Health*. 2025;4(6):e0000877. doi: 10.1371/journal.pdig.0000877 — https://journals.plos.org/digitalhealth/article?id=10.1371/journal.pdig.0000877

**Caveat for Phase 1/4 framing:** The 79.97% GPT-4 accuracy is a research-benchmark number, not a clinical-deployment outcome. Use as "RAG measurably improves LLM medical accuracy" evidence, not as "RAG is clinically validated for production care."

### 8.2 AI Agents in clinical workflows

**Doctronic — patient-facing AI consult agent (presented at 2026 ASTP Annual Meeting):**
- 22 million AI consults processed; 99.2% agreement rate with clinicians on consult outputs
- **Citation:** Pavelle M, presentation at 2026 ASTP Annual Meeting (Feb 2026), reported in DynamicHealthIT recap — https://dynamichealthit.com/post/2026-astp-annual-meeting/

**Abridge — ambient clinical documentation, scaled US deployment:**
- Deployed at Northwell Health (28 hospitals; largest non-profit health system in the Northeast), UI Health (University of Illinois Chicago academic enterprise; inpatient + outpatient + emergency), and OhioHealth (thousands of ambulatory clinicians, post-evaluation)
- Company reports use across "200+ of the largest US health systems"
- **Note on peer-reviewed evidence:** Abridge cites a JAMIA paper showing up to 67% reduction in clinician burnout. **This citation has not been independently verified in this Phase 0 pass — verify before quoting the burnout figure in published material.** Press-release-grade evidence used here only for "deployment scale" claims, not clinical-outcome claims.
- **Sources (deployment):**
  - Northwell: https://www.abridge.com/press-release/northwell-scales-abridge
  - UI Health: https://www.abridge.com/press-release/uihealth-deploys-abridge-across-care-settings
  - 200+ health systems: https://www.abridge.com/

**Caveat for Phase 4 framing:** Abridge is best framed as "scaled clinical AI deployment in US health systems," not as "agentic" in the multi-step autonomous-agent sense. Doctronic is the truer agentic example (multi-turn patient consult). For multi-agent clinical examples, the Oxford TrustedMDT system (Microsoft + Oxford Department of Oncology) is interesting but is UK-based and was excluded under the US-only rule.

### 8.3 Longitudinal context for diagnostic AI

**Wong et al. 2021 — external validation of the Epic Sepsis Model (cautionary tale):**
- **Setting:** Michigan Medicine (US academic health system); 27,697 adult patients, 38,455 hospitalizations, Dec 2018 – Oct 2019
- **Model under study:** Epic Sepsis Model (ESM), a proprietary AI model built on longitudinal EHR data (vitals, labs, demographics, history). At time of study, deployed at hundreds of US hospitals.
- **Vendor's claimed performance:** AUC 0.76–0.83
- **Independent validation result:** **AUC 0.63** (95% CI: 0.62-0.64) — substantially worse than the developer's reported performance
- **Operating-point performance:** sensitivity **33%**, specificity **83%**, PPV **12%**, NPV **95%**
- **Clinical impact:**
  - Identified only **183 of 2,552 (7%)** sepsis patients who would have benefited from earlier antibiotics
  - **Missed 1,709 (67%) of sepsis cases** despite triggering alerts
  - Generated alerts on **6,971 of 38,455 (18%)** of all hospitalizations — substantial alert-fatigue burden
- **Citation:** Wong A, Otles E, Donnelly JP, et al. "External Validation of a Widely Implemented Proprietary Sepsis Prediction Model in Hospitalized Patients." *JAMA Internal Medicine*. 2021 Aug 1;181(8):1065-1070. — https://jamanetwork.com/journals/jamainternalmedicine/fullarticle/2781307
- **Companion editorial (also useful for Phase 4):** Habib AR, Lin AL, Grant RW. "The Epic Sepsis Model Falls Short—The Importance of External Validation." *JAMA Internal Medicine*. 2021;181(8). — https://pubmed.ncbi.nlm.nih.gov/34152360/

**Why this matters for the project's thesis:** The Epic Sepsis Model is built on exactly the kind of longitudinal EHR data TEFCA can deliver. Wong et al. is a cautionary tale that having the *data* available is necessary but not sufficient — local validation, calibration, and ongoing monitoring are also required. Directly supports Phase 4's "what TEFCA does NOT solve for AI" honesty section: TEFCA solves *data delivery*; it does not solve *model validity*.

**Caveat for Phase 4 framing:** "Longitudinal" here is real-time-windowed EHR features (vitals, labs over recent hours/days), not multi-year longitudinal records. For a stronger multi-year longitudinal example (e.g., HCC risk from years of labs, oncology surveillance from prior imaging), additional citations would be needed — flag for follow-up if Phase 4 demands a long-horizon longitudinal example.

---

## Section 9 — Reference Documents (primary sources)

### TEFCA official
- TEFCA on ONC: https://healthit.gov/policy/tefca/
- RCE homepage: https://rce.sequoiaproject.org/
- Designated QHINs: https://rce.sequoiaproject.org/designated-qhins/
- Candidate QHINs: https://rce.sequoiaproject.org/candidate-qhins/
- RCE FAQs: https://rce.sequoiaproject.org/rce/faqs/
- Common Agreement page: https://rce.sequoiaproject.org/common-agreement/
- News and Announcements: https://rce.sequoiaproject.org/news-and-announcements/
- TEFCA Glossary (Jan 2026): https://rce.sequoiaproject.org/wp-content/uploads/2026/01/TEFCA-Glossary_Jan-2026-v2_508.pdf

### Technical
- Facilitated FHIR SOP v2.0 Draft: https://rce.sequoiaproject.org/wp-content/uploads/2026/02/SOP-Facilitated-FHIR-Implementation-2.0-Draft-508.pdf
- ONC TEFCA Updates Presentation Feb 2026: https://www.healthit.gov/wp-content/uploads/2026/02/2026-02-19_TEFCA_Updates_Presentation.pdf

### Regulatory
- HTI-2 Final Rule (Dec 2024): https://www.federalregister.gov/documents/2024/12/16/2024-29163/
- ASTP/ONC Deregulatory Proposed Rule (Dec 2025): https://www.federalregister.gov/documents/2025/12/29/2025-23896/

### HL7 / FHIR
- HL7 FHIR R4 specification: https://hl7.org/fhir/R4/
- US Core IG: https://hl7.org/fhir/us/core/
- SMART App Launch: https://hl7.org/fhir/smart-app-launch/
- UDAP: https://www.udap.org/

### Policy / commentary
- ONC reinstatement coverage: https://distilinfo.com/2026/04/06/hhs-reinstates-onc-ends-astp-dual-title/
- 2026 ASTP Annual Mtg recap: https://dynamichealthit.com/post/2026-astp-annual-meeting/

---

## Section 10 — Problem Statement Stats (Problem Wall source material)

These statistics quantify the clinical problems TEFCA exists to address. Sourced for Phase 1's Problem Wall.

### 10.1 Duplicate imaging in emergency departments

**Lammers et al. 2014 — landmark HIE-and-imaging study:**
- **Setting:** 447 emergency departments in California and Florida, 2007-2010 (37 EDs that joined an HIE during the study period vs 410 controls)
- **Baseline repeat-imaging rates** (within 30 days, at unaffiliated EDs): **14.7% of CTs, 20.7% of ultrasounds, 19.5% of chest x-rays** were repeats
- **HIE-associated absolute reduction:** -8.7 pp CT (95% CI: -14.7, -2.7); -9.1 pp ultrasound (95% CI: -17.2, -1.1); -13.0 pp chest x-ray (95% CI: -18.3, -7.7)
- **HIE-associated relative reduction:** **44%-67% across the three modalities** (CT 59%, ultrasound 44%, chest x-ray 67%)
- **Citation:** Lammers EJ, Adler-Milstein J, Kocher KE. "Does health information exchange reduce redundant imaging? Evidence from emergency departments." *Medical Care*. 2014 Mar;52(3):227-34. doi: 10.1097/MLR.0000000000000067 — https://pubmed.ncbi.nlm.nih.gov/24374414/

**Jung et al. 2015 — cost-side follow-up (different research group, Rochester RHIO):**
- **Setting:** 12,620 commercially-insured adults in 13-county western New York region, served by Rochester RHIO, 2009-2010
- **HIE-associated cost savings:** **$32,460 annually** in avoided repeat imaging across the cohort, or **$2.57 per patient**
- **Odds reduction:** **19% reduction in odds** of a procedure being repeated (OR 0.81)
- **Modality split:** Basic imaging (radiography, ultrasound, mammography) = 85% of avoided cases but only 50% of cost savings; Advanced imaging (CT, MRI) = 13% of avoided cases but 50% of cost savings
- **Citation:** Jung HY, Vest JR, Unruh MA, Kern LM, Kaushal R. "Use of Health Information Exchange and Repeat Imaging Costs." *Journal of the American College of Radiology*. 2015 Dec;12(12):1364-1370. doi: 10.1016/j.jacr.2015.09.010 — https://pmc.ncbi.nlm.nih.gov/articles/PMC4722040/

**Caveat for Phase 1 framing:** Both studies are 10+ years old. They establish the *mechanism* (HIE → less duplication) but the absolute numbers reflect 2007-2010 (Lammers) and 2009-2010 (Jung) practice patterns. For 2026 framing, cite as "the foundational evidence base" rather than current rates. Newer data may exist — flag for re-verification before Phase 1 publication.

### 10.2 Care fragmentation cost

**Frandsen et al. 2015 — landmark fragmentation study (US, large commercial insurer claims):**
- **Setting:** 506,376 commercially insured, chronically ill US patients (cardiovascular, diabetes, asthma, arthritis, or migraine), claims data 2004-2008
- **Method:** Each patient assigned a "fragmentation index" based on how dispersed their PCP's referral patterns were; outcomes compared between highest and lowest quartiles of fragmentation
- **Cost impact:** **$4,542 higher annual healthcare spending** for patients in the highest fragmentation quartile vs lowest ($10,396 vs $5,854; P<.001) — a ~78% relative cost increase
- **Quality impact:** **32.8% vs 25.9%** departure from clinical best practice (P<.001) — ~7 percentage points more clinical errors with high fragmentation
- **Hospitalization impact:** **9.1% vs 7.1%** preventable hospitalization rate (P<.001) — 2 percentage points more avoidable admissions
- **Citation:** Frandsen BR, Joynt KE, Rebitzer JB, Jha AK. "Care Fragmentation, Quality, and Costs Among Chronically Ill Patients." *American Journal of Managed Care*. 2015 May;21(5):355-62. PMID: 26167702 — https://pubmed.ncbi.nlm.nih.gov/26167702/

**Caveat for Phase 1 framing:** Like the Lammers/Jung imaging studies, this is 10+ years old and uses 2004-2008 claims data. The mechanism (fragmentation → costs and quality lapses) is well-established; the absolute dollar figures should be inflation-adjusted or framed as "in 2008 dollars" if quoted directly. The relative gap (~78% higher spending) is more durable than the absolute number.

### 10.3 Medication reconciliation errors

**Pippins et al. 2008 — US prospective study at Brigham and Women's + Mass General:**
- **Setting:** 180 general medical inpatients across two large academic hospitals in Boston, MA (May–June 2006)
- **Method:** Study pharmacists took gold-standard medication histories and compared them with medical teams' histories, admission orders, and discharge orders. Blinded physicians adjudicated each unexplained discrepancy
- **Discrepancies identified:** **2,066 total medication discrepancies** across 180 patients
- **Potentially harmful unintentional discrepancies (PADEs):** **257 (12% of all discrepancies)** — average **1.4 PADEs per patient**
- **Patient prevalence:** **54% of patients had at least one PADE**; 37% had ≥2; 9% had ≥5
- **Where errors happen:** **75% of PADEs occurred at discharge** (vs 25% at admission) — making discharge the highest-risk transition
- **Why errors happen:** **72% of PADEs were due to errors in taking the preadmission medication history** (not in reconciling it). Only 26% were reconciliation-step errors. Translation: most "med rec errors" are actually history-taking errors at the front door
- **Severity:** 23% of PADEs were judged "potentially serious" (could cause hospitalization or persistent functional alteration)
- **Citation:** Pippins JR, Gandhi TK, Hamann C, et al. "Classifying and Predicting Errors of Inpatient Medication Reconciliation." *Journal of General Internal Medicine*. 2008 Sep;23(9):1414-1422. doi: 10.1007/s11606-008-0687-9 — https://pmc.ncbi.nlm.nih.gov/articles/PMC2518028/

**Caveat for Phase 1 framing:** Single-period, two-hospital prospective study (n=180). The percentages (54% of patients with PADEs, 75% at discharge, 72% history-taking) are the most-cited findings and are robust within their sample, but inflation-adjusted or replicated incidence numbers in 2026 should ideally be cross-checked against a more recent national dataset (e.g., AHRQ MEPS or a 2020s replication). For the Problem Wall, "more than half of admitted patients experience a potentially harmful medication discrepancy" is the headline.

**Relevance to TEFCA:** TEFCA's Treatment exchange purpose can pull a patient's true medication list from across QHINs, attacking the root cause Pippins identified (history-taking errors). FHIR's MedicationRequest and MedicationStatement resources are exactly the data classes needed to make this work. But this only helps if the upstream EHRs have accurate, current med lists — TEFCA cannot fix garbage-in.

---

## Checklist — Phase 0 Completion
- [x] Governance / oversight / RCE
- [x] Common Agreement v2.1 / QTF v2.1 identified
- [x] All 6 Exchange Purposes
- [x] Document vs FHIR reality
- [x] USCDI v3 requirement
- [x] Major regulatory shifts (Manner Exception removal)
- [x] All 11 QHINs named with designation dates
- [x] Stats reconciliation (pick one authoritative number pre-Phase 1)
- [x] Patient matching study citation
- [x] Care fragmentation / duplicate imaging / med reconciliation stats (ONC, RAND, CMS, or peer-reviewed)
- [x] Clinical AI use case citations (2-3 strong)
- [x] IHE profile cross-check against QTF v2.1 actual text
