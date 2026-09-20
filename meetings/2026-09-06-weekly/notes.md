# LQAI Committee — Weekly Call (2026-09-06)

*Discussion and action items are summarized without identifying individual speakers or owners. Named ownership is maintained in the internal record.*

| Field | Record |
|---|---|
| Date / platform | September 6, 2026 / Zoom |
| Time zone | GMT−7, as identified in the source record |
| Attendees | Houfu Ang, Joel Kaufmann, Jamie Tso, Alexios Kirillov |
| Facilitator | Not recorded in source notes |
| Minutes-taker | Not recorded in source notes |
| Attendee-list and content publication approval | Joel Kaufmann confirmed on 2026-09-20 that all attendees and the information in these public notes are confirmed and approved for publication. |

## Key Outcomes

The call connected the road to 1.0 with two priorities: **operator trust** and **maintainer capacity**. No new survey responses were reported for the preceding week, and the emerging direction would be developed into ADRs for asynchronous approval.

The discussion covered contribution standards, a stronger agent harness, possible engineering support, and the practical requirements of enterprise deployment and customization. A short demonstration of an agent-accessible board portal was proposed for the next call. No new harness architecture, commercial offering, certification rule, or governance system was approved.

## Decisions and Agreed Follow-Ups

- Develop the survey direction into ADR proposals for asynchronous review; those future ADRs are not approved by these minutes.
- Address repository permissions and security-reporting arrangements and progress remediation work.
- Continue responding to review requests on existing PRs.
- Catch up on meeting records and obtain attendee review before publication.
- Arrange a guided board-portal demonstration at the next call; any adoption decision remains separate.

No express ratification of prior minutes or formal vote adopting a new policy was identified in the source transcript.

## Release and Survey Update

A v0.7.2 release that week was reported, along with a recent contribution said to have shortened the test process substantially. These are meeting reports rather than an independent release or performance audit.

The survey discussion emphasized making promised features reliable and strengthening the maintenance arrangements needed to sustain them. The group welcomed the quality of the feedback and the clearer direction. No fixed 1.0 delivery date was adopted at this call.

## Security Response and Reporting

The discussion addressed a previously received report, prepared fixes still to be progressed through merge and release, and improvements to reporting and advisory arrangements. End-of-month completion was discussed as a target, not an established outcome.

The public record does not establish that every reported concern was resolved or that all deployments were unaffected. Detailed findings and operational disclosure arrangements remain outside these public notes.

## Contribution Standards and Maintainer Capacity

The committee considered how to encourage useful contributions without transferring unresolved design and review work to a small maintainer group. Themes included:

- Clear acceptance criteria and evidence that a contribution improves the relevant workflow.
- Bounded changes with solid testing, rather than requiring every contribution to be a best-in-class feature.
- Recording material decisions so later contributors can understand and revisit them.
- Constructive feedback and smaller tasks that support learning and participation.
- Narrowly scoped residency projects built on LQAI where appropriate to the participant's experience and aims.

Linking contributions with training or certification was proposed, but no new requirement was adopted. Additional maintainer capacity and a repeatable release process were discussed as ways to create room for larger architectural work.

## Harness Architecture and Engineering Support

The existing harness was discussed as a candidate for further development, including richer multi-turn behavior. Reviewing established approaches and obtaining engineering input were suggested before committing to a particular implementation.

Possible sponsorship or engineering help was discussed alongside the need for a defined problem, clear scope, and a sustainable maintenance arrangement. General engineering choices and legal-workflow needs—such as citation and verification behavior—both require attention. No framework, sponsor, team, or delivery schedule was selected.

## Enterprise Deployment and Sustainable Support

The discussion explored whether community expertise could support deployment, customization, training, and ongoing maintenance for organizations interested in LQAI. Important questions remained about feature fit, hosting arrangements, who would provide support, and the value offered alongside existing software or an organization's own IT capability.

A tailored deployment or fork, with suitable improvements contributed upstream, was considered as one possible approach. Training on existing tools, embedded customization, and more advanced capabilities were discussed as different levels of service. These were exploratory models, not an approved offering, customer commitment, or pricing decision.

Customization and local control may justify an upfront investment, but the discussion did not establish that a supported LQAI deployment would be cheaper than commercial alternatives. Deployment interest would be reported back if it developed further.

## Governance Experiment

An early agent-accessible board portal was proposed for a guided demonstration of roughly ten minutes at the next call. The group was open to seeing how it might help record decisions and make review practices more consistent.

Membership rules, voting thresholds, and decision procedures remained questions to clarify. Willingness to see or test the tool does not adopt it, amend governance, or create a new voting rule.

## Action Items

*Internal action IDs are retained so the two versions can be reconciled. Individual owners are not published.*

- [ ] **S06-01:** Draft ADR proposals reflecting the survey direction and circulate them for asynchronous approval.
- [ ] **S06-02:** Address the repository permissions needed for security-advisory work and confirm the result.
- [ ] **S06-03:** Complete reporting-process arrangements and progress prepared fixes through review, merge, and release.
- [ ] **S06-04:** Respond to review requests on existing PRs.
- [ ] **S06-05:** Prepare outstanding meeting notes and obtain attendee review/approval before publication.
- [ ] **S06-06:** Confirm the next-call slot and demonstrate the board portal with guidance for participants.
- [ ] **S06-07:** Report back on further enterprise-deployment interest if it develops.

Harness research, additional engineering input, contributor incentives, and a commercial support model remain proposals requiring further scoping and ownership.

## Takeaway

Progress toward 1.0 depends on reliable software and a sustainable process for maintaining it. Clearer contribution expectations, stronger review capacity, and focused architectural research can support that work; deployment and governance experiments still require evaluation before becoming commitments.

These are retrospective meeting notes. Statements about project behavior, security, and commercial possibilities are reports of the discussion, not independent verification.

## Ratification

- **Posted (merged):** 2026-09-20
- **Objection window closes:** 2026-09-27 (posted + 7 days)
- **Attendee-list and content publication review:** Joel Kaufmann confirmed on 2026-09-20 that all attendees and the information in these public notes are confirmed and approved for publication.
- **Status:** Open for objections through 2026-09-27.

These minutes are the canonical operational record of the working directions and follow-ups recorded above. Proposals and future ADR reviews are not recorded as adopted architectural or product decisions.

Corrections after posting are added as dated entries; the seven-day public objection window runs from posting, not from the meeting or earlier review.
