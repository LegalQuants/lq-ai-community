# Decision log

Chronological index of LQ.AI committee decisions. **The canonical text of every
architectural or product decision lives in the lq-ai repository** (as an ADR, PR, or
issue); this log indexes decisions and links to the minutes that record them. If this
table and a canonical artifact ever disagree, the canonical artifact controls.

Add a row here in the same PR that posts the minutes recording the decision.

| Date | Decision | Canonical record | Minutes | Status |
|---|---|---|---|---|
| 2026-07-26 | Adopt committee governance and meeting-records model (root `GOVERNANCE.md`; public minutes in `lq-ai-community`; 7-day objection window) | ADR 0022 — [lq-ai PR #311](https://github.com/LegalQuants/lq-ai/pull/311) | [2026-07-26-weekly](../meetings/2026-07-26-weekly/notes.md) | Confirmed at call; PR merged 2026-07-27 (`8c1dd5e`); canonical status text remains Proposed |
| 2026-07-26 | Adopt uv-managed lockfiles for `gateway/` and `api/` (`uv.lock` committed; `uv sync --frozen` in CI/images; `uv lock --check` gate) | ADR 0023 — [lq-ai PR #312](https://github.com/LegalQuants/lq-ai/pull/312) | [2026-07-26-weekly](../meetings/2026-07-26-weekly/notes.md) | Confirmed at call; PR merged 2026-07-27 (`2b7112b`) |
| 2026-07-26 | Adopt expansion direction and contribution routing (skills → lq-skills; sources → lq-ai; corpora → org-level repos; scope carve-ins → mini-PRDs); **litigation carve-in narrowed to research and drafting only** | Proposed ADR 0024 — [lq-ai PR #313](https://github.com/LegalQuants/lq-ai/pull/313) | [2026-07-26-weekly](../meetings/2026-07-26-weekly/notes.md) | Confirmed at call; PR remains open (checked 2026-08-02) |
| 2026-07-26 | Track releases v0.6.3 and v0.7 via GitHub milestones | These minutes (canonical operational record) | [2026-07-26-weekly](../meetings/2026-07-26-weekly/notes.md) | Confirmed |
| 2026-07-26 | Continue recording decisions transparently and bring Kevin Keller up to date before a public release | These minutes (canonical operational record) | [2026-07-26-weekly](../meetings/2026-07-26-weekly/notes.md) | Confirmed |
| 2026-07-26 | Zoom confirmed as the standing meeting platform | These minutes (canonical operational record) | [2026-07-26-weekly](../meetings/2026-07-26-weekly/notes.md) | Confirmed |
| 2026-07-19 | Adopt ADR-first decision workflow as the working direction | Formalized in ADR 0022 — [lq-ai PR #311](https://github.com/LegalQuants/lq-ai/pull/311) | [2026-07-19-weekly](../meetings/2026-07-19-weekly/notes.md) | PR merged 2026-07-27; canonical status text remains Proposed |
| 2026-07-19 | Move the standing call to Zoom | These minutes (canonical operational record) | [2026-07-19-weekly](../meetings/2026-07-19-weekly/notes.md) | Confirmed |
| 2026-07-19 | Commission three ADRs for community comment before accepting related implementation work | [lq-ai PR #311](https://github.com/LegalQuants/lq-ai/pull/311), [#312](https://github.com/LegalQuants/lq-ai/pull/312), and [#313](https://github.com/LegalQuants/lq-ai/pull/313) | [2026-07-19-weekly](../meetings/2026-07-19-weekly/notes.md) | Submitted; #311 and #312 merged, #313 remains open (checked 2026-08-02) |
| 2026-08-09 | Approve versioning policy + version-consistency gate + pipeline ordering (minor bump signals breaking changes; patch releases use a third number) | ADR 0025 — [lq-ai PR #487](https://github.com/LegalQuants/lq-ai/pull/487) | [2026-08-09-weekly](../meetings/2026-08-09-weekly/notes.md) | Approved and merged; clears the v0.7.0 release blocker |
| 2026-08-09 | Approve routing for jurisdiction and practice-area expansion contributions (four routing shapes + coverage-map claim ledger) | ADR 0024 — [lq-ai PR #313](https://github.com/LegalQuants/lq-ai/pull/313) | [2026-08-09-weekly](../meetings/2026-08-09-weekly/notes.md) | Approved and merged (supersedes the 2026-07-26 "open" status); unblocks the stalled expansion proposals across lq-ai/lq-skills |
| 2026-08-09 | Adopt meeting-notes process (draft after each call, ratified at the following week's call, published with anonymized speaker attribution) | These minutes (canonical operational record) | [2026-08-09-weekly](../meetings/2026-08-09-weekly/notes.md) | Confirmed |
| 2026-08-16 | Defer the document-ingestion dependency decision (keep and integrate vs. replace/remove vs. pluggable ingestion layer) pending an ADR for group review at the next meeting | These minutes (canonical operational record of the deferral); forthcoming ADR will be canonical for the eventual decision | [2026-08-16-weekly](../meetings/2026-08-16-weekly/notes.md) | Deferred; ADR pending |

| 2026-08-23 | Delay planned v0.7.1 release by one week to include the web UI dependency update | These minutes (canonical operational record of scheduling decision) | [2026-08-23-weekly](../meetings/2026-08-23-weekly/notes.md) | Recorded at call; public objection window through 2026-09-18 |
| 2026-08-23 | Accept removal of unused upstream Docling integration; defer pluggable ingestion as DE-387 | [ADR 0026](https://github.com/LegalQuants/lq-ai/blob/main/docs/adr/0026-document-ingestion-parser-and-docling.md) — [lq-ai PR #528](https://github.com/LegalQuants/lq-ai/pull/528) | [2026-08-23-weekly](../meetings/2026-08-23-weekly/notes.md) | ADR records acceptance 2026-08-23; PR merged 2026-08-26 (`e42f842e`); public minutes window through 2026-09-18 |
| 2026-08-23 | Frame the 1.0 consultation as a survey, not a binding ballot; roadmap scope remains open | These minutes (canonical operational record) | [2026-08-23-weekly](../meetings/2026-08-23-weekly/notes.md) | Recorded at call; public objection window through 2026-09-18 |

| 2026-08-30 | Prioritize operator trust, acknowledge API-only use as unsupported, and leave the 1.0 date uncommitted pending clearer capacity | These minutes (canonical operational record) | [2026-08-30-weekly](../meetings/2026-08-30-weekly/notes.md) | Working directions; no complete roadmap formally adopted; public objection window through 2026-09-27 |
| 2026-08-30 | Keep the survey open another week and coordinate individual reminders | These minutes (canonical operational record) | [2026-08-30-weekly](../meetings/2026-08-30-weekly/notes.md) | Operational follow-ups recorded at call; public objection window through 2026-09-27 |
| 2026-09-06 | Develop survey direction into ADR proposals for asynchronous review | These minutes (canonical operational record) | [2026-09-06-weekly](../meetings/2026-09-06-weekly/notes.md) | Follow-up only; future ADRs not approved by these minutes; public objection window through 2026-09-27 |
| 2026-09-06 | Progress security-reporting and permissions work, PR reviews, and reviewed meeting records; arrange a guided board-portal demonstration | These minutes (canonical operational record) | [2026-09-06-weekly](../meetings/2026-09-06-weekly/notes.md) | Operational follow-ups; no governance-system adoption; public objection window through 2026-09-27 |
| 2026-09-13 | Seek roadmap and technical ADR reviews with clearer reviewer guidance | These minutes (canonical operational record) | [2026-09-13-weekly](../meetings/2026-09-13-weekly/notes.md) | Review follow-up; no ADR adoption recorded; public objection window through 2026-09-27 |
| 2026-09-13 | Trial direct reviewer correction of minor PR errors while returning substantive choices to the contributor and observing merge requirements | These minutes (canonical operational record) | [2026-09-13-weekly](../meetings/2026-09-13-weekly/notes.md) | Limited working approach; no blanket policy change; public objection window through 2026-09-27 |
| 2026-09-13 | Explore opt-in telemetry through an issue and prepare clearer user-feedback invitations and launch outreach | These minutes (canonical operational record) | [2026-09-13-weekly](../meetings/2026-09-13-weekly/notes.md) | Exploration and outreach follow-ups; no telemetry implementation approved; public objection window through 2026-09-27 |

| 2026-09-20 | Accept governed orchestration roadmap (ADR 0035) | [lq-ai PR #567](https://github.com/LegalQuants/lq-ai/pull/567) | [2026-09-20-weekly](../meetings/2026-09-20-weekly/notes.md) | Canonical acceptance dated September 20 and same-day merges verified in the notes; implementation is separate; public objection window through 2026-10-15 |
| 2026-09-20 | Accept request budgets and timeouts (ADR 0027) | [lq-ai PR #573](https://github.com/LegalQuants/lq-ai/pull/573) | [2026-09-20-weekly](../meetings/2026-09-20-weekly/notes.md) | Canonical acceptance dated September 20 and same-day merges verified in the notes; implementation is separate; public objection window through 2026-10-15 |
| 2026-09-20 | Accept RustFS storage replacement and deployment migrations framework (ADRs 0036–0037) | [lq-ai PR #583](https://github.com/LegalQuants/lq-ai/pull/583) | [2026-09-20-weekly](../meetings/2026-09-20-weekly/notes.md) | Canonical acceptance dated September 20 and same-day merges verified in the notes; implementation is separate; public objection window through 2026-10-15 |
| 2026-09-20 | Accept documentation-site plan (ADR 0028 and mini-PRD) | [lq-ai PR #580](https://github.com/LegalQuants/lq-ai/pull/580) and [#511](https://github.com/LegalQuants/lq-ai/pull/511) | [2026-09-20-weekly](../meetings/2026-09-20-weekly/notes.md) | Canonical acceptance dated September 20 and same-day merges verified in the notes; implementation is separate; public objection window through 2026-10-15 |
| 2026-09-20 | Progress contribution guidance, minutes review, plugin compatibility testing, and first-party plugin integration; keep roadmap review open and revisit governance-tool adoption later | These minutes (canonical operational record) | [2026-09-20-weekly](../meetings/2026-09-20-weekly/notes.md) | Follow-ups and priorities only; no governance-tool adoption, Jev integration, or event commitment approved; public objection window through 2026-10-15 |

| 2026-09-27 | No meeting held (cancelled for LQ Residency Demo Day) | [Cancellation record](../meetings/2026-09-27-weekly/notes.md) | [2026-09-27-weekly](../meetings/2026-09-27-weekly/notes.md) | No decisions |
| 2026-10-04 | Review the pending ADRs (tabular bulk operations, identity, community skill catalog, UI component system) ahead of the next meeting; give the Road to 1.0 ADR a final review before merging | These minutes (canonical operational record); ADR/PR numbers not recorded in source | [2026-10-04-weekly](../meetings/2026-10-04-weekly/notes.md) | Review follow-ups only; no ADR acceptance recorded on October 4; public objection window runs seven days from merge |
| 2026-10-04 | Add contributor stories to the community repository; continue posting starter issues roughly every two weeks | These minutes (canonical operational record) | [2026-10-04-weekly](../meetings/2026-10-04-weekly/notes.md) | Operational follow-ups; public objection window runs seven days from merge |
| 2026-10-04 | Keep UI improvement a medium-term priority and consolidate UI feedback before further discussion | These minutes (canonical operational record) | [2026-10-04-weekly](../meetings/2026-10-04-weekly/notes.md) | Working direction; public objection window runs seven days from merge |
| 2026-10-04 | Align the draft sponsorship framework with the LegalQuants organization before any external use | These minutes (canonical operational record) | [2026-10-04-weekly](../meetings/2026-10-04-weekly/notes.md) | No sponsors, tiers, or prices approved; public objection window runs seven days from merge |
| 2026-10-11 | No meeting held (cancelled — scheduling conflicts) | [Cancellation record](../meetings/2026-10-11-weekly/notes.md) | [2026-10-11-weekly](../meetings/2026-10-11-weekly/notes.md) | No decisions |

| 2026-10-18 | Adopt ADR for workspace events, Today View, and staged read-only email (ADR 0042, provisional); approval of ADR text and staged scope only, not implementation | [lq-ai PR #677](https://github.com/LegalQuants/lq-ai/pull/677) | [2026-10-18-weekly](../meetings/2026-10-18-weekly/notes.md) | Proposed for adoption with no objection; PR open at 2026-10-19 check; public objection window runs seven days from merge |
| 2026-10-18 | Adopt design-system primitives ADR with narrowed scope (ADR 0043) | [lq-ai PR #282](https://github.com/LegalQuants/lq-ai/pull/282) | [2026-10-18-weekly](../meetings/2026-10-18-weekly/notes.md) | Proposed for adoption with no objection; PR open at 2026-10-19 check; final ADR number to be confirmed at merge; public objection window runs seven days from merge |
| 2026-10-18 | Adopt Slack/Teams `/lq` quick-ask flow including ADR 0039; Teams JWT validation and other items left to follow-up work | [lq-ai PR #415](https://github.com/LegalQuants/lq-ai/pull/415) | [2026-10-18-weekly](../meetings/2026-10-18-weekly/notes.md) | Proposed for adoption with no objection; PR open at 2026-10-19 check; public objection window runs seven days from merge |
| 2026-10-18 | Select documentation-site version C; deliver a DOCX-to-Markdown ingestion stopgap and the writing skill as first first-party plugin skill in November; defer IT security hand-off document nearer 1.0 | These minutes (canonical operational record) | [2026-10-18-weekly](../meetings/2026-10-18-weekly/notes.md) | Working directions; public objection window runs seven days from merge |
| 2026-10-18 | Pursue LegalQuants-owned Apple Developer and Microsoft developer accounts for release signing and distribution | These minutes (canonical operational record) | [2026-10-18-weekly](../meetings/2026-10-18-weekly/notes.md) | Raised with the LegalQuants organization; no purchase approved by these minutes; public objection window runs seven days from merge |
| 2026-10-18 | LQAI judged not ready for full deployment; agent harness plus first-party open-source skills identified as the path forward; no archive, restart, or re-platform decision | These minutes (canonical operational record) | [2026-10-18-weekly](../meetings/2026-10-18-weekly/notes.md) | Direction only; target users, minimum feature set, and UI ownership remain open; public objection window runs seven days from merge |

**Maintenance note:** status checked 2026-08-16. Recheck linked artifacts before each
publication and cite any later merge commit or canonical status change.

**2026-09-11 addition:** August 23 rows were checked against the circulated notes,
ADR 0026, and PR #528. PR #530's prior closure is recorded as discussion status in
the minutes, not as a new August 23 decision. Older status rows were not re-audited.

**2026-09-20 addition:** August 30, September 6, and September 13 public notes were approved for publication as confirmed by Joel Kaufmann. New rows index only the working directions and operational follow-ups recorded in those notes; proposed architecture, sponsorship, governance, and telemetry implementations are not treated as adopted decisions. Older status rows were not re-audited.

**2026-10-08 addition:** September 20 attendee-list and public-note publication approval confirmed by Joel Kaufmann. These rows preserve the September 20 canonical-status snapshot documented in the notes; older rows and subsequent implementation status were not re-audited.

**2026-10-19 addition:** October 4 attendee-list and public-note publication approval confirmed by Joel Kaufmann on 2026-10-19 after internal circulation without objection. Cancellation records for September 27 and October 11 are indexed for calendar completeness. These records were circulated before the coordinated process change took effect and follow the prior public-posting rule. Older rows were not re-audited.

**2026-10-20 addition:** October 18 attendee-list and public-note approval recorded 2026-10-20 after internal circulation on 2026-10-19 (all attendees confirmed; no objections). The September 27, October 4, and October 11 records were published on 2026-10-19 (PR #6); their `Pending merge` fields are replaced with that date and the objection window runs through 2026-10-26. ADR PR links reflect status at the 2026-10-19 check; older rows were not re-audited.

## Internal-review process clarification — 2026-10-13

[Issue #3](https://github.com/LegalQuants/lq-ai-community/issues/3) records the proposal;
the [October 6 confirmation](https://github.com/LegalQuants/lq-ai-community/issues/3#issuecomment-6006999060)
supports proceeding with the PR. Joel Kaufmann confirmed on October 13 that the team
approved the proposal as proposed. This date records that confirmation, not an inferred
meeting or vote date; no new meeting record is reconstructed.

| Record date | Decision | Canonical source | Implementation status |
|---|---|---|---|
| 2026-10-13 | Clarify community participation and navigation; begin seven-day review at internal circulation; publish approved public notes afterward; recirculate material changes for a fresh window | [GOVERNANCE.md](https://github.com/LegalQuants/lq-ai/blob/main/GOVERNANCE.md#meetings) and [ADR 0022](https://github.com/LegalQuants/lq-ai/blob/main/docs/adr/0022-committee-governance-and-meeting-records.md), coordinated under [issue #3](https://github.com/LegalQuants/lq-ai-community/issues/3) | Team approval confirmed; [governance amendment #721](https://github.com/LegalQuants/lq-ai/pull/721) and effective-date rule remain for PR review |

The [dated transition clarification](../meetings/README.md#transition-clarification-2026-10-13)
proposes prospective effect after both coordinated PRs merge. Existing published deadlines
remain as recorded, including September 27 for the August 30, September 6, and September 13
notes and October 15 for the September 20 notes. No historical circulation dates, objection
outcomes, or ratification statuses are inferred. The documentation-site URL and launch-link
owner remain unassigned for review; the README marks the site forthcoming.
