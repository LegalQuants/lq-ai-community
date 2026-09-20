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

**Maintenance note:** status checked 2026-08-16. Recheck linked artifacts before each
publication and cite any later merge commit or canonical status change.

**2026-09-11 addition:** August 23 rows were checked against the circulated notes,
ADR 0026, and PR #528. PR #530's prior closure is recorded as discussion status in
the minutes, not as a new August 23 decision. Older status rows were not re-audited.

**2026-09-20 addition:** August 30, September 6, and September 13 public notes were approved for publication as confirmed by Joel Kaufmann. New rows index only the working directions and operational follow-ups recorded in those notes; proposed architecture, sponsorship, governance, and telemetry implementations are not treated as adopted decisions. Older status rows were not re-audited.
