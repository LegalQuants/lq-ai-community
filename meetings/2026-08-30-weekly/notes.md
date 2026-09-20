# LQAI Committee — Weekly Call (2026-08-30)

*Discussion and action items are summarized without identifying individual speakers or owners. Named ownership is maintained in the internal record.*

| Field | Record |
|---|---|
| Date / platform | August 30, 2026 / Zoom |
| Time zone | GMT−7, as identified in the source record |
| Attendees | Houfu Ang, Joel Kaufmann, Julian Bryant |
| Facilitator | Not recorded in source notes |
| Minutes-taker | Not recorded in source notes |
| Attendee-list and content publication approval | Joel Kaufmann confirmed on 2026-09-20 that all attendees and the information in these public notes are confirmed and approved for publication. |

## Key Outcomes

The committee reviewed seven responses to the 1.0 community survey. The discussion favored **operator trust**: making the existing product dependable and ensuring that code, documentation, and public claims agree before committing to a major new capability.

The timetable moved away from the earlier proposed first-quarter target toward **no committed 1.0 date until capacity is clearer**. The survey would remain open another week. Participation, reviewer capacity, and practical ways for members to contribute were central themes, alongside release work and improvements to the security-reporting process.

## Decisions and Working Directions

The transcript supports the following working directions and operational follow-ups. It does not record a formal vote adopting a complete roadmap.

- **Operator trust first:** focus on the stability and completeness of existing capabilities.
- **API-only use acknowledged but unsupported:** retain focus on the ordinary UI and avoid an additional support/documentation commitment for a separate headless offering.
- **No committed release date until capacity is clearer:** review and merging capacity remain important constraints; additional maintainer help is welcome.
- **Survey remains open for another week:** seek additional responses and use the results to guide priorities and contribution opportunities.
- **Individual outreach:** coordinate personal reminders to people who have not completed the survey.

No express approval of the previous week's minutes was identified in the source transcript.

## Release Progress

Recent dependency updates across the web UI, API, and gateway were reported. The stated intention was to finish outstanding changes and release v0.7.1 on August 31. Scope for the following release remained under discussion. This is the plan reported at the meeting, not confirmation of the eventual release outcome.

## Roadmap and Feature Priorities

- Baseline work discussed included stability, security findings, the procurement pack, matter-intake work, and reconciliation of documentation with actual behavior.
- The discussion favored deferring contract-repository work from the near-term 1.0 scope. This should not be read as a decision to remove a shipped feature.
- Scanned-document support and OCR received strong interest. Reliable ingestion was treated as foundational: incomplete source input limits what later processing can achieve.
- Meta-memory remained a candidate for further consideration, with additional underlying data-structure work to understand.
- A broader Word add-in would need research and a contributor willing to lead the work. No unconditional commitment to deliver that feature was recorded.
- Survey feedback also questioned whether feature selection should precede a clearer account of target users and their needs. That product-definition question remained part of the discussion.

## Contribution and Maintainer Capacity

Attorney review was the most commonly offered form of help in the survey, but meaningful acceptance testing can require both legal and engineering work. The discussion cautioned against assuming that lawyer attestation is a simple final check detached from the way the software is tested.

The committee explored how to turn interest into practical contributions. Suggestions included smaller tasks, clearer requests, matching work to individual interests, and making the learning benefits of participation more visible. An introductory session covering GitHub basics and beginner tasks was proposed, without a fixed owner or date.

More targeted outreach was supported. Individual survey reminders would be coordinated, and members who offered help could be approached about specific opportunities. The survey results were useful input from a small respondent group, not a binding vote or a complete measure of community opinion.

## Security-Reporting Process

The committee discussed shortcomings in the documented security-reporting routes and the need to respond to a report and coordinate remediation. Repairing those routes and addressing the report were identified as follow-up work. This record does not establish that fixes were merged, released, or verified; detailed findings remain outside these public notes.

## Action Items

*Internal action IDs are retained so the two versions can be reconciled. Individual owners are not published.*

- [ ] **A30-01:** Complete outstanding release work and check the outcome against the planned August 31 v0.7.1 release.
- [ ] **A30-02:** Keep the survey open for another week and incorporate additional responses into planning.
- [ ] **A30-03:** Match offers of help to concrete contribution opportunities.
- [ ] **A30-04:** Coordinate individual reminders to survey nonrespondents.
- [ ] **A30-05:** Complete the outstanding survey response volunteered during the call.
- [ ] **A30-06:** Repair the security-reporting process, respond to the report, and coordinate remediation through the appropriate channels.

The proposed beginner session and welcoming contribution message remain suggestions/offers to confirm rather than scheduled deliverables.

## Takeaway

The emerging route to 1.0 is a trustworthy, well-documented product supported by realistic delivery capacity. The immediate work is to turn survey feedback into manageable priorities and individual contributions while completing release and reporting-process improvements.

## Ratification

- **Posted (merged):** 2026-09-20
- **Objection window closes:** 2026-09-27 (posted + 7 days)
- **Attendee-list and content publication review:** Joel Kaufmann confirmed on 2026-09-20 that all attendees and the information in these public notes are confirmed and approved for publication.
- **Status:** Open for objections through 2026-09-27.

These minutes are the canonical operational record of the working directions and follow-ups recorded above. Proposals and future ADR reviews are not recorded as adopted architectural or product decisions.

Corrections after posting are added as dated entries; the seven-day public objection window runs from posting, not from the meeting or earlier review.
