# LQAI Committee — Weekly Call (2026-11-01)

**PUBLIC VERSION — approved for publication.**

*Discussion and action items are summarized without identifying individual speakers or owners. Named ownership is maintained in the private record.*

| Field | Record |
|---|---|
| Date / platform | November 1, 2026 / Zoom |
| Time zone | Pacific (GMT−8; standard time resumed this day), per the transcript timestamps |
| Attendees | Houfu Ang, Joel Kaufmann, Emily Cabrera, Jamie Tso |
| Facilitator | Not recorded in source notes |
| Minutes-taker | Not recorded in source notes |
| Regrets | Not recorded in source notes |
| Attendee-list and content publication approval | Attendee list and public notes confirmed by Houfu Ang on the circulation post; no objections from Emily Cabrera or Jamie Tso by the deadline; approval recorded 2026-11-09, confirmed by Joel Kaufmann. |

## Key Outcomes

The call was deliberately short and run as an open conversation rather than against an agenda. Version 0.9.1 has been released; the release included a "feature parade" of short, automatically generated videos showcasing each contributor's feature. Pull-request volume has fallen from roughly 50–60 open PRs to the low twenties now that the review backlog has been cleared, and attention has shifted to three planning decks circulated in the community chat: a new agent harness, document ingestion, and an interface redesign. Sequencing and engineering decisions within those workstreams remain unresolved.

The main discussion concerned the strategic direction of the project. The group discussed whether continuing to pursue feature parity with established commercial and open-source legal AI products is realistic or motivating, given how quickly frontier capabilities move and the technical debt carried by the legacy codebase. An alternative framing was developed: reimagining LQAI as a "gateway" to LQ community projects — a Labs area where members can showcase agents, experiments, evaluations, and best practices — built on a small retained core that preserves some contract-review functionality. There was broad support for this direction, together with the view that LQAI's distinctive value lies in research-driven best practices and in serving as a training ground for contributors of all skill levels. A complementary proposal was to draw on learnings from the LQ Residency program, potentially through a task force of residency mentors researching best practices for the infrastructure-level problems LQAI needs to solve.

No decision was taken. The group agreed to pause after the 0.9.1 release, circulate the record of this call, and gather further comments from the wider committee before deciding on direction.

## Decisions and Agreed Follow-Ups

No formal decisions were recorded and no vote was taken. Agreed directions:

- Make no decision on project direction at this call; develop the "gateway" / Labs framing further and gather comments from the wider committee after the record of this call is circulated.
- Take a short pause after the 0.9.1 release to reflect on direction before committing to the sequencing of the new-harness, document-ingestion, and interface workstreams.
- Explore consolidating LQ Residency learnings into LQAI best practices, possibly through a task force among residency mentors; a proposal on the gateway concept may be developed offline for later discussion.
- Gather feedback on the 0.9.1 feature parade, and research what others in the legal AI space are experimenting with and where interest is likely to be over the coming months, to inform prioritization.

These minutes are the canonical operational record for the items above.

## Release 0.9.1 and Project Activity

Version 0.9.1 shipped with a feature parade: each accepted feature contribution was turned into a 30–60 second video crediting the contributor. The videos were produced by looping an AI coding agent over the contributions rather than by scripting each one by hand; generation took roughly two hours and a substantial number of tokens, which delayed the release slightly. Feedback was sought on whether the format is worth repeating. Not all attendees had yet reviewed the release or the videos; feedback was promised later the same day.

The drop in pull-request volume was described as a natural consequence of clearing the backlog, allowing focus to move to the longer-term goals captured in the three planning decks. The week was nonetheless described as difficult from a project-management standpoint, because the ideas in the decks are clear but many sequencing and engineering decisions behind them are not yet made.

## Project Direction: the "Gateway" and Labs Concept

Concern was raised that chasing established legal AI products — whether commercial or open-source — is neither motivating nor strategically sound: the frontier is moving too quickly, other open-source tools (including permissively licensed ones) are already well ahead, and upgrading the legacy codebase to that standard is a large amount of unrewarding work. It was also noted that evaluations have not been incorporated into LQAI because the product architecture is still bound to the original contract-review use case, which blocks broader experimentation.

In the course of the interface redesign, the Labs tab was identified as the part of the product with the most potential: a gateway through which members can see LQAI's components at work — for example, a dedicated page where Jev, the Typesafe (typesafe.ai) agent, runs through an NDA, with the code exposed and the results presented as a walkthrough. Under this framing each lab could design its own presentation layer (a chat interface, an evaluation display, or otherwise) on top of shared building blocks in a small core. The project's purpose would become showing what LQ members build and know, rather than replicating a general-purpose legal AI assistant. A member project could be ported into LQAI as a way for its author to demonstrate expertise. A previously proposed gateway design was referenced as still attractive, which is one reason a small core would be retained.

Support was expressed for building what the community is uniquely positioned to build and has the people to support, rather than catching up with other open-source projects. It was suggested that the historical roots of the project need not constrain it: learnings could be consolidated into documented best practices, a small core gateway could be built as an MVP to show how different projects bolt on, and a poll or proposal could follow. A European open-source legal tool with a built-in benchmarking tab was cited as a reference point; LQAI could similarly evaluate a method (for example, Jev-assisted NDA review versus unassisted review) to demonstrate why the approach matters. A recent licensing-policy change by a widely used open-source chat interface — requiring display of its logo above a user threshold — was cited as a reason to avoid deep dependency on external platforms.

The concept was also described as a "coding gym": a training ground where a contributor can attempt an ambitious project, such as a Word plug-in, or take on lighter tasks, with all skill levels encouraged. A recent third-party comparison was said to show that LQAI already offers a different perspective from the incumbent open-source alternative. It was observed that the existence of open-source tools resembling commercial legal AI assistants raises the question of whether such a tool is needed at all when members are able to build their own; the interfaces were still judged to have value, and what the project needs to be was described as an important and evolving question.

A question was raised about how evaluations can be presented in a way that non-specialists understand easily; this was acknowledged as an unresolved design challenge.

## Research-Driven Best Practices and Residency Integration

It was suggested that a clear roadmap directing contributions would ease the maintenance burden, and that the project should concentrate on what it can distill as best practices. Rather than copying architectural choices from existing open-source projects, LQAI could justify its choices through research — for example, for document ingestion, comparing the available open-source and commercial libraries, defining benchmarks, and publishing the findings as a community opinion that can be revisited and swapped as better components appear. This would give the project authority and distinguish it from purely user-focused alternatives. It was noted that a benchmarks conversation from a few weeks earlier had died down, and that experiments run on LQAI could generate benchmark-style content usable for external brand development.

A proposal was made to consolidate learnings from the LQ Residency and contribute them back to LQAI as best practices, forming a natural bridge between the programs: where several residents are solving the same infrastructure-level problem, the problem could be solved within LQAI first and new residents pointed to that resource. A task force within the residency mentor group could research best practices for specific problems and feed the resulting architectural choices into the codebase, so that the code becomes the embodiment of the group's research. Making support for the open-source project an expectation of residency mentors was also raised. It was noted that two attendees had independently arrived at the idea of tapping residency learnings, which was taken as validation of the direction. A separate commitment was made to research what others are experimenting with and where interest is heading over the coming months. Mentor capacity is limited in the current cohort.

## Interface, Core Scope, and Skills Ingestion

The forthcoming interface redesign was welcomed and expected to resolve many usability issues encountered in an earlier real-world trial. Drawing on that trial, the architecture was described as solid, but the system needs more of the community's skills and playbooks imported into it; a cold-start or ingestion process for LQAI, similar to the one used by the LQ plugins, was suggested. Continued collection of interface feedback was encouraged. What belongs in the small retained core, and what can be cut, was identified as an open question on which experience from real deployments would be valuable.

## Action Items

*IDs match the private record. Individual owners are not published. These are follow-ups, not verified completion.*

- [ ] **N01-01:** Review the 0.9.1 release and feature parade and send feedback (same day).
- [ ] **N01-02:** Research what others in the legal AI space are experimenting with and where interest is likely to be over the next few months, to inform LQAI priorities.
- [ ] **N01-03:** Consider how to consolidate LQ Residency learnings for LQAI, including forming a task force among residency mentors to research best practices for infrastructure-level components; develop a proposal on the gateway concept offline.
- [ ] **N01-04:** Pause after the 0.9.1 release to reflect on project direction and the gateway concept before committing to workstream sequencing.
- [ ] **N01-05:** Circulate the record of this call to the committee and gather comments on the proposed direction (all members).

## Review, approval, and publication

*This record was circulated while lq-ai [PR #721](https://github.com/LegalQuants/lq-ai/pull/721) remained open (still open at the 2026-11-09 check), so the prior public-posting rule formally applies under the [transition clarification](../README.md#transition-clarification-2026-10-13); the seven-day internal review was run in any event, consistent with the preceding records.*

- **Draft prepared:** November 1, 2026.
- **Internal circulation:** 2026-11-01, 09:21 (Pacific Standard Time), LQAI Slack channel (internal and public versions).
- **Objection deadline:** 2026-11-08, 09:21 (Pacific; circulation + 7 days).
- **Approval date:** 2026-11-09
- **Approval basis and confirmation:** No objections were raised by the deadline, and none were raised when the notes were revisited at the 2026-11-08 call. Houfu Ang confirmed the notes on the circulation post; Emily Cabrera and Jamie Tso raised no objections (no-objection process). Confirmed by Joel Kaufmann.
- **Attendee-list publication review:** Confirmed by Houfu Ang on the circulation post; no objection from Emily Cabrera or Jamie Tso by the deadline; recorded by Joel Kaufmann on 2026-11-09.
- **GitHub publication (merged):** Pending merge
- **Objection-window close (prior rule):** Merge date + 7 days.
- **Status:** Approved for publication — open for public objections for seven days after merge.

These notes summarize the Zoom transcript of the call; statements about release activity, contribution volume, third-party tools, and deployment experience reflect participants' reports and were not independently verified. Corrections after publication are added as dated entries.
