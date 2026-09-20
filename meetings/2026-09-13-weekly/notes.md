# LQAI Committee — Weekly Call (2026-09-13)

*Discussion and action items are summarized without identifying individual speakers or owners. Named ownership is maintained in the private record.*

| Field | Record |
|---|---|
| Date / platform | September 13, 2026 / Zoom |
| Time zone | GMT−7, as identified in the source record |
| Attendees | Houfu Ang, Joel Kaufmann, Alexios Kirillov, Julian Bryant |
| Facilitator | Not recorded in source notes |
| Minutes-taker | Not recorded in source notes |
| Attendee-list and content publication approval | Joel Kaufmann confirmed on 2026-09-20 that all attendees and the information in these public notes are confirmed and approved for publication. |

## Key Outcomes

The call focused on the anticipated Codex for Legal plugin launch, LQAI's orchestration architecture, and the review practices needed to progress the roadmap to 1.0. The discussion also connected sponsorship with a clearer account of what support would fund and how LQAI helps its users.

Practical follow-ups included clearer reviewer guidance, reviews of outstanding ADR work, a trial approach to minor PR corrections, launch-related outreach, and an issue exploring opt-in telemetry. A broader role for LQAI as a model-agnostic orchestration layer drew interest, but no new architecture, sponsorship arrangement, or telemetry implementation was approved.

## Decisions and Agreed Follow-Ups

- Seek community review of the roadmap and outstanding technical ADR work, with clearer guidance on what reviewers should assess.
- Try having the reviewer make straightforward corrections to a contributor's PR and progress the merge, while returning substantive questions and choices to the contributor. This records a working approach discussed with that contributor, not a blanket change to repository merge or approval requirements.
- Explore opt-in telemetry through an issue, with disclosure and user choice central to the discussion.
- Prepare clearer invitations for users to share feedback and connect launch interest with opportunities to build on LQAI.

No formal vote or express ratification of prior minutes was identified. A possible next-week disposition of a technical ADR was mentioned, but these notes do not record that ADR as adopted.

## Plugin Launch and Orchestration

Participants anticipated the Codex for Legal plugin launch and discussed adapting its skills for LQAI, including a broader balance of litigation and transactional work. Source-file availability and compatibility with other environments remained matters to confirm through release materials and testing.

The existing orchestrator was described as limited, and work on a more capable version was reported. A broader proposal would make LQAI a flexible coordination layer through which practitioners could use their own playbooks, different models, existing tools, and potentially local deployments. This would place value on reusable architecture and practitioner control as well as the supplied skills.

Cross-platform skill adaptation was discussed, including Microsoft environments. Reported experience adapting other skills does not establish that the forthcoming plugin will work seamlessly across platforms. The proposed integrations and local-deployment options were not demonstrated or adopted at this call.

## Roadmap and PR Review

The roadmap poll was reported complete with nine responses, with its direction translated into ADR proposals. Community reviewers were sought for the roadmap to 1.0, particularly to assess whether the proposals reflect the discussion and make sense from a governance perspective. More technical ADR work also remained under review.

The discussion emphasized mutual review and useful guidance for contributors with different levels of technical experience. Asking the wider community for help on a specific obstacle was suggested as a practical way to broaden participation.

AI-assisted contributions and reviews can help maintainers, but findings need to be evaluated against the actual scope of a PR. Unrelated improvements may belong in separate issues. Functional demonstrations and model explanations also leave questions about code quality, security, and effects elsewhere in the application that require informed technical review.

## Sponsorship and Launch Outreach

The discussion favored making possible sponsorship requests more concrete: engineering capacity, a defined feature, or an integration, with a clear explanation of the intended result. A sponsorship page and recognition in the README were proposed. Hardware providers, AI labs, and other organizations were considered as possible types of partners.

These ideas require scope, ownership, and terms. No sponsor, budget, deliverable, or partnership status was established by the call.

The plugin launch was seen as an opportunity to invite more people to use and build on LQAI. Launch posts connecting readers with the project were planned. Broader outreach to credible practitioners and potential endorsers remained a proposal; no outreach campaign or spending was authorized.

## Adoption, Value, and Accountability

The committee discussed how practical usefulness, ease of deployment, support, and institutional credibility all influence adoption. The conversation included differing views on vendor loyalty and openness to building or customizing tools. It did not establish comparative product quality or feature parity.

A central point was that zero license cost does not establish lower total cost. Deployment, technical staff, maintenance, support, and responsibility for failures all affect the decision. Different organizations also have different tolerance for risk and different approval processes.

The proposed orchestration role could help distinguish LQAI, but its value needs to be demonstrated through actual workflows and user experience.

## User Relationships and Opt-In Telemetry

The group identified limited visibility into who uses LQAI, what they use it for, and where they need help. Limited feedback could reflect either a small user base or users who do not identify themselves; the call did not establish an active-user count.

Ideas included a voluntary invitation in the README or interface to make contact, explain a use case, and share candid feedback. Technical usage reporting was also discussed, alongside concern about sending information outside a deployment, especially where local operation is important.

The agreed next step was to open an issue exploring opt-in telemetry and clearer user engagement. No telemetry was enabled by the meeting. Data fields, consent flow, storage, access, retention, and implementation remain to be specified and reviewed.

## Action Items

*IDs match the private record. Individual owners are not published. These are follow-ups, not verified completion.*

- [ ] **S13-01:** Try adapting the released plugin skills in another environment and assess compatibility; first-day testing was an expressed intention, subject to availability.
- [ ] **S13-02:** Write clear reviewer guidance and identify an accessible place to publish it.
- [ ] **S13-03:** Review the roadmap to 1.0 ADR proposal, with technical guidance where needed; exact assignments and PR links remain to be confirmed.
- [ ] **S13-04:** Review and respond to comments on the outstanding technical ADR/PR work.
- [ ] **S13-05:** Trial direct reviewer correction of minor execution errors, returning substantive choices to the contributor and observing applicable merge requirements.
- [ ] **S13-06:** Use planned plugin-launch posts to invite readers to explore and build on LQAI.
- [ ] **S13-07:** Open an issue to explore opt-in telemetry and the associated disclosure and user-engagement questions.
- [ ] **S13-08:** Draft a clearer invitation for users to share candid feedback and make contact.

The sponsorship page, broader practitioner outreach, and longer-term orchestration design remain proposals requiring further scoping and ownership.

These notes summarize the supplied meeting record. Release expectations, technical capabilities, adoption observations, and sponsorship possibilities are reports of the discussion, not independently verified findings.

## Ratification

- **Posted (merged):** 2026-09-20
- **Objection window closes:** 2026-09-27 (posted + 7 days)
- **Attendee-list and content publication review:** Joel Kaufmann confirmed on 2026-09-20 that all attendees and the information in these public notes are confirmed and approved for publication.
- **Status:** Open for objections through 2026-09-27.

These minutes are the canonical operational record of the working directions and follow-ups recorded above. Proposals and future ADR reviews are not recorded as adopted architectural or product decisions.

Corrections after posting are added as dated entries; the seven-day public objection window runs from posting, not from the meeting or earlier review.
