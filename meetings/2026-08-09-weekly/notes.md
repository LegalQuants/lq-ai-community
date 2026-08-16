# LQ.AI Committee — Weekly call — 2026-08-09

*Public meeting notes with anonymized speaker attribution, per the committee's notes process.*

| | |
|---|---|
| **Date** | 2026-08-09; time and time zone not recorded in source notes |
| **Platform** | Zoom (standing platform) |
| **Facilitator** | Not recorded in source notes |
| **Minutes** | Joel Kaufmann |
| **Attendees** | Ang Houfu, Joel Kaufmann, Emily, Julian, Peter Scripps |
| **Attendee-list approval** | Confirmed by Joel Kaufmann (minutes-taker) |
| **Regrets** | Not recorded in source notes |

## Decisions

<!-- Canonical text of each architectural/product decision lives in lq-ai (ADR/PR/issue).
     A matching row for each decision is added to ../../decisions/README.md in the same commit. -->

1. **Meeting notes process.** Draft posted shortly after each meeting, ratified at the following week's call, then published to the public repo with anonymized speaker attribution. *These minutes are the canonical operational record for this decision.*
2. **Version numbering policy.** Minor version bump (e.g., 0.6 → 0.7) signals breaking changes requiring users to review docs; patch releases use a third number. Canonical: ADR 0025 — [lq-ai PR #487](https://github.com/LegalQuants/lq-ai/pull/487).
3. **ADR 0025 approved and merged** (versioning policy + version-consistency gate + pipeline ordering) — [lq-ai PR #487](https://github.com/LegalQuants/lq-ai/pull/487) — clears the v0.7.0 release blocker.
4. **ADR 0024 approved and merged** — [lq-ai PR #313](https://github.com/LegalQuants/lq-ai/pull/313) — routing for jurisdiction and practice-area expansion contributions; unblocks the ~dozen stalled expansion proposals across lq-ai/lq-skills.
5. **0.7.0 release path.** With ADR 0025 ratified, sequence proceeds: rebase #499 → label breaking changes → tag v0.7.0 → cut desktop-v0.7.0; three issues remain outstanding on the 0.7 milestone. *These minutes are the canonical operational record for this decision.*
6. **Governance transparency.** Open discussion on Slack and calls; formal decisions recorded on the public repository. *These minutes are the canonical operational record for this decision.*

## Discussion summary

### Key Outcomes

The committee held its first meeting under the new ADR governance structure, covering governance bootstrapping, the road to the **0.7.0 hardening release**, ADR ratifications needed to unblock it, documentation gaps, contributor onboarding, and longer-term questions around project direction and IP protection. Two new committee members were oriented to the project and identified areas where they can contribute. **ADR 0024 and ADR 0025 were approved and merged**, clearing the v0.7.0 release blocker; several additional action items and strategic topics were surfaced for follow-up.

### Agenda

1. Welcome & governance kickoff
2. Road to v0.7.0
3. Decisions needed (ADR ratifications and related items)
4. Contributor onboarding & community
5. Open floor & action items

### Governance Kickoff

- **Attendance** was taken for the record — the first attendee list to be published under the new process.
- **GOVERNANCE.md + ADR 0022** (merged 27 Jul, #311): adoption confirmed in substance, but the status flip ("Proposed" → "Adopted") remains **outstanding** in the document itself.
- **Record-keeping bootstrap:** a minute-taker was designated for this call; creation of the community repo and the timing of notes posting (which starts the 7-day ratification clock) were addressed.

### Road to v0.7.0

Signposted by the draft release notes in #499 — a **hardening release**, the first substantial remediation of the 22-finding security audit (#288).

- **Already on `main`:** all three *High* findings closed (GW-01 gateway key, API-01 chat-creation IDOR, D-01 skill-markdown XSS) plus three Mediums (GW-04, AG-01, API-04); uv lockfiles (ADR 0023), SHA-pinned actions, stack-boot smoke test, KB junction backfill, and the governance framework.
- **Why a minor, not a patch:** #396 and #399 change operator-visible behavior.
- **Former blocker resolved:** the tag was waiting on **ADR 0025** (versioning policy + version-consistency gate + pipeline ordering, #487), which was **approved and merged**. Remaining sequence: rebase #499 → label breaking changes → tag v0.7.0 → cut desktop-v0.7.0.
- **Also approved and merged:** **ADR 0024** (#313) — routing for jurisdiction and practice-area expansion contributions: four routing shapes plus the coverage-map claim ledger.

### Decisions Still Pending

- **ADR 0022 status flip** — document status still reads "Proposed"; flip to "Adopted" outstanding.
- **ADR 0023 balance** — gateway/api lockfiles shipped; decide whether/when the `web` image moves off `requirements.txt` onto the fork's upstream `uv.lock`.
- **Docs website** — proposal to stand up a documentation site: tooling, scope (operator docs / contributor guides / skill authoring), where it lives, and who owns it.
- **Remaining #288 findings** — 7 Medium / 8 Low / 1 Info still open post-v0.7.0; confirm ownership and a finding-ID commit convention.

### Contributor Onboarding & Community

- **Good-first-issues backlog + template** — status reviewed and seeding of the tracker discussed.
- **Top community pickups:** DE-287 (Word add-in surface), DE-288 (Slack/Teams `/lq`), plus small starters (DE-322, DE-333).
- **Skills pipeline** — call for practicing attorneys to attest/review skills.
- **Proposal routing:** proposals flow through DE-XXX / a tracking issue / an ADR as appropriate.

### Open Questions

- What is the **end goal / 1.0 definition** for LQAI — product vs. chassis vs. educational platform?
- Should **"good first issues"** be restricted to LQs/lawyers to prevent resume-padding contributors ("sharks")?
- What level of **IP protection or commercialization** is appropriate, and what does LQ want to protect long-term?
- How to **build a resilient core contributor group** so the project continues if the primary maintainer steps back?

### Pending Confirmation

- **Documentation site PRD** — the lead maintainer to draft within 1–2 weeks for community review.
- **Cross-disciplinary accelerator program** (law/CS/business) organized by a committee member — fireside chat in September, hackathon in October, cohort launch in January; potential LQAI partnership to be explored.
- Landing page ownership: confirmed within this group's purview; needs clearer messaging on target user, value proposition, and getting-started guidance.

### Identified Risks

- **Single maintainer dependency:** The lead maintainer currently holds sole merge rights; no backup maintainer in place.
- **Contributor vetting gap:** Open repo with no formal vetting may attract low-intent contributors; could affect project reputation and IP.
- **Usage data absent:** ~500 cloners in last 14 days but no visibility into actual use cases or most-valued features.

## Action items

- [ ] **Lead maintainer** — Draft PRD for documentation site within 1–2 weeks; post for community comment.
- [ ] **Committee member (practitioner)** — Deploy LQAI at their law firm beyond experiment to surface real-world bugs and documentation gaps.
- [ ] **Committee member (practitioner)** — Consult a systems engineer for documentation tooling recommendations.
- [ ] **New member (IP/litigation background)** — Use an AI agent to analyze the repo against their skill set and identify contribution areas; share thoughts in Slack before acting.
- [ ] **New member (IP/litigation background)** — Analyze LQAI components from an IP/licensing perspective; provide recommendations on what to protect vs. share openly.
- [ ] **New member** — Review LQAI landing page; propose revisions for clarity on target user, value, and onboarding.
- [ ] **All new contributors** — Read the **PRD** and HONEST STATE documents in the repo to get oriented.
- [ ] **Next call** — Confirmed for next Sunday.

## Ratification

- **Posted (committed to main):** 2026-08-16
- **Objection window closes:** 2026-08-23 (posted + 7 days)
- **Attendee-list publication review:** Confirmed by Joel Kaufmann (minutes-taker)
- **Status:** Open for objections through 2026-08-23

<!-- Per GOVERNANCE.md (lq-ai PR #311): committee members who miss a call may register
     agreement or objection within 7 days of posting; silence after 7 days is assent.
     On window close, set Status to "Ratified (silence is assent)" or record the
     objection outcome. Posted minutes are append-only — corrections are added as
     dated "Correction (YYYY-MM-DD):" entries. -->
