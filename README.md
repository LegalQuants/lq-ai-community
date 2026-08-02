# LQ.AI Community

Meeting minutes and governance records for the [LQ.AI](https://github.com/LegalQuants/lq-ai) open-source project.

> **Status:** Bootstrapped 2026-07-26 following the committee's recorded decision on
> ADR 0022. The implementing lq-ai PR
> [#311](https://github.com/LegalQuants/lq-ai/pull/311) merged on 2026-07-27. As of
> 2026-08-02, the canonical ADR 0022 and `GOVERNANCE.md` still label themselves
> **Proposed**. Those canonical files control; this repository records the committee
> decision and does not independently change their status.

## Publication Requirements

Before publishing or merging meeting-related materials:

1. Do not include meeting access information. Remove all meeting links, dial-in numbers, passcodes, and credentials.
2. Do not include transcripts or recordings.
3. Do not include protected information. Exclude confidential, privileged, and client-identifying material.
4. Verify attendee lists. A second attendee or the committee collectively must confirm
   the list before publication, and the record must identify the reviewer or approving
   body.
5. Review statements about identifiable individuals. Confirm accuracy and use neutral, factual phrasing.
6. Document decisions consistently. Cross-link each decision to its canonical LQ-AI artifact and include the corresponding decision-log row in the same pull request.
7. Do not guess at missing facts. Use `Not recorded in source notes` until a participant
   supplies a verified correction.

## What lives here?

| Content | Location |
|---|---|
| Meeting minutes — the public record of committee calls | [`meetings/`](meetings/) |
| Chronological index of committee decisions | [`decisions/`](decisions/) |

## What does not live here?

Per the proposed routing direction in ADR 0024 (open lq-ai PR
[#313](https://github.com/LegalQuants/lq-ai/pull/313), status checked 2026-08-02) and the
main repository's single-source-of-truth practice:

| Content | Canonical home |
|---|---|
| Code, PRD, ADRs, API/DB contracts | [LegalQuants/lq-ai](https://github.com/LegalQuants/lq-ai) |
| Governance rules (`GOVERNANCE.md`) | [lq-ai repository root](https://github.com/LegalQuants/lq-ai/blob/main/GOVERNANCE.md) (added by PR #311) |
| Skills | [LegalQuants/lq-skills](https://github.com/LegalQuants/lq-skills) |
| Raw transcripts and recordings | **Nowhere public.** They are not published; the minutes are the record (ADR 0022). |

Architectural and product decisions recorded here link back to their canonical artifact
(ADR, PR, or issue) in lq-ai. For an operational decision with no separate artifact, the
posted minutes are identified as the canonical operational record. This repository indexes
decisions; it does not restate canonical architectural or product decisions.

## Minutes and Ratification

Minutes are public: decisions, action items, and attendee lists are published. Committee
members who miss a call may register agreement or objection on posted minutes within
**7 days**; silence after 7 days is assent to the recorded decisions. (GOVERNANCE.md, via
lq-ai PR #311.)

The initial repository push counts as posting for the bootstrap records. Their initial
publication date is 2026-08-02 and their objection window closes on 2026-08-09. For later
records, merging the minutes PR is the posting event.

See [`meetings/README.md`](meetings/README.md) for the folder convention, the minutes
template, and the posting lifecycle.

## Historical Record Backlog

ADR 0022 called for the repository to be seeded with records for the 2026-06-28,
2026-07-05, 2026-07-12, and 2026-07-19 calls. Only the 2026-07-19 record could be prepared
from the source material available for this bootstrap; the three earlier records remain
outstanding. They must not be reconstructed or published without source material and
participant review. The 2026-07-26 call is also included because it confirmed the
bootstrap decisions.

## Rules for Final Publication

Nothing is committed here until it clears the checklist in
[`meetings/README.md`](meetings/README.md#before-you-publish). In particular: **no
transcripts or recordings, no meeting links or credentials, and no confidential,
privileged, or client-identifying material — ever.**
