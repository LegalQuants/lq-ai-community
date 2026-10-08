# LQAI Committee — Weekly Call (2026-09-20)

**PUBLIC VERSION — approved for publication.**

*Discussion and action items are summarized without identifying individual speakers or owners. Named ownership is maintained in the private record.*

| Field | Record |
|---|---|
| Date / platform | September 20, 2026 / Zoom |
| Time zone | GMT−7, as identified in the source record |
| Attendees | Houfu Ang, Joel Kaufmann, Alexios Kirillov, Emily Cabrera, Julian Bryant |
| Facilitator | Not recorded in source notes |
| Minutes-taker | Not recorded in source notes |
| Attendee-list and content publication approval | Joel Kaufmann confirmed on 2026-10-08 that the attendee list and public notes are approved for publication. |

## Key Outcomes

The call focused on preparations for LQAI 0.8.0, the next steps for orchestration and plugin skills, and clearer ways for community members to contribute. The canonical records for the four ADR-related agenda topics now show acceptance dated September 20, with the decision PRs and documentation mini-PRD merged after the call. The roadmap to 1.0 remained open for review, while substantial UI redesign was treated as a later workstream behind technical capability.

An agent-facing governance tool was demonstrated, prompting discussion of reminders, more accessible project information, and future in-house governance features. Participants favored avoiding premature formalization and revisiting adoption after clarifying committee roles and decision rules.

Practical follow-ups included improving getting-started guidance, refining the minutes-review process, testing plugin compatibility in another environment, and investigating community-event opportunities. First-party LQ plugin integration was identified as an October priority. Jev applications remained exploratory.

## Decisions and Agreed Follow-Ups

- Record acceptance of ADRs 0035, 0027, 0036–0037, and 0028, as documented in the merged canonical records, and progress implementation under the accepted decisions and documentation mini-PRD.
- Keep the roadmap to 1.0 open for further community review and clearer review steps.
- Give technical capability and orchestration priority over a substantial UI redesign; develop design work with appropriate contributor interest and user feedback.
- Improve community participation guidance and the minutes-review process.
- Share plugin source for a Cowork compatibility test and use the results to inform integration work.
- Revisit governance-tool adoption after the project's decision-making needs and rules are clearer; no deployment or replacement of existing processes was approved.

The merged ADRs record committee ratification on September 20. The transcript does not contain a vote tally or enumerate every written resolution; the canonical documents supply the detailed decision record. Reviewers should flag any mismatch with the intended decisions. Approval of the previous meeting’s minutes remains a separate matter to confirm.

## Release Preparation and ADRs

LQAI 0.8.0 was anticipated in approximately nine or ten days. A collaborative approach in which reviewers make agreed corrections directly was reported to have improved PR flow. This was a working practice discussed among contributors, not a blanket change to repository approval requirements.

**Post-call repository verification — September 20, 2026:** The five ADRs associated with the four agenda topics record committee acceptance dated September 20. Their decision PRs and the documentation-site mini-PRD merged after the call, between 09:49 and 09:54 PDT. The table below separates that verified repository status from implementation still outstanding at the check. Publication approval was subsequently confirmed on October 8, 2026; the technical statuses below remain the September 20 snapshot.

| Call topic | Canonical decision / plan | Verified post-call status | Implementation / follow-up |
|---|---|---|---|
| Orchestrator roadmap | [ADR 0035](https://github.com/LegalQuants/lq-ai/blob/502977f4fee9fcf3fd0d504dda38b0f49583818b/docs/adr/0035-governed-orchestration-run-tree.md) · [PR #567](https://github.com/LegalQuants/lq-ai/pull/567) | Accepted September 20; merged 09:51:45 PDT | Production adoption and script enablement retain separate review and evidence requirements |
| Request budgets and timeouts | [ADR 0027](https://github.com/LegalQuants/lq-ai/blob/502977f4fee9fcf3fd0d504dda38b0f49583818b/docs/adr/0027-request-budgets-and-timeouts.md) · [PR #573](https://github.com/LegalQuants/lq-ai/pull/573) | Accepted September 20; merged 09:49:28 PDT | Timeout implementation [PR #535](https://github.com/LegalQuants/lq-ai/pull/535) remained open; deferred tuning work is recorded in the ADR |
| MinIO → RustFS and deployment migrations | [ADR 0036](https://github.com/LegalQuants/lq-ai/blob/502977f4fee9fcf3fd0d504dda38b0f49583818b/docs/adr/0036-bundled-object-store-rustfs.md) + [ADR 0037](https://github.com/LegalQuants/lq-ai/blob/502977f4fee9fcf3fd0d504dda38b0f49583818b/docs/adr/0037-deployment-migrations-framework.md) · [PR #583](https://github.com/LegalQuants/lq-ai/pull/583) | Both accepted September 20; merged 09:53:19 PDT | Framework, migration, launcher, rehearsal, and release work are separate follow-ups |
| Documentation site | [ADR 0028](https://github.com/LegalQuants/lq-ai/blob/502977f4fee9fcf3fd0d504dda38b0f49583818b/docs/adr/0028-documentation-site-generator-and-hosting.md) · [PR #580](https://github.com/LegalQuants/lq-ai/pull/580); [mini-PRD](https://github.com/LegalQuants/lq-ai/blob/502977f4fee9fcf3fd0d504dda38b0f49583818b/docs/contribute/mini-prds/docsite/README.md) · [PR #511](https://github.com/LegalQuants/lq-ai/pull/511) | ADR accepted and merged 09:50:39 PDT; mini-PRD merged 09:54:15 PDT and marked ready for implementation | Site implementation [PR #581](https://github.com/LegalQuants/lq-ai/pull/581) remained open; plan acceptance is not site publication |

The call’s four topics therefore map to **five ADRs and one mini-PRD**, rather than four individual ADRs. Status snapshot: GitHub API and canonical files checked September 20 at approximately 11:39 PDT, with document links pinned to commit `502977f4fee9fcf3fd0d504dda38b0f49583818b`. Open implementation statuses are as of that check.

The four items discussed were:

1. **Orchestrator roadmap:** introduce an orchestrator profile beyond chat/completion and support the use of LQ plugin skills.
2. **Request budget:** address gateway request-budget and timeout settings.
3. **MinIO to RustFS migration:** respond to reported container-availability failures with the accepted storage replacement and deployment-migration framework.
4. **Documentation-site mini PRD:** progress the plan underlying the documentation site, with further improvement still possible.

The call described an upgrade that reads existing volumes. The accepted storage ADRs record supporting compatibility tests and a synthetic in-place rehearsal, with explicit limits and further release checks. Those tests were not independently rerun for these notes. Acceptance of the plan does not establish a completed rollout or provide an instruction to upgrade.

The roadmap to 1.0 was deferred pending more community comments and review guidance. [PR #564](https://github.com/LegalQuants/lq-ai/pull/564), covering proposed ADRs 0029–0034, remained open at the recorded check.

## UI, Documentation, and Contributor Onboarding

Participants supported focusing first on practical capability and the technical roadmap. UI work remains valuable, but should receive focused design effort, testing, and user feedback rather than becoming an incidental release task. Contributors interested in UI/UX were encouraged to become involved as that work develops.

Documentation, testing, feedback, and coding all offer useful contribution paths. The discussion favored helping contributors find work aligned with their interests. The new documentation site was identified as an area that would benefit from review.

A broader onboarding gap was also identified: interested people may not know where to begin or how their skills fit the project. Proposed improvements to the community repository would explain how members and non-members can participate, try the software, provide feedback, and connect with the community.

The minutes-review workflow and appropriate arrangements for internal committee material were discussed. A simpler review-and-publication process was proposed, but no replacement of existing publication requirements was established by the call.

## Governance-Tool Demonstration and Project Participation

A demonstration explored an MCP-based governance tool through which members use their own agents to retrieve proposals, review information, and submit authenticated votes. The server was described as enforcing a governance protocol without making its own LLM calls. Minutes review, comment reconciliation, reminders, and charter-based decision rules were also described.

These were demonstration descriptions, not independent verification of security, production readiness, or compatibility across agents. Potential benefits included more visible reminders and the ability to ask questions about project materials with source references.

Participants saw a possible future role for the tool both in committee work and as an in-house governance feature. Adoption would require clarity on roles, authority, and decision rules. Although a parallel trial was discussed, the later discussion favored parking formal adoption until the need and structure are clearer. No pilot, charter, appointment, or rollout was approved.

## Jev and First-Party Plugin Skills

The discussion explored whether Jev could help with bounded checks within larger workflows, including diligence, research, and tabular review. Early experience prompted interest in speed and cost, alongside the need to evaluate accuracy. The call did not establish a validated benchmark or approve an integration.

Python-based skills were identified as a possible integration point. Delivery and architecture remained open. Potential research applications were ideas for testing, not established LQAI capabilities.

Separate discussion concerned adapting LQ plugin skills to Cowork and LQAI. A source-sharing and compatibility-testing follow-up was agreed for a citation-checking skill. Earlier assumptions about host capabilities were reported to need correction, reinforcing the need to test actual behavior.

Bringing LQ plugins into LQAI as first-party skills, including the required harness changes, was identified as a priority for October. This was a development priority rather than a fixed completion date. No separate Jev delivery deadline was established.

## Events and Community Visibility

The planned October 8 San Francisco gathering was discussed as an opportunity to introduce the projects through a mix of discussion, demonstrations, and hands-on participation. No specific LQAI version, presenter, or demonstration slot was confirmed in the call.

An offer of logistics help was made, and a possible future event or conference presence in the Dubai/Abu Dhabi region will be explored. No booking, budget, or event commitment was approved.

## Action Items

*IDs match the private record. Individual owners are not published. These are follow-ups, not verified completion.*

- [ ] **S20-01:** Progress the implementation and release work discussed for 0.8.0 under the accepted decisions, with remaining implementation approvals, testing, and release checks.
- [ ] **S20-02:** Review contribution opportunities and follow up on a suitable area; documentation review was discussed.
- [ ] **S20-03:** Improve the community repository's getting-started and participation guidance.
- [ ] **S20-04:** Develop a clearer minutes-review/publication process and appropriate treatment of internal material, consistent with existing requirements.
- [ ] **S20-05:** Share ideas for the getting-started guide.
- [ ] **S20-06:** Share the plugin source-repository link needed for the citation-checking skill test.
- [ ] **S20-07:** Test that skill in Cowork and report results; confirm the exact source and revision.
- [ ] **S20-08:** Identify and address harness gaps for first-party LQ plugin skills in LQAI, as an October priority.
- [ ] **S20-09:** Investigate a possible event or conference opportunity in the Dubai/Abu Dhabi region.

Jev integration, a governance-tool trial, and formal committee arrangements remain proposals requiring further scope or decisions. Event-logistics support was offered without a specific assignment.

## Review and Ratification

- **Draft prepared:** September 20, 2026; revised after same-day repository verification.
- **Attendee-list and content publication approval:** Joel Kaufmann confirmed on 2026-10-08 that the attendee list and public notes are approved for publication.
- **Decision record:** Canonical acceptance and merge status verified as detailed above. Review the written resolutions for accuracy; separately confirm any approval of prior minutes.
- **Posted (merged):** 2026-10-08
- **Objection-window close:** 2026-10-15 (posted + 7 days).
- **Status:** Open for objections through 2026-10-15.

These notes summarize the supplied meeting record and the separately identified post-call repository check. Acceptance and merge status were verified from canonical records; implementation performance, experiment results, and event plans were not independently validated.

Corrections after posting are added as dated entries; the seven-day public objection window runs from posting, not from the meeting or earlier review.
