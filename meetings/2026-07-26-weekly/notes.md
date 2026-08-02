# LQ.AI Committee — Weekly call — 2026-07-26

| | |
|---|---|
| **Date** | 2026-07-26; time and time zone not recorded in source notes |
| **Platform** | Zoom (standing platform) |
| **Facilitator** | Not recorded in source notes |
| **Minutes** | Joel Kaufmann |
| **Attendees** | Alexios, Ang Houfu, Peter Scripps (pscripps), Joel Kaufmann |
| **Attendee-list approval** | Confirmed by the LQ.AI team before publication; approval reported by Joel Kaufmann on 2026-08-02 |
| **Regrets** | — |

## Purpose

- Review repository statistics and backlog status.
- Discuss Alexios's AI-generated bulk PR submission (47 of 112 roadmap items).
- Establish a code review and PR merging workflow.
- Review and adopt three pending Architecture Decision Records.
- Define release milestones and prioritization strategy.

## Decisions

1. **All three ADRs to be merged** once pscripps posts formal comments on the
   expansion/litigation ADR PR:
   - ADR 0022 — committee governance and meeting records (GOVERNANCE.md; minutes in a
     separate `lq-ai-community` repository) — lq-ai PR
     [#311](https://github.com/LegalQuants/lq-ai/pull/311);
   - ADR 0023 — uv-managed lockfiles for `gateway/` and `api/` — lq-ai PR
     [#312](https://github.com/LegalQuants/lq-ai/pull/312);
   - ADR 0024 — expansion direction paper and contribution routing — lq-ai PR
     [#313](https://github.com/LegalQuants/lq-ai/pull/313).
   *Publication status checked 2026-08-02: PRs #311 and #312 merged on 2026-07-27;
   PR #313 remains open.*
2. **Litigation scope narrowed.** The litigation expansion moves forward limited to
   **research and drafting only**, as these skills are the most transferable across legal
   domains. Canonical proposal: ADR 0024 in lq-ai PR
   [#313](https://github.com/LegalQuants/lq-ai/pull/313).
3. **Release milestones.** Target releases v0.6.3 and v0.7; GitHub milestones will be
   used to assign PRs and issues to releases. Owner: Houfu. *These minutes are the
   canonical operational record for this decision.*
4. **Transparency and founder loop-in.** The committee will continue committing decisions
   to the repository transparently and will bring Kevin Keller up to date before any
   public release, once the 112 roadmap items are addressed. *These minutes are the
   canonical operational record for this decision.*
5. **Zoom confirmed** as the standing meeting platform. *These minutes are the canonical
   operational record for this decision.*

## Discussion summary

- **Repository backlog.** 54 open pull requests and 37 new issues reported at the call;
  low closure rate over the past week; no releases published for an extended period.
  Risk: a growing backlog may slow momentum.
- **Bulk PR submission.** Alexios used an agentic loop running headless (~8 hours) to
  generate 47 PRs against Kevin Keller's 112-point roadmap, categorized into tool use,
  security, new features, and compliance. A separate AI session reviewed all 47 PRs;
  8 errors were identified and corrected. Risk: the code has not yet been reviewed by a
  human programmer, and the anonymization feature was found to be non-functional. Next:
  Houfu to act as reviewer/pair programmer using his maintainer agent; Alexios to provide
  a prioritized list of PRs.
- **AI-assisted review workflow.** Current approach is AI-generated code reviewed by a
  second AI session against defined criteria. pscripps noted enterprise teams have
  largely shifted to AI-first review with layered staging environments. Proposed
  workflow: adversarial AI review (Houfu's maintainer agent reviewing Alexios's
  submissions), followed by recalibration and further PR batches.
- **Anonymization feature (open).** Alexios raised a substantive concern that the
  pseudonymization/anonymization feature is unreliable and potentially misleading —
  complete anonymization cannot be guaranteed and cases can be identified by context. He
  suggested removing the feature entirely rather than representing it as functional.
  **This remains an open discussion point.**

## Action items

- [ ] **Alexios** — Send Houfu a prioritized list of PRs (feature value, bug fixes,
      security) to guide review sequencing.
- [ ] **Alexios** — Continue testing LQ.AI locally and with Anthropic, fixing issues as
      PRs are merged.
- [ ] **Alexios** — Proceed toward completing the remaining roadmap items (up to 112 PRs
      total) after initial review feedback from Houfu.
- [ ] **Houfu** — Act as reviewer and pair programmer for Alexios's PRs using the LQAI
      maintainer agent.
- [ ] **Houfu** — Stress-test the maintainer agent against Alexios's submitted PRs.
- [ ] **Houfu** — Set GitHub milestones for v0.6.3 and v0.7 and assign PRs/issues.
- [ ] **Houfu** — Merge the three ADRs after pscripps posts comments on the
      expansion/litigation ADR. *(Status checked 2026-08-02: #311 and #312 merged;
      #313 remains open.)*
- [ ] **Houfu** — Release updated maintainer agent (v0.3) for Alexios to try.
- [ ] **Peter** — Post formal comments on the expansion/litigation ADR PR supporting
      the narrowed scope (research and drafting only) — by end of day, meeting date.
- [x] **Joel** — Set up the LQAI community repository with the meeting folder convention.
      *(Completed by this repository's initial publication.)*
- [x] **Joel** — Upload meeting minutes from this week and last week to the community
      repo. *(Completed by this repository's initial publication.)*
- [ ] **Joel** — Draft a mini-PRD for the litigation module based on the adopted ADR
      scope.
- [ ] **Joel** — Shift focus from architectural proposals to validating and progressing
      existing open issues.

## Ratification

- **Posted (initial repository publication):** 2026-08-02
- **Objection window closes:** 2026-08-09
- **Attendee-list publication review:** Confirmed by the LQ.AI team
- **Status:** Open for objections through 2026-08-09
