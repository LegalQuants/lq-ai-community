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

**Maintenance note:** status checked 2026-08-16. Recheck linked artifacts before each
publication and cite any later merge commit or canonical status change.
