# LQ.AI Committee — Weekly call — 2026-07-19

| | |
|---|---|
| **Date** | 2026-07-19, 07:30 (GMT-7) |
| **Platform** | Google Meet (platform issues at start; standing call moved to Zoom thereafter) |
| **Facilitator** | Not recorded in source notes |
| **Minutes** | Joel Kaufmann |
| **Attendees** | Ang Houfu, Peter Scripps (pscripps), Joel Kaufmann |
| **Attendee-list approval** | Confirmed by the LQ.AI team before publication; approval reported by Joel Kaufmann on 2026-08-02 |
| **Regrets** | — |

> **Retrospective record.** This meeting predates the creation of this repository. The
> record was migrated from committee notes on 2026-07-26, when the repository was
> bootstrapped under ADR 0022 (lq-ai PR #311).

## Purpose

- Establish a sustainable governance model and decision-making process for the LQ.AI
  open-source project, which has grown beyond its original founder-driven structure.
- Determine how litigation-specific features should be incorporated into a product
  initially designed as an in-house legal tool.

## Decisions

1. **ADR-first working approach (direction).** Before issues or PRs are accepted, the
   underlying architectural question is settled in a drafted ADR, so contributions are
   reviewed against already-agreed direction. Proposed by Ang; endorsed by Peter and Joel.
   *Subsequently formalized in ADR 0022 via lq-ai PR
   [#311](https://github.com/LegalQuants/lq-ai/pull/311).*
2. **Standing call moves to Zoom** (weekly, same format and participants), resolving
   recurring Google Meet authentication issues. Owner: Joel. *These minutes are the
   canonical operational record for this decision.*
3. **Three ADRs to be drafted** by Ang for community comment before related issues/PRs are
   accepted: (i) jurisdictions, (ii) litigation / areas of law, (iii) technical
   maintenance. Joel and Peter to comment once submitted. The resulting proposals were
   lq-ai PRs [#311](https://github.com/LegalQuants/lq-ai/pull/311),
   [#312](https://github.com/LegalQuants/lq-ai/pull/312), and
   [#313](https://github.com/LegalQuants/lq-ai/pull/313).

## Discussion summary

- **Governance gap.** Ang noted that for many pending decisions there are equally valid
  arguments on both sides, and the existing ADRs, PRDs, and roadmap do not resolve the
  gray areas. Peter identified the structural tension of open source — contributors lack
  employment-style incentives, and triaging 10–12 contributors' staggered submissions is
  difficult for one or two reviewers. The group agreed the bottleneck is governance and
  decision-making structure, not technical capability.
- **Models for structure.** Joel outlined lessons from Debian's governance (project
  leaders, a technical committee, a project secretary, contributor-to-maintainer
  progression, domain-specific ownership). Ang valued the committee concept but noted the
  project is currently too small for a full Debian-style structure.
- **Contributor depth.** Ang emphasized building a core group deeply familiar with the
  source code beyond himself, Eric Sales, and Kevin, for redundancy of knowledge.
- **Litigation feature.** Joel explained his litigation-workflows PR: LQ.AI's document
  ingestion layer and overall architecture are strong foundations for litigation, though
  the product is positioned as an in-house tool. Peter noted his firm handles litigation
  in-house — useful, but scope discipline is needed. Ang was uncomfortable positioning
  the product in a way that alienates other practice areas, while agreeing new practice
  areas must be introduced carefully for maintenance and feature-completeness reasons.
  The roadmap currently contains no implementation detail for litigation; Joel and Peter
  will collaborate on a roadmap proposal after the ADRs land.
- **Broader applicability.** Joel argued litigation support will attract contributors
  (his own initial dismissal of the repo as in-house-only being the example), and
  stressed continued documentation improvements for new-contributor accessibility.
- **Maintainer agent.** Joel endorsed the maintainer-agent concept raised in Slack and
  suggested temporal currency flags on legal outputs (e.g., "this was the law as of
  July 19, 2026").

## Action items

- [x] **Ang** — Draft the three ADRs and submit as PRs for community review.
      *(Status at posting: done — lq-ai PRs #311, #312, #313.)*
- [ ] **Joel & Peter** — Draft a roadmap proposal for the litigation feature within the
      existing architecture. *(Status at posting: in progress — mini-PRD draft exists;
      scope narrowed at the 2026-07-26 call.)*
- [ ] **Joel & Peter** — Comment on the ADRs once submitted. *(Status at posting: in
      progress — pscripps to post comments on the expansion/litigation ADR per the
      2026-07-26 call.)*
- [x] **Joel** — Switch the recurring meeting to Zoom. *(Done.)*
- [x] **Joel** — Share meeting notes with the group via Slack. *(Done.)*

## Ratification

- **Posted (initial repository publication):** 2026-08-02
- **Objection window closes:** 2026-08-09
- **Attendee-list publication review:** Confirmed by the LQ.AI team
- **Status:** Open for objections through 2026-08-09
