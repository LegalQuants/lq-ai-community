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
**Decisions**, **Action items** (each with an owner), and the **Ratification** block. A
discussion summary is encouraged but optional. If a header fact is unavailable, write
`Not recorded in source notes`; do not infer it or leave a publication placeholder.

## Posting lifecycle

1. The minutes-taker opens a PR adding the meeting folder. For the bootstrap records only,
   the initial repository push is the posting event.
2. One other attendee reviews against the publication checklist below — a hygiene review,
   not a substance gate.
3. **Merge = posted** for later records. The 7-day objection window runs from posting;
   record the posting date and close date in the Ratification block.
4. Objections or corrections go through an issue or a follow-up PR. Posted minutes are
   **append-only**: corrections are added as dated `Correction (YYYY-MM-DD):` entries,
   never silent edits.
5. At window close, update the Ratification block to `Ratified (silence is assent)` or
   record the objection outcome.

*Steps 2–5 are a suggested implementation of GOVERNANCE.md's 7-day window; the committee
may adjust the mechanics by ordinary lazy consensus.*

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
