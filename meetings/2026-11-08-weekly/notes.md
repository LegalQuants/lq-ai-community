# LQAI Committee — Weekly Call (2026-11-08)

**PUBLIC VERSION — approved for publication.**

*Discussion and action items are summarized without identifying individual speakers or owners. Named ownership is maintained in the private record.*

| Field | Record |
|---|---|
| Date / platform | November 8, 2026 / Zoom |
| Time zone | Pacific (GMT−8), per Zoom meeting metadata (7:00 AM start; call ran approximately 50 minutes) |
| Attendees | Houfu Ang, Joel Kaufmann, Julian Bryant |
| Facilitator | Not recorded in source notes |
| Minutes-taker | Not recorded in source notes |
| Regrets | Not recorded in source notes |
| Attendee-list and content publication approval | Attendee list and public notes confirmed by Houfu Ang at the 2026-11-15 call; Julian Bryant, also present, raised no correction or objection; approval by all attendees recorded 2026-11-15, confirmed by Joel Kaufmann. |

## Key Outcomes

Version 0.9.1 was released following the previous call, and a short pause in development was noted before activity picks up again. The main item was a second discussion of the change of direction first raised at the previous call: reorienting LQAI away from pursuing feature parity with established commercial legal-AI products and toward a "small core plus Labs" model, in which the project keeps its core infrastructure (the gateway and the skills architecture) and devotes development energy to a Labs or showcase area where LegalQuants members can present their own experiments and tools. The direction was supported, and the view was expressed that the ideas were more developed than when first raised. The discussion ranged over why the change is proposed, its consequences for deployment into firm or corporate environments, the risk that it makes LQAI's identity less clear, the difficulty of sustaining contributions to a shared open-source codebase in the era of AI coding agents, the project's relationship to the LegalQuants learning programmes, and how LQAI should coexist with general-purpose AI coding tools.

The near-term work plan has three prongs: the new interface (first visible changes targeted for November), bringing Labs into the interface the following month, and further work on a more open "harness" that combines skills and models. Document (`.docx`) ingestion will be opened to the community for a member to take up. The published minutes will be used to explain the direction change to the wider membership, and space is to be created for more people to contribute so the work does not rest on one person.

## Decisions and Agreed Follow-Ups

No formal vote tally was recorded. Agreed directions:

- Confirm the change of direction raised at the previous call: LQAI is reoriented toward a small core plus a Labs/showcase area for LegalQuants members' experiments and skills, rather than toward feature parity with established commercial legal-AI products. The gateway and skills architecture are retained as core; what else constitutes "core" remains to be determined. Deployment into firm or corporate environments becomes a lower priority, although the gateway and APIs remain available to anyone who wishes to use them. No ADR was adopted at this call.
- Adopt a three-prong work plan: the new interface first (first visible changes targeted for November); Labs brought into the interface the following month, including the automation features; and continued work on a more open harness, with updates as it progresses. Open the `.docx` ingestion work to the community for a member to take up.
- Use the published minutes to explain the new direction to the wider membership, and create space for more members to contribute so that the work is not carried by one person.

These minutes are the canonical operational record for these items. Design and architecture decisions arising from the interface and harness work will be canonical in their forthcoming ADRs.

## Project Update

Version 0.9.1 was released after the previous call. A short break was noted before work picks up again. A community member has taken more interest in the Word plug-in work; the resulting contributions will be reviewed and steered, with some caution noted given the discussion about keeping the core small. Work on the shell of the new interface is about to begin, with the aim of showing the first steps of the changed look this month before larger questions, such as how to move away from the current chat front end, are considered. Because the interface work has been prioritized, the `.docx` ingestion work will be offered to the community, along with other small changes, through the community chat group this week.

## Direction Change: Small Core and Labs

**Rationale.** For several months the project has concentrated on clearing pull requests and incremental improvements. A member's attempt to introduce LQAI into their own organization encountered two blockers: the interface was not adequate for real work, even after adjustment, and `.docx` ingestion was missing. Two responses were considered: push LQAI as hard as possible toward parity with the established commercial products (some of which already offer `.docx` ingestion), or modify the direction. Chasing parity was described as intellectually stimulating but not sustainable for a volunteer-maintained project, because it depends on repeatedly asking members to contribute tests and incremental fixes. The interface redesign and the Road to 1.0 milestone, by contrast, drew a good response, suggesting that large challenges and showcasing members' work are what engage the community.

**The Labs idea.** The Labs tab in the redesigned interface was originally conceived for automations and has since been extended with a new harness. The example given was using Jev, the Typesafe agent, to review as many NDAs as possible as cheaply as possible: an experiment that fits naturally into a Labs area but would be awkward to place on a product roadmap modelled on commercial tools. The focus is therefore not on a product that wins over users of those tools, but on a place where LegalQuants members can show what they are working on and what they are good at. Core infrastructure is retained; the group needs to determine what the core is and what is introduced as showcases or experiments.

**Deployment.** A question was raised whether another attempt to deploy LQAI in a firm or corporate environment is contemplated, for example in a few months' time. Under the new direction this becomes less of a priority. The gateway and APIs are good enough to support such use for anyone who wants to pursue it, but development mindshare and effort will be directed less toward asking practising lawyers what features would help with, for example, contract review.

**Identity concern.** Concern was raised that, while the showcase model may meet contributors' enthusiasm, it makes LQAI harder to describe to a prospective user: rather than solving a practical legal need for a defined target user, the software would do several disconnected things well according to where contributor enthusiasm happened to be. This was acknowledged as a fair point. It connects to the unresolved question of what "core" is; pressed hard, "core" tends to expand to everything currently being worked on, and the discussion did not resolve this with clarity. It was also noted that each change of direction makes the question "what is LQAI for?" murkier, and that the project has wanted to tie itself more closely to the residents' journey.

**What keeps the project going.** It was observed that LQAI is focused on some of the hardest questions in open-source legal technology, such as how to get more lawyers coding or contributing to something anyone can adopt, and that the project will probably have to coexist with many other tools, including general-purpose coding agents and their legal offerings.

## Contributor Engagement and Open-Source Sustainability

Most LegalQuants members do not know what LQAI is for; considerable introduction will be needed, drawing on the community's communications channels, and members who have done interesting work will likely need to be approached directly. The project will also need to bridge the gap between a member's experiment and how it is placed on LQAI.

The contribution structure of a comparable open-source legal-AI project was discussed. In that project most contributions come from one person with engineering help for review; it accepts many contributors, not all of them lawyers, who typically contribute a small piece and leave direction to the maintainer; it has high visibility on social media and a sponsorship but no revenue. LegalQuants members who contribute to LQAI are lawyers, while anonymous contributors elsewhere may be engineers or students.

A target set in January for having a second maintainer by this coming January was recalled; it now appears unlikely to be met. This was described as a check on how the project is progressing rather than a hard deadline, and as a challenge without a found solution: code is comparatively easy with AI agents, whereas securing a human being's sustained time and attention is different. The tension was acknowledged between members' own practices and contribution to LQAI; building tools for one's own practice is often the stronger incentive, and it is an open question how a collection of practising lawyers organizes itself to produce a substantial software product. Wikipedia was raised as an example of a successful volunteer project whose success is hard to account for.

A broader observation emerged: AI coding agents may have reduced the incentive to contribute to a large collective project, because it is now easier to spin up an agent to solve one's specific problem than to learn a codebase the size of LQAI, follow its contribution process, and integrate with its interface. This may mirror a wider question in software between large shared platforms and individuals building many small custom tools. If that is the probable outcome, the question becomes what LQAI should look like, and this is part of what draws the project toward the showcase and small-core idea rather than trying to beat a competitor. It was noted that this philosophical underpinning gives the showcase idea a new context.

## Relationship to the LegalQuants Learning Programmes

A question was raised whether there is a structured path within LegalQuants for someone who has completed a first project in the residency to gain experience building more sophisticated tools with others, in the manner of an accelerator or clinic. The LegalQuants programmes were outlined in response; it was noted on the call that some details may not yet be public and should be checked before publication, so they are not reproduced here. The hope was expressed that LQAI will serve as a proving ground connected to this pipeline, so that what residents build can flow into Labs or experiments, or even into the core. Residents who become members were described as enthusiastic ambassadors, with the caveat that the interest of existing members, not only graduating residents, must be maintained. It was also noted that the bones of the project remain useful for integrating LQAI into anyone's project, not only for contract review.

## Coexistence with General-Purpose AI Coding Tools

The current interface was described as somewhat cumbersome in practical use, and many of the planned interface changes correspond to issues identified in test runs. A tension was discussed between adopting a general-purpose AI assistant as the foundation of a legal practice and building bespoke applications for that practice. If a general-purpose assistant becomes the environment in which daily legal work happens, including client engagement, calendar, invoicing, and time management, then context-switching to a separate application to do legal work seems unlikely to be what lawyers will do, and bespoke applications might need to be deconstructed into skills or MCP components instead, which raises both philosophical and practical questions.

Surveys of LegalQuants members show that two general-purpose AI tools dominate what members actually use, and the view was expressed that the "lawyer's IDE" is likely to be much closer to a general-purpose coding agent than to a dedicated application. The question of how a bespoke application coexists with that is the same problem LQAI faces, and it was described as troubling. The response was that this is precisely what makes the Labs and showcase direction attractive: wherever the technology goes, there will be a need to experiment, test, and try things, probably through some combination of members' own applications and working directly in coding agents; a place to learn adds durability to the project, has been its most beneficial aspect, and is a more honest framing — not a clone of the commercial products, but a way to learn how they work, how to build one's own, and how to improve one's skills.

## Action Items

*IDs match the private record. Individual owners are not published. These are follow-ups, not verified completion.*

- [ ] **N08-01:** Begin work on the shell of the new interface; first visible changes targeted for November.
- [ ] **N08-02:** Bring Labs into the interface the following month, including the automation features.
- [ ] **N08-03:** Continue work on the harness so that it is more open (combining skills and models) and can accommodate members' projects in Labs; provide updates as it progresses.
- [ ] **N08-04:** Share the existing harness description (a GitHub issue, noted as outdated) in the community chat group; a more definite description is to follow.
- [ ] **N08-05:** Post the `.docx` ingestion work, with other small changes, in the community chat group this week to find a member to take it up.
- [ ] **N08-06:** Review the Word plug-in contributions from an interested community member and steer them appropriately.
- [ ] **N08-07:** Make the new direction known to the membership through the community's communications channels, and approach members who have done interesting work about contributing showcase experiments.
- [ ] **N08-08:** Use the minutes of this call to explain the direction change to the wider membership.
- [ ] **N08-09:** Confirm which details of the LegalQuants learning programmes may be shared publicly before they appear in published material.
- [ ] **N08-10:** Circulate November 8 minutes (internal and public) to the group (standing process item).

## Review, approval, and publication

*This record was circulated while lq-ai [PR #721](https://github.com/LegalQuants/lq-ai/pull/721) remained open (still open at the 2026-11-15 check), so the prior public-posting rule formally applies under the [transition clarification](../README.md#transition-clarification-2026-10-13). The seven-day internal review was opened in any event, consistent with the preceding records; unlike those records, this one was approved by its attendees and submitted for publication one day before the internal deadline, as set out below.*

- **Draft prepared:** November 8, 2026.
- **Internal circulation:** 2026-11-09, 09:33 (Pacific Standard Time), LQAI Slack channel (internal and public versions).
- **Objection deadline:** 2026-11-16, 09:33 (Pacific; circulation + 7 days).
- **Approval date:** 2026-11-15
- **Approval basis and confirmation:** The notes were taken up as the first agenda item at the 2026-11-15 call. Houfu Ang confirmed the notes; Julian Bryant, also present, raised no correction or objection. No objections had been raised on the circulation post as of 2026-11-15. Approval was recorded on that basis one day before the internal objection deadline, rather than by the no-objection process at its expiry; a later objection is handled under the correction process in the [meetings README](../README.md#review-and-publication-process). Approval by all attendees confirmed by Joel Kaufmann.
- **Attendee-list publication review:** Confirmed by Houfu Ang at the 2026-11-15 call; no objection from Julian Bryant; recorded by Joel Kaufmann on 2026-11-15.
- **GitHub publication (merged):** Pending merge
- **Objection-window close (prior rule):** Merge date + 7 days.
- **Status:** Approved for publication — open for public objections for seven days after merge.

These notes summarize the Zoom transcript of the call; statements about release status, contribution patterns in other projects, survey results, and timing reflect participants' reports and were not independently verified. Corrections after publication are added as dated entries.
