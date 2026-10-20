# LQAI Committee — Weekly Call (2026-10-04)

**PUBLIC VERSION — approved for publication.**

*Discussion and action items are summarized without identifying individual speakers or owners. Named ownership is maintained in the private record.*

| Field | Record |
|---|---|
| Date / platform | October 4, 2026 / Zoom |
| Attendees | Houfu Ang, Joel Kaufmann, Alexios Kirillov, Emily Cabrera, Matteo Johannes Bürgler |
| Facilitator | Not recorded in source notes |
| Minutes-taker | Not recorded in source notes |
| Regrets | Not recorded in source notes |
| Attendee-list and content publication approval | Joel Kaufmann confirmed on 2026-10-19 that the attendee list and public notes are approved for publication. |

## Key Outcomes

The previous meeting was held September 20; the September 27 meeting was cancelled because of the LQ Residency demo. LQAI 0.8.0 has been released, and thanks were extended to all contributors.

Several new ADRs are in the review queue, covering tabular bulk operations, identity, a community skill catalog, and — from an external contributor — a structured UI component system to replace Tailwind-based styling. These are expected to be reviewed and likely approved at the next meeting. The Road to 1.0 ADR will receive a final review before merging.

The call also covered contributor onboarding, a draft sponsorship framework, maintainer sustainability, a planned epic for the new agent harness, and a shared agent configuration to help contributors align PRs with review expectations.

## Decisions and Agreed Follow-Ups

No formal votes or ADR acceptances were recorded at this meeting. Agreed directions:

- Review the pending ADRs ahead of the next meeting, where approval is expected to be considered.
- Give the Road to 1.0 ADR a final review before merging into main.
- Add contributor stories to the community repository to lower the barrier for newcomers.
- Continue posting starter issues to the LQ community roughly every two weeks.
- Keep UI improvement as a medium-term priority and consolidate UI feedback before further discussion.
- Align the draft sponsorship framework with the LegalQuants organization before any external use; no sponsors, tiers, or prices were approved.

These minutes are the canonical operational record for the items above; no ADR or PR numbers were recorded in the source.

## Community Repository and Contributor Onboarding

A pull request for the LQAI community repository was discussed. The repository is intended as a first stop for new contributors and for anyone who has missed meetings. Regular issue posting to the LQ community chat has already produced first contributions, resolved within about a week using coding agents.

It was noted that the project can feel overwhelming at first, and that pointing a coding agent at the codebase has worked well. The group agreed the onboarding message should be simplified along those lines. A “contributor stories” feature was proposed in which early contributors describe how they made their first contribution. Interest from prospective contributors outside the community was also reported; they are being directed to CONTRIBUTE.md.

## SF Tech Week

The San Francisco Tech Week event was discussed. An LQAI demo was not on the agenda; the question is to be followed up offline.

## UI Inspiration

An open-source legal desktop tool (“Legal Work,” from Eigenwelt) was shared as UI inspiration, noted for its familiar, lawyer-friendly interface and Word and Outlook integrations. It was noted that the current LQAI UI was built to demonstrate features rather than for daily use, and that UI improvement is already on the medium-term roadmap. Feedback from several community members will be consolidated for a structured discussion.

## Sponsorship Framework

A draft sponsorship framework was presented. There are no formal sponsors yet, but the project has real costs (such as the Apple Developer account used for macOS app signing) and may have more (such as telemetry infrastructure). Two models were outlined: a tiered monthly retainer with visibility benefits, and one-off sponsorships tied to specific roadmap items, including a “moonshot” category for high-complexity features. Funds would flow through the LegalQuants organization, with the community deciding allocation.

Support was expressed for using sponsorship to compensate maintainers, both for continuity and for succession planning, and for designating a successor or shadow maintainer. The upcoming SF Tech Week event was identified as a possible opportunity to raise sponsorship. Partnerships with law schools — where students contribute for academic credit — were proposed as a contributor pipeline that could also appeal to sponsors. No commitments were made.

## Agent Harness, Release Process, and PR Review

The new agent loop previewed in 0.8.0 was described as a good start, but integrating the open-source plugins and skills into LQAI requires substantially more work. An epic issue will lay out contributor tasks with a clear ladder showing which skills each contribution activates.

The release process (merging PRs, closing gates, running the release runbook, and writing release notes) was identified as a low-barrier pathway for contributors interested in becoming maintainers.

A substantial backlog of contributor PRs remains, with roughly half expected to merge this month. It was noted that AI review agents can make aggressive suggestions that require human judgment. A shared contributor configuration was proposed; a shared review agent already in development will be published in the community repository so contributors can pre-check PRs against the same criteria used in review.

## Action Items

*IDs match the private record. Individual owners are not published. These are follow-ups, not verified completion.*

- [ ] **O04-01:** Final review and merge of the Road to 1.0 ADR.
- [ ] **O04-02:** Review the pending ADRs (tabular bulk operations, identity, community skill catalog, UI component system) ahead of the next meeting.
- [ ] **O04-03:** Invite early contributors to write short contributor stories for the community repository.
- [ ] **O04-04:** Review the shared UI reference and consolidate UI feedback for a future discussion.
- [ ] **O04-05:** Align the sponsorship framework with the LegalQuants organization before the SF Tech Week event.
- [ ] **O04-06:** Draft an epic/tracker issue for the new agent harness and skill integration.
- [ ] **O04-07:** Publish the shared agent/plugin configuration in the community repository.
- [ ] **O04-08:** Continue posting starter issues to the LQ community roughly every two weeks.
- [ ] **O04-09:** Welcome and onboard prospective contributors.
- [ ] **O04-10:** Merge roughly half of the outstanding contributor PRs this month.
- [ ] **O04-11:** Coordinate how sponsorship will be raised at the SF Tech Week event.
- [ ] **O04-12:** Share event information to support targeted sponsor outreach.
- [ ] **O04-13:** Discuss the sponsorship approach with the LegalQuants organization as appropriate.
- [ ] **O04-14:** Review the sponsorship framework and provide pitch feedback.
- [ ] **O04-15:** Continue submitting PRs.
- [ ] **O04-16:** Make a first contribution and route an interested external contact to the maintainers.
- [ ] **O04-17:** Explore law school partnerships as a contributor pipeline.

## Review, approval, and publication

*This record was prepared and circulated before the coordinated process change took effect, so it follows the prior public-posting rule (merge = posting; seven-day public objection window from posting). See the [transition clarification](../README.md#transition-clarification-2026-10-13).*

- **Draft prepared:** October 8, 2026.
- **Internal circulation:** Not recorded in source notes (circulated to attendees for review after October 8, 2026; exact date and time not recorded).
- **Objection deadline (internal):** Not recorded in source notes.
- **Approval date:** 2026-10-19
- **Approval basis and confirmation:** No objections or corrections were raised by attendees following internal circulation; publication of the attendee list and public notes confirmed by Joel Kaufmann on 2026-10-19.
- **Attendee-list publication review:** Confirmed by Joel Kaufmann on 2026-10-19.
- **GitHub publication (merged):** 2026-10-19
- **Objection-window close (prior rule):** 2026-10-26 (merged 2026-10-19 + 7 days).
- **Status:** Published 2026-10-19 — open for public objections through 2026-10-26.

These notes summarize an AI-generated meeting summary; no verbatim transcript was used. Corrections after posting are added as dated entries.
