# Meeting records

Convention per ADR 0022 (lq-ai PR [#311](https://github.com/LegalQuants/lq-ai/pull/311)):
**one folder per meeting**, named `meetings/YYYY-MM-DD-<topic>/`, containing `notes.md`
plus any shareable artifacts from that meeting.

```
meetings/
├── README.md                    ← this file (the convention)
├── _template/
│   └── notes.md                 ← copy this to start a new record
├── 2026-07-19-weekly/
│   └── notes.md
└── 2026-07-26-weekly/
    └── notes.md
```

## Naming

- **Date:** ISO 8601 (`YYYY-MM-DD`) — the meeting date in the committee's announced time
  zone. ISO dates sort chronologically in every file listing.
- **`<topic>`:** short, lowercase, hyphenated. The standing call is `weekly`
  (`2026-07-26-weekly/`). Special sessions get a descriptive slug
  (`2026-08-14-release-planning/`).
- **Artifacts:** files shared at the meeting live in the same folder alongside `notes.md`
  (e.g. `roadmap-snapshot.pdf`), with descriptive lowercase-hyphenated names. Never
  transcripts or recordings.

## `notes.md` structure

Copy [`_template/notes.md`](_template/notes.md). Required sections: the header table
(date, platform, facilitator, minutes-taker, attendees, and attendee-list approval),
**Decisions**, **Action items** (each with anonymized ownership), and the
**Review, approval, and publication** block. A discussion summary is encouraged but optional. If a header fact is unavailable, write
`Not recorded in source notes`; do not infer it or leave a publication placeholder.

## Review and publication process

This implements the process approved in [issue #3](https://github.com/LegalQuants/lq-ai-community/issues/3),
subject to the coordinated transition below. The canonical rules are in
[lq-ai GOVERNANCE.md](https://github.com/LegalQuants/lq-ai/blob/main/GOVERNANCE.md#meetings)
and [ADR 0022](https://github.com/LegalQuants/lq-ai/blob/main/docs/adr/0022-committee-governance-and-meeting-records.md).

1. **Prepare and circulate internally.** Share internal notes and the proposed public
   version with committee members after the meeting. Record the circulation date/time,
   time zone, and an explicit review deadline seven days later. Keep internal notes,
   discussion, and private review exchanges private.
2. **Allow seven days for review.** The window begins with internal circulation, not the
   meeting date or GitHub publication. All committee members, including those absent
   from the call, may raise corrections or objections.
3. **Resolve objections and record approval.** If no objections are raised by the
   deadline, record approval through the no-objection process (silence is assent).
   Resolve outstanding objections before publication. Record the approval date, basis,
   and confirming person or body without disclosing private exchanges. Expiry alone
   does not establish that no objections were raised.
4. **Publish the approved public version.** Joel Kaufmann opens the publication PR after
   review is complete, as time permits. One other attendee checks the publication
   checklist below; attendee-list confirmation remains a separate requirement.
   Include the corresponding decision-log rows. Record GitHub publication separately
   when the PR merges. Publication does not restart the seven-day window.
5. **Preserve later corrections.** Raise an issue or follow-up PR. Published minutes are
   append-only: add dated `Correction (YYYY-MM-DD):` entries rather than silent edits.
   Material changes to recorded decisions, attendee identification, or publishable
   content require internal recirculation and a fresh seven-day window before publishing
   the correction. Typographical corrections do not restart the window.

The public record must separately identify internal circulation, objection deadline,
approval date and basis, and GitHub publication. Do not publish internal review links or
private correspondence. For an unavailable fact use `Not recorded in source notes`;
missing evidence of completed review or approval must be resolved before publication.
In a publication PR only, the GitHub publication field may read `Pending merge`; replace
it with the actual merge date after publication without guessing a date in advance.

## Transition clarification (2026-10-13)

**Proposed effective-date rule for review:** no calendar effective date was specified.
Apply the new process to records first circulated internally on or after both coordinated
PRs (this repository and [lq-ai #721](https://github.com/LegalQuants/lq-ai/pull/721))
have merged. Until
then, and for records already in review at that point, retain the previous public-posting
rule. Record the actual effective date here in a dated follow-up once both merges occur.
The documentation-site launch-link owner remains unassigned for review in issue #3.

Previously published records retain their recorded posting dates and objection deadlines.
In particular, the [August 30](2026-08-30-weekly/notes.md),
[September 6](2026-09-06-weekly/notes.md), and [September 13](2026-09-13-weekly/notes.md)
records retain their September 27, 2026 public objection deadline. The subsequently
published [September 20](2026-09-20-weekly/notes.md) record retains its October 15, 2026
deadline. This clarification neither restarts nor shortens those windows, nor declares
an objection resolved or a record ratified solely because its deadline has passed.

Do not backfill historical internal circulation, review, or approval dates without
confirmation. Add verified information as dated clarifications; preserve the original
entries and link any corresponding decision-log correction. Older references to public
posting describe the process used for those records and are not the prospective rule.

## Historical backlog

ADR 0022 called for bootstrap records from 2026-06-28, 2026-07-05, 2026-07-12, and
2026-07-19. Verified source material was available here only for 2026-07-19. The first
three records remain outstanding and should be added only from source material reviewed
by participants; do not reconstruct them from memory.

## Before you publish

- [ ] No transcript or recording content — the minutes are the record (ADR 0022).
- [ ] No meeting links, dial-ins, passcodes, or credentials. Calendar invites and Slack
      carry logistics; the public record never does.
- [ ] No confidential, privileged, or client-identifying material.
- [ ] Attendee list confirmed by at least one other attendee or by the committee
      collectively; the reviewer or approving body is identified in the record.
- [ ] Statements about identifiable individuals reviewed for accuracy and neutral phrasing.
- [ ] Each decision cross-linked to its canonical artifact (ADR / PR / issue) in lq-ai, and
      a corresponding row added to [`../decisions/README.md`](../decisions/README.md) in the
      same PR.
- [ ] Public discussion and action ownership anonymized; internal notes and private review
      exchanges excluded.
- [ ] Applicable review window completed, objections resolved, and approval date and basis
      recorded; any material changes recirculated for a fresh seven-day window.
- [ ] Internal circulation, objection deadline, approval, and GitHub publication recorded
      separately under the applicable process; no historical dates inferred.
