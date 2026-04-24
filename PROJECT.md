# Project: TEFCA + FHIR + Clinical AI — Interactive Knowledge Hub

> Single source of truth for this project. Paste this file at the start of every new Claude or Claude Code session to restore full context.

> **Currency note:** All TEFCA facts in this document are accurate as of **April 2026** and cross-referenced in `CONTENT.md`. TEFCA is evolving rapidly — re-verify before any publication pass.

---

## Status
- **Current Phase:** 4 of 5 — code complete on `phase-4-clinical-ai`, awaiting merge to `main` + `v0.4` tag for DoD. v0.4 = launch milestone per the revised plan (launch after Phase 4 ships, per LinkedIn timing).
- **Last Completed:** Phase 4 — Clinical AI Unlock section: section intro framing data-vs-model split; 6-step RAG pipeline (TEFCA query → ingest → normalize coding → vector store → retrieval → LLM grounding) with clinician-skip cue; 4 use case cards (care transitions, prior auth with honest peer-to-peer caveat, longitudinal diagnostic context with image-sharing-network honesty, cohort queries with PCORnet acknowledgement); amber-toned Wong/Epic Sepsis warning callout; 5-item "What TEFCA does NOT solve for AI" limitations list. Clinical-reader review pass applied (removed Doctronic for credibility, hedged unsourced claims, expanded consent limitation to cover HIPAA + state law + §164.514 thicket). Visually verified.
- **Next Up:** Either (a) merge `phase-4-clinical-ai` → `main`, tag `v0.4`, then begin the LinkedIn launch sequence (push to GitHub → enable Pages → draft Phase 3 post in POSTS.md → publish); or (b) defer launch until Phase 5 polish lands (v1.0). Phase 5 still pending; Phase-0-residual consent-granularity §7.2 item still open and would be a natural Phase 5 inclusion.
- **Version:** v0.1, v0.2, v0.3 shipped; v0.4 pending (= the launch milestone)

---

## Project Goal
A single HTML file, hosted on GitHub Pages, serving as a deep-dive interactive knowledge hub on TEFCA, FHIR, and Clinical AI. Targeted at Healthcare IT professionals and clinicians. Designed as a portfolio/consulting signal — not a beginner explainer. Feeds a parallel LinkedIn content series.

**Unique angle (revised after Phase 0 research):** Not just "TEFCA + FHIR + Clinical AI" — but **"TEFCA today vs TEFCA tomorrow"**. Honest about the current document-based (C-CDA) reality, the FHIR migration in progress (Facilitated FHIR SOP v2.0), and the regulatory turbulence (proposed removal of the TEFCA Manner Exception). This honesty is the differentiator.

---

## Decisions Made
- **Format:** Single HTML file (no framework, no build step)
- **Hosting:** GitHub Pages — free, version-controlled, permanent URL
- **Theme:** Dark, professional — feels like an architect built it, not marketing
- **Audience:** Healthcare IT professionals + Clinicians
- **Depth:** Deep — policy, architecture, FHIR/IHE standards, Clinical AI
- **Angle:** Broader clinical workflows (not radiology-specific)
- **Personal branding:** None — no name, no GitHub link, no personal details
- **Version tag:** "v1.0 — evolving" label retained in footer
- **Claude API:** Not embedded (avoid hosting/key exposure concerns)
- **Oversight body naming:** Use **ONC** (as of March 31, 2026 reinstatement). Acknowledge the July 2024 – March 2026 "ASTP/ONC" era where historically relevant.

---

## Author Context (for Claude sessions — do not render in app)
- 17 years Healthcare IT, primarily EHR implementations
- Hands-on FHIR, SMART on FHIR — 5-6 apps built
- AI/RAG, Agents, Transfer Learning — applied to radiology and clinical workflows
- Knows what interoperability failure looks like from the inside

---

## Repository Structure
```
/
├── index.html         ← the deliverable
├── PROJECT.md         ← this file (session handover)
├── CONTENT.md         ← verified facts, sources, citations (Phase 0 output)
├── POSTS.md           ← LinkedIn content plan (parallel track)
├── CHANGELOG.md       ← version-by-version changes
└── README.md          ← public-facing repo description
```

---

## Git Workflow
- **Branch per phase:** `phase-0-research`, `phase-1-foundation`, etc.
- **Merge to `main`** only when phase passes Definition of Done
- **Tag releases** at end of each phase: `v0.1`, `v0.2`, ..., `v1.0` at Phase 5 completion
- **Commit often** within a phase branch — granular history helps Claude in future sessions

---

## Definition of Done (applies to every phase)
A phase is only complete when ALL of the following are true:
- [ ] All checklist items for the phase are done
- [ ] All facts/claims have a source cited in `CONTENT.md`
- [ ] Works correctly on desktop (Chrome, Firefox, Safari) and mobile
- [ ] No console errors in browser dev tools
- [ ] A short entry added to `CHANGELOG.md`
- [ ] PROJECT.md status block updated
- [ ] Phase branch merged to `main` and tagged

---

## Five Phases (+ Phase 0)

### Phase 0 — Research & Content Prep ⬅ CURRENT
**Est. time:** 4-6 hours
Front-load all fact-gathering so build phases aren't blocked by verification. Output is a `CONTENT.md` with every claim sourced. **This phase is partially seeded** — see CONTENT.md for what's done and what remains.

- [x] Common Agreement current version (v2.1) with source
- [x] QTF current version (v2.1) with source
- [x] All six Exchange Purposes identified (incl. Government Benefits Determination)
- [x] Oversight body naming clarified (ONC, post-March 2026)
- [x] Document-vs-FHIR reality documented (TEFCA today is primarily C-CDA; FHIR via Facilitated FHIR SOP v2.0 rolling out)
- [x] TEFCA Manner Exception removal proposal documented
- [x] USCDI v3 requirement (Jan 1, 2026) documented
- [x] Headline adoption stats captured (with reconciliation note)
- [x] **Full list of all 11 Designated QHINs with designation dates**
- [x] **Adoption stats reconciliation** — RCE homepage vs Nov 2025 blog post discrepancy
- [x] Real statistics: care fragmentation cost, duplicate imaging rates, med reconciliation errors — with peer-reviewed / ONC / RAND sources
- [x] FHIR R4 resource types relevant to each query flow — verified against HL7 US Core v3.1.1+
- [x] IHE profiles actually referenced in TEFCA QTF v2.1 (XCA, XCPD confirmed relevant — verify exact references)
- [ ] Known gaps: patient matching (exact studies), consent granularity, adoption data
- [x] Clinical AI references — 2-3 credible, citable examples of RAG / Agent workflows in clinical settings

**Definition of Done:** `CONTENT.md` complete, every fact sourced, no "[TBD]" or "[verify]" placeholders.

---

### Phase 1 — Foundation + Problem Wall
**Est. time:** 3-4 hours
Shell + theme + navigation + the first real content section (Problem Wall). First commit to `main` should have something worth showing.
- [x] HTML skeleton, all sections stubbed
- [x] Sticky navigation with smooth scroll
- [x] CSS variables, typography, dark professional theme
- [x] Responsive foundation (mobile + desktop)
- [x] Problem Wall: 4-5 clinical scenarios, specific and recognizable
- [x] Statistics grounded in sourced data from `CONTENT.md`
- [x] v1.0 tag in footer

**Definition of Done:** Shell deployable to GitHub Pages, Problem Wall fully content-complete and visually polished.

---

### Phase 2 — TEFCA Ecosystem Map
**Est. time:** 4-5 hours
Interactive diagram. ONC → RCE (Sequoia Project) → QHINs → Participants → Subparticipants. Clickable nodes with detail panels. Common Agreement v2.1 as legal spine. All 11 Designated QHINs represented accurately.
- [x] SVG/JS interactive diagram
- [x] Clickable nodes open detail panel (role, responsibilities, real examples)
- [x] Real QHIN list (all 11, from `CONTENT.md`)
- [x] Common Agreement v2.1 explainer
- [x] All six Exchange Purposes documented (Treatment, Payment, Health Care Operations, Public Health, IAS, Government Benefits Determination)
- [x] Distinction between Designated vs Candidate QHINs shown

**Definition of Done:** Interactive diagram passes DoD, every claim traceable to `CONTENT.md`.

---

### Phase 3 — Query Flow (Document + FHIR)
**Est. time:** 5-6 hours
**Two parallel flows shown side-by-side:** today's document-based exchange (C-CDA over IHE XCA/XCPD) AND the emerging Facilitated FHIR flow (per SOP v2.0). This honesty differentiates this project from everything else on LinkedIn.
- [x] Flow A: Document-based — XCPD (patient discovery) → XCA (document query) → C-CDA payload
- [x] Flow B: Facilitated FHIR — UDAP dynamic client registration → FHIR endpoints in RCE Directory → FHIR Bundle with US Core v3.1.1+ resources
- [x] FHIR resource types labeled: Patient, DocumentReference, Consent, Bundle, MedicationRequest, AllergyIntolerance, ImagingStudy
- [x] Treatment vs IAS vs Government Benefits Determination flows differentiated
- [x] Realistic latency shown, at least one error/consent scenario
- [x] Honest annotation on "document-based is the 2026 reality; FHIR is transitioning"

**Definition of Done:** Flow is technically accurate enough that a FHIR practitioner or TEFCA implementer finds no errors.

---

### Phase 4 — Clinical AI Unlock
**Est. time:** 5-7 hours
TEFCA as data ingestion layer for Clinical AI. Specific, concrete deliverables — not hype. Acknowledge that C-CDA-dominant data requires normalization before it's AI-ready.
- [x] RAG pipeline diagram: TEFCA → C-CDA/FHIR ingestion → Normalization (USCDI v3) → Vector store → Retrieval → LLM
- [ ] Agent workflow example: clinical task requiring multi-source queries via TEFCA *(deferred — Doctronic was the only US example and was removed during clinical-reader review for credibility reasons; revisit if a stronger US-specific peer-reviewed example surfaces)*
- [x] 3-4 concrete use cases across clinical workflows:
  - [x] Care transitions / med reconciliation
  - [x] Prior authorization automation
  - [x] Clinical context for diagnostic AI (incl. longitudinal imaging priors)
  - [x] Longitudinal cohort queries (research/QI)
- [x] Honest section: what TEFCA does NOT solve for AI
  - Data quality (C-CDA variability, incomplete USCDI conformance)
  - Semantic normalization
  - Consent-at-scale for AI training/inference
  - Patient matching still imperfect
  - Document vs FHIR transition creates dual-pipeline burden

**Definition of Done:** Each use case has a clear data-flow diagram and plain-English explanation; honest limitations section present.

---

### Phase 5 — Road Ahead + Polish
**Est. time:** 3-4 hours
Gap analysis + policy turbulence + full polish pass. Tag v1.0 on completion.
- [ ] Gaps: patient matching, consent granularity, adoption unevenness, C-CDA→FHIR transition
- [ ] Regulatory turbulence: TEFCA Manner Exception removal proposal (HTI deregulatory rule), ONC re-established from ASTP/ONC
- [ ] TEFCA direction: Facilitated FHIR SOP v2.0 rollout, Government Benefits Determination use cases
- [ ] CMS Health Tech Ecosystem and its interaction with TEFCA (context, not endorsement)
- [ ] Animation polish pass across all sections
- [ ] Responsiveness audit (mobile, tablet, desktop)
- [ ] Accessibility quick-pass (keyboard nav, contrast, ARIA labels)
- [ ] Final "v1.0 — evolving" tag in footer

**Definition of Done:** Site ships as v1.0 tagged release. Ready for LinkedIn announcement.

---

## Parallel Track — LinkedIn Content Plan
Tracked in `POSTS.md`. Each post tied to a phase.

**Posting timing (decided 2026-04-23):** Do NOT post any of these until Phase 3 ships. Rationale: Phase 1 (Problem Wall) alone is table-stakes for healthcare interop content; Phase 3's "TEFCA today is C-CDA, here's where FHIR fits" is the unique differentiator that makes the project worth sharing. Launch post = the Phase 3 idea below. Phase 1 and 2 posts become retrospective deep-dives after the launch. Phase 4 and 5 posts drip as those phases ship.

| Phase Shipped | Post Idea |
|---|---|
| 1 | "Why I built a TEFCA knowledge hub — and what the Problem Wall says about US healthcare" |
| 2 | "11 QHINs, one Common Agreement — the TEFCA ecosystem in April 2026" |
| 3 | "The uncomfortable truth about TEFCA: it's still mostly C-CDA. Here's where FHIR actually fits." |
| 4 | "TEFCA + Clinical AI — what's genuinely unlocked, and what's still blocking" |
| 5 | "v1.0 shipped — honest gaps, the Manner Exception debate, and what's next" |

Full drafts and scheduling live in `POSTS.md`.

---

## Rollback Strategy
- If a phase goes wrong, revert the phase branch — `main` is never broken
- Keep the previous phase's tagged release (`v0.3`, etc.) as a known-good fallback
- Notes on failed approaches go into `CHANGELOG.md` under "Dropped" so future sessions don't repeat them

---

## Known Issues / Deferred
*(Things intentionally skipped for later — documented here so they aren't forgotten.)*
- *(none open — Phase 0 deferred items resolved as of 2026-04-23)*

---

## Handover Instructions
At the start of every new Claude or Claude Code session:
1. Paste the contents of this file
2. Claude confirms current phase and next steps
3. Work proceeds on the current phase branch
4. Before ending the session: update Status block, tick completed checklist items, commit PROJECT.md along with any code changes

---

## Guiding Principles
- Every section should have something a 17-year Healthcare IT veteran finds non-obvious
- No vendor language — write from a practitioner's perspective
- No unsourced claims — if it's in the app, it's in `CONTENT.md`
- Technical accuracy over marketing polish — audience will fact-check
- Honest limitations earn more credibility than aspirational claims
- **Re-verify TEFCA facts before every major publication** — the policy and regulatory landscape is moving quickly in 2026
