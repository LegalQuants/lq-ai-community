# LQ.AI Community

This is the community repository for following and participating in
[LQ.AI](https://github.com/LegalQuants/lq-ai), an open-source AI platform for legal teams.
It is also the public home for approved LQ.AI Committee meeting notes. Here you can follow
published discussions, recorded decisions, and links to the work shaping the project.

## Follow the project

| Destination | Purpose |
|---|---|
| [Meeting notes](meetings/) | Read approved public committee meeting records |
| [Decision log](decisions/) | Follow recorded decisions and their supporting artifacts |
| [LQ.AI project](https://github.com/LegalQuants/lq-ai) | Explore the software and development activity |
| [Contribution guide](https://github.com/LegalQuants/lq-ai/blob/main/CONTRIBUTING.md) and [project issues](https://github.com/LegalQuants/lq-ai/issues) | Find ways to contribute, offer feedback, and raise ideas |
| **LQ-AI documentation — forthcoming.** | The official documentation-site URL will be added once verified at launch; link owner remains unassigned for review in [issue #3](https://github.com/LegalQuants/lq-ai-community/issues/3) |
| [LegalQuants](https://www.legalquants.com/) | **Who we are:** learn about the broader community and its activities |

## What lives here and where related work lives

This repository provides the community record of published discussions and decisions.
The main LQ.AI repository is the home for software development and canonical technical
and governance artifacts. The forthcoming documentation site will provide published
project documentation; the LegalQuants website introduces the broader community.

| Content | Canonical home |
|---|---|
| Approved public meeting notes | [`meetings/`](meetings/) |
| Chronological index of committee decisions | [`decisions/`](decisions/) |
| Code, PRD, ADRs, API/DB contracts | [LegalQuants/lq-ai](https://github.com/LegalQuants/lq-ai) |
| Governance rules | [lq-ai `GOVERNANCE.md`](https://github.com/LegalQuants/lq-ai/blob/main/GOVERNANCE.md) |
| Skills | [LegalQuants/lq-skills](https://github.com/LegalQuants/lq-skills) |
| Raw transcripts and recordings | **Nowhere public.** The minutes are the public record ([ADR 0022](https://github.com/LegalQuants/lq-ai/blob/main/docs/adr/0022-committee-governance-and-meeting-records.md)). |

Architectural and product decisions recorded here link back to their canonical artifact
(ADR, PR, or issue) in lq-ai. For an operational decision with no separate artifact, the
posted minutes are identified as the canonical operational record. This repository indexes
decisions; it does not restate canonical architectural or product decisions.

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

Public discussion and action ownership remain anonymized. Confirmed attendee lists and
the identity of the attendee-list reviewer or approving body remain part of the record.
Internal notes and private review exchanges are not published.

## Minutes and Ratification

Under the process approved in [issue #3](https://github.com/LegalQuants/lq-ai-community/issues/3),
internal notes and the proposed public version circulate internally with an explicit
review deadline. Committee members, including those who missed the call, have **seven
days from internal circulation** to raise corrections or objections. If there are no
objections by the deadline, approval is recorded through the no-objection process;
outstanding objections must be resolved before publication.

Joel Kaufmann publishes the approved public version to GitHub after review is complete,
as time permits. Publication does not restart the seven-day window. Material changes to
recorded decisions, attendee identification, or publishable content require recirculation
and a fresh seven-day window; typographical corrections do not. Later corrections use
issues or follow-up PRs and dated entries to preserve the historical record.

See [the review and publication process](meetings/README.md#review-and-publication-process)
for the separate circulation, deadline, approval, and publication fields, and the
[dated transition clarification](meetings/README.md#transition-clarification-2026-10-13)
for the proposed effective-date rule and treatment of existing records. The coordinated
canonical governance amendment must take effect before this process replaces the prior rule.

## Historical bootstrap context

This repository was bootstrapped following the July 26, 2026 committee decision on
ADR 0022; its implementing [lq-ai PR #311](https://github.com/LegalQuants/lq-ai/pull/311)
merged on July 27. The August 2 README described the canonical files as Proposed;
[GOVERNANCE.md](https://github.com/LegalQuants/lq-ai/blob/main/GOVERNANCE.md) and
[ADR 0022](https://github.com/LegalQuants/lq-ai/blob/main/docs/adr/0022-committee-governance-and-meeting-records.md)
now record adoption and acceptance (checked October 13, 2026).
The [August 9 decision log](decisions/README.md) records approval and merge of
[PR #313](https://github.com/LegalQuants/lq-ai/pull/313), superseding the earlier open status.
Canonical artifacts control their own status.

The initial repository push posted the bootstrap records on August 2, 2026, with an
August 9 objection deadline. Later records used merge as the posting event under the
previous process. These historical dates remain unchanged by the transition.

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
