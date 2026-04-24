# POSTS.md — LinkedIn Content Plan

Plain-text drafts ready to paste into LinkedIn. LinkedIn does not support markdown; bullets use `→`, line breaks are intentional, and Unicode bold/italic are deliberately avoided (they break screen readers and look unprofessional).

**Timing decision (revised 2026-04-24):** Launch post below goes first, after v1.0 ships. Subsequent posts are retrospective deep-dives that pick one angle from the page and go further. Drip naturally over weeks; no fixed cadence.

---

## Launch post (Phase 3 angle — strongest hook)

**Status:** Draft ready for review and personalization. Adjust the voice if it doesn't sound like you.

**Paste-ready text below.** Copy from the line after the `<<<` marker to the line before the `>>>` marker.

<<<
Most TEFCA writeups assume FHIR.

In 2026, production reality is still C-CDA over IHE. The FHIR migration is real but in draft (Facilitated FHIR SOP v2.0, March 2026); UDAP-based registration runs only through 2027. Practitioners building today carry dual-pipeline complexity, not a clean cutover.

I got curious about where TEFCA actually stands today vs the marketing version. Ended up pulling together a knowledge hub that organizes what I found — for healthcare IT folks and clinicians who want the honest version, sourced and verified.

What's inside:

→ A Problem Wall grounded in real literature: cross-organization patient match rates can drop to 50% (Pew 2018), HIE participation cuts ED imaging duplication by 44-67% (Lammers, Medical Care 2014), 54% of admitted patients have at least one potentially harmful medication discrepancy with 75% occurring at discharge (Pippins, JGIM 2008), and high care fragmentation correlates with $4,542 higher annual spending per chronically ill patient (Frandsen, AJMC 2015).

→ The TEFCA ecosystem as an interactive layer cake — all 11 Designated QHINs in chronological order, the 6 Exchange Purposes including the new Government Benefits Determination for SSA disability flows.

→ Two query flows side-by-side: today's document-based exchange (XCPD → XCA → C-CDA) and tomorrow's Facilitated FHIR (RCE Directory → UDAP → FHIR R4 / US Core v3.1.1). With realistic latency, the consent-filtered "0 alerts" silent failure mode, and the dual-pipeline reality.

→ Clinical AI Unlock — a RAG pipeline grounded in TEFCA data, four concrete use cases (med rec, prior auth, longitudinal diagnostic context, cohort queries), and the Epic Sepsis Model cautionary tale (Wong, JAMA Internal Medicine 2021: missed 67% of sepsis cases in external validation). Data delivery isn't the same as model validity.

→ Road Ahead — honest gaps, regulatory turbulence including the proposed TEFCA Manner Exception removal (status: proposed, not yet final), the ONC reinstatement story, and CMS Health Tech Ecosystem context.

The thesis: TEFCA in 2026 is real, growing, and turbulent. Honest framing about C-CDA dominance and the FHIR transition is more useful than aspirational FHIR-only narratives.

🔗 https://pcmedsinge.github.io/TEFCA-Knowledge/

What's the most underestimated TEFCA gap you're hitting in production right now?

#TEFCA #FHIR #HealthIT #Interoperability #ClinicalAI
>>>

**Customization notes:**
- Voice: written in an opinionated practitioner register. Soften or sharpen to match how you actually post on LinkedIn.
- "I spent the last several weeks" — adjust the timeframe to match your actual build window.
- Engagement question is generic — swap for something more specific to your network if you have a stronger one.
- Hashtags: 5 is the LinkedIn-recommended sweet spot. Add `#USCore` or `#ONC` or `#HIE` if those align better with your followers.

---

## Future post drafts (drip after launch)

Numbered for tracking; write/post in any order.

| # | Angle | Working hook |
|---|---|---|
| 2 | Phase 4 deep-dive | "TEFCA + Clinical AI: the Epic Sepsis Model cautionary tale every implementer should re-read." |
| 3 | Phase 1 deep-dive | "Five clinical scenarios that explain why TEFCA exists — sourced, not anecdotal." |
| 4 | Phase 2 deep-dive | "11 QHINs, one Common Agreement, and the layer cake underneath." |
| 5 | Phase 5 deep-dive | "Honest gaps in TEFCA 2026: what doesn't yet work, and the Manner Exception debate." |

Drafts to be added as you choose to write each one.

---

## LinkedIn formatting cheat sheet

- **No markdown** — paste plain text. Asterisks, underscores, and `#` headers do not render.
- **Line breaks** render exactly as you type them. Use blank lines for paragraph spacing.
- **Bullets:** use `→` or `•` or `—` at the start of each line. Don't use `*` or `-` (those just appear literally).
- **Bold / italic:** do NOT use Unicode bold workarounds (e.g., 𝐭𝐡𝐢𝐬). They break screen readers, look unprofessional, and harm accessibility.
- **Hashtags:** 3-5 is optimal; more dilutes engagement.
- **URLs:** paste plain. LinkedIn auto-detects and shows a preview card if the page has Open Graph meta tags. (`index.html` has a `<meta name="description">` but no Open Graph tags — could add later if previews are weak.)
- **First two lines** are above the "see more" fold. Make them count.
- **Character limit:** 3,000. Most strong posts run 1,500–2,500.
- **Best posting time** (general rule, varies by audience): Tuesday–Thursday morning US business hours. For healthcare IT specifically, mid-morning ET often works.
