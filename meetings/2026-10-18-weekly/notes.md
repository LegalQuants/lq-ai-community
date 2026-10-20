# LQAI Committee — Weekly Call (2026-10-18)

**PUBLIC VERSION — approved for publication.**

*Discussion and action items are summarized without identifying individual speakers or owners. Named ownership is maintained in the private record.*

| Field | Record |
|---|---|
| Date / platform | October 18, 2026 / Zoom |
| Time zone | Pacific (GMT−7), per the transcript timestamps |
| Attendees | Houfu Ang, Joel Kaufmann, Peter Scripps, Alexios Kirillov (joined part-way through) |
| Facilitator | Not recorded in source notes |
| Minutes-taker | Not recorded in source notes |
| Regrets | Not recorded in source notes |
| Attendee-list and content publication approval | All attendees confirmed the attendee list and public notes; approval recorded 2026-10-20, confirmed by Joel Kaufmann. |

## Key Outcomes

No recorded meeting was held on October 11. The 0.9.1 milestone is roughly 80% complete; the remaining maintainer focus this month is the documentation site, and November is earmarked for bringing the first open-source LQ plugin skill — the writing skill — into LQAI as a reference framework for others. The Road to 1.0 milestone has been published, has generated a wave of new issues, and is about 11% complete, with community members already picking up items.

Three contributor ADRs were proposed for adoption on an "adopt first, refine later" basis: workspace events with a Today View and staged read-only email ([lq-ai PR #677](https://github.com/LegalQuants/lq-ai/pull/677), ADR 0042), design-system primitives ([PR #282](https://github.com/LegalQuants/lq-ai/pull/282), ADR 0043), and the Slack/Teams quick-ask flow ([PR #415](https://github.com/LegalQuants/lq-ai/pull/415), with ADR 0039). No objection was recorded. Documentation-site version C (a chat-style interface) has been selected; further review was invited before merge.

The main discussion concerned real-world readiness. A member's pilot deployment at their organization did not proceed, principally because Word (DOCX) document ingestion is not yet supported and because the interface was judged not ready for daily use. Attendees agreed LQAI is not ready for full deployment and discussed product direction openly, including the question of who the product is for. A DOCX-to-Markdown stopgap was targeted for November, and the new agent harness combined with first-party open-source skills was identified as the path forward. No decision to archive, restart, or re-platform the project was made.

Release signing for macOS has depended on a personal developer account that stopped working during the 0.9.0 release; obtaining LegalQuants-owned Apple and Microsoft developer accounts was identified as a priority.

## Decisions and Agreed Follow-Ups

No formal vote tally was recorded. Agreed directions:

- Adopt the three contributor ADRs and continue development, refining through later PRs:
  - [lq-ai PR #677](https://github.com/LegalQuants/lq-ai/pull/677) — workspace events, Today View, and read-only email (ADR 0042, number provisional). Approval is of the ADR text and its staged scope; it does not itself authorize implementation.
  - [lq-ai PR #282](https://github.com/LegalQuants/lq-ai/pull/282) — design-system primitives for the LQ.AI shell (ADR 0043), with narrowed scope.
  - [lq-ai PR #415](https://github.com/LegalQuants/lq-ai/pull/415) — `/lq` slash command and quick-ask flow for Slack and Teams, including ADR 0039 on Slack identity resolution; several items are left to separate follow-up work.
  All three PRs were open when these notes were prepared; final ADR numbers and acceptance dates are recorded in the canonical files on merge.
- Proceed with documentation-site version C; invite further review this week before merging.
- Deliver a DOCX-to-Markdown ingestion stopgap in November, using a library compatible with the project's Apache-2.0 licence.
- Make the writing skill the first first-party open-source plugin skill in LQAI, in November, as a framework for the remaining skills.
- Defer the IT security hand-off document until nearer 1.0, when the security posture is more stable.
- Pursue LegalQuants-owned Apple Developer and Microsoft developer accounts for release signing and distribution.
- Trial monthly contribution snapshots for contributors; explore linking contributions to LQ member profiles.

The three ADR PRs are the canonical record for the adopted decisions; these minutes are the canonical operational record for the remaining items.

## Milestones, PR Backlog, and Road to 1.0

Nothing is being rushed into 0.9.1. The backlog of one contributor's PRs is down to roughly a quarter remaining; a few are deliberately parked, including a security-posture document for customer IT teams, which would otherwise need repeated rewriting as the codebase changes. The Road to 1.0 milestone is expected to be the main source of contribution requests to the community in coming months.

## Documentation Site

Version C was chosen. Reviewers were asked to look now, while changes are cheap, and a "last call" to the wider group was suggested. Enabling the hosting platform's preview comment feature was suggested as a low-friction way to collect feedback; whether it can be switched on will be checked before the next request for review.

## ADRs Proposed for Adoption

1. **Workspace events, Today View, and read-only email** — [PR #677](https://github.com/LegalQuants/lq-ai/pull/677), ADR 0042 (provisional). The ADR proposes an internal workspace-event substrate, a chronological Today View as a new front page, and — later and optionally — read-only email ingestion with advisory triage, each behind its own review gate. The PR contains only the ADR; retention, read-only tool scopes, ownership, and lifecycle questions are explicit prerequisites before any real ingestion, and implementation proceeds through small, maintainer-reviewed PRs. Approach on the call: let it be built, then assess.
2. **Design-system primitives** — [PR #282](https://github.com/LegalQuants/lq-ai/pull/282), ADR 0043. A primitive component layer (buttons, layout, text, alerts, pills, switch, cards, hover cards) backed by a single token file and applied to selected reference components; it does not rewrite all components and defers a semantic colour system. Pending since July while UI direction was settled; reframed as an ADR so the approach is agreed before wider porting. Approach: adopt first, critique later.
3. **Slack/Teams `/lq` quick-ask flow** — [PR #415](https://github.com/LegalQuants/lq-ai/pull/415), including ADR 0039. Adds a `/lq` slash command for Slack and Teams that runs a configured skill through the normal chat path as the linked user, with bridge authentication, fail-closed identity resolution, and a uniform refusal for unlinked accounts. Teams inbound token validation, an admin-UI skill selector, a thread-forward flow, and live-tenant verification are left to separate follow-up work. The maintainer does not use either platform and asked for a contributor to own the experience; one attendee offered to test with their firm's Teams deployment and suggested testing against the community's own Slack. Expected to land in November.

## Community Repository, Governance, and Contributor Recognition

The community-repository and governance PRs were presented as a place for contributors to catch up after missing meetings, and as a documented reflection of the actual approval process (internal circulation, no objection, publication). The community repository was framed as the landing page for *how to contribute*, with the documentation site covering *how to use*; it could also host user experiences and contribution write-ups, and should link to the documentation site once live.

An "LQAI contributions" field has been added to LQ member profile pages. Attendees discussed connecting contribution posts, project progress, and member profiles; a quarterly contributions review; and the LQ member MCP/plugin as a possible vehicle. The maintainer emphasized making it easy for people to post and comment, and noted that PR testing already produces screenshots and artifacts that could support contribution posts. A monthly snapshot showing each contributor where their work sits in the project will be trialled this month. Intermittent contribution — contribute for a few weeks, step away, catch up through the notes, return — was explicitly encouraged.

## Real-World Adoption Feedback and Product Direction

A committee member tested LQAI end-to-end before proposing it internally at their organization, including re-skinning the interface, and ultimately did not proceed. The blockers were DOCX ingestion (Markdown, text, and PDF work; Word documents are refused), attachment-handling errors, and an interface judged not suitable for daily legal work; colleagues preferred incumbent tooling. The member praised the architecture, ADRs, and engineering, regarded the UI as secondary because deployers will rebrand it, and raised the question of whether the project should be refocused or restarted — while stating they were not necessarily advocating dropping it. The maintainer also sees the DOCX gap in demos and testing and called this one of the few real-world implementation attempts to date.

Other attendees echoed the concerns from their own deployments: the product is not ready for full deployment and must become more useful and easier to deploy. One framing was that the recurring unanswered question is *who the product is for* — which users, which tasks, and what minimum viable feature set — without which feature prioritization is difficult.

The maintainer's going-forward view: there is significant technical debt; the original "completion tool" design (prompt plus skill produces an output) is dated; the new agent harness, built around the open-source plugin skills, offers a sound basis for real use. What attracted contributors was the gateway and API rather than the front end. A person or team to own the UI and user journey is needed and has been hard to find. If the technical debt proves too great, starting over remains acceptable. Attendees also noted that deployers increasingly expect "out-of-the-box plus customization," and that applications are consolidating into single windows through MCP and plugin UIs — trends the project should watch.

A member's firm front end on LQAI and another member's fork were mentioned as further sources of feedback to collect.

## Release Signing and Developer Accounts

Unsigned macOS builds are flagged as unsafe. Signing has relied on a personal Apple Developer account, which stopped working during the 0.9.0 release, causing the release action to fail. The maintainer recommended that LegalQuants hold its own Apple Developer account (approximately US$100 per year) and a Microsoft developer account for store and plugin distribution. The matter is being raised with the LegalQuants organization; the macOS application may not be released until it is resolved.

## Community Pickup

Regular calls for contributions in the community chat continue to draw responses, and LQ members contribute each month. External usage remains unknown because telemetry has not been implemented; repository clone and visitor statistics show real but modest interest relative to other LQ projects. Broader promotion has been held back pending UI improvement.

## Action Items

*IDs match the private record. Individual owners are not published. These are follow-ups, not verified completion.*

- [ ] **O18-01:** Circulate October 18 minutes (internal and public) to the group.
- [ ] **O18-02:** Review documentation-site version C; check whether preview comments can be enabled; send a last call for feedback before merge.
- [ ] **O18-03:** Review documentation-site version C and give feedback this week.
- [ ] **O18-04:** Merge the three adopted ADR PRs ([#677](https://github.com/LegalQuants/lq-ai/pull/677), [#282](https://github.com/LegalQuants/lq-ai/pull/282), [#415](https://github.com/LegalQuants/lq-ai/pull/415)) with final ADR numbers and status lines; continue development.
- [ ] **O18-05:** Test the Slack/Teams integration when available.
- [ ] **O18-06:** Scope a November DOCX-to-Markdown stopgap and seek a volunteer owner.
- [ ] **O18-07:** Build the writing skill as the first first-party plugin skill (November) and document the framework.
- [ ] **O18-08:** Explore the LQ member MCP and profile contribution field; confirm ownership.
- [ ] **O18-09:** Trial monthly contribution snapshots, starting this month.
- [ ] **O18-10:** Share reflections and open issues from a member's firm deployment.
- [ ] **O18-11:** Raise LegalQuants-owned Apple and Microsoft developer accounts with the organization.
- [ ] **O18-12:** Revisit the IT security hand-off document nearer 1.0.
- [ ] **O18-13:** Define target users and a minimum viable feature set; identify a UI / user-journey owner (unassigned).
- [ ] **O18-14:** Link the community repository to the documentation site once live.

## Review, approval, and publication

*This record was first circulated after lq-ai-community PR #5 merged but while lq-ai #721 remained open, so the prior public-posting rule formally applies under the [transition clarification](../README.md#transition-clarification-2026-10-13); the seven-day internal review was run in any event.*

- **Draft prepared:** October 19, 2026.
- **Internal circulation:** 2026-10-19, 13:18 (Pacific), LQAI Slack channel.
- **Objection deadline:** 2026-10-26, 13:18 (Pacific; circulation + 7 days).
- **Approval date:** 2026-10-20
- **Approval basis and confirmation:** All attendees (Houfu Ang, Peter Scripps, Alexios Kirillov, Joel Kaufmann) affirmatively confirmed the notes and attendee list before the deadline; no objections were raised. Confirmed by Joel Kaufmann.
- **Attendee-list publication review:** Confirmed by all attendees; recorded by Joel Kaufmann on 2026-10-20.
- **GitHub publication (merged):** Pending merge
- **Objection-window close (prior rule):** Merge date + 7 days.
- **Status:** Approved for publication — open for public objections for seven days after merge.

These notes summarize the Zoom transcript of the call; statements about product readiness, traffic, and deployment experience reflect participants' reports and were not independently verified. Corrections after publication are added as dated entries.
