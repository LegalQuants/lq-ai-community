# LQAI Committee — Weekly Call (2026-10-25)

**PUBLIC VERSION — approved for publication.**

*Discussion and action items are summarized without identifying individual speakers or owners. Named ownership is maintained in the private record.*

| Field | Record |
|---|---|
| Date / platform | October 25, 2026 / Zoom |
| Time zone | Pacific (GMT−7), per Zoom meeting metadata (7:00 AM start; call ran approximately 39 minutes) |
| Attendees | Houfu Ang, Joel Kaufmann, Julian Bryant |
| Facilitator | Not recorded in source notes |
| Minutes-taker | Not recorded in source notes |
| Regrets | Not recorded in source notes |
| Attendee-list and content publication approval | Attendee list and public notes confirmed by Houfu Ang and Julian Bryant; no objections by the deadline; approval recorded 2026-11-01, confirmed by Joel Kaufmann. |

## Key Outcomes

This is release week for version 0.9.1. The remaining work is in three broad areas; the documentation site is expected to be finalized with closing commits the evening of the call, and the release may be brought forward from the usual 30–31 October timing because most of the planned work is already done. A documentation page on unsupported headless boot ([lq-ai PR #734](https://github.com/LegalQuants/lq-ai/pull/734)) has two reviewer suggestions outstanding; they will be applied and the PR resubmitted. An outside contributor is also reviewing; if that review is not received promptly the PR may move to the following release.

The main item was a presentation of a proposed redesign of the LQAI application interface: a move from top-tab navigation to a left-to-right workspace layout (navigation sidebar, chat in the centre, metadata panel on the right), a reduced black-and-white palette with colour reserved for governance, trust/privacy, and error states, outline rather than full-colour icons, and a reorganisation of several features (a "Labs" area for experimental features, a "Customize" area for skills, knowledge, and saved prompts, and the removal of a prompt-enhancement button and a save-skill-work screen). The redesign was received as a substantial improvement in professionalism and usability. Feedback centred on the use of colour (governance and error colours are too close; colour should not be abandoned entirely) and on the tension between resembling established legal-tech products and expressing a distinct, welcoming identity for an open-source project.

The committee agreed to proceed on the presented design as the working base, to circulate the full presentation (roughly fifty screens) to the wider community for comment, and to take the design through the ADR process before implementation. Implementation is expected to take about two months or longer, with much of it landing in December and January.

Because of the United States daylight-saving change, the standing call will keep its Pacific time, which moves it one hour later for attendees in regions that do not observe the change; this was accepted at least for next week's call, with the arrangement to be revisited when daylight saving resumes in spring.

## Decisions and Agreed Follow-Ups

No formal vote tally was recorded. Agreed directions:

- Proceed with the version 0.9.1 release this week, possibly ahead of the usual 30–31 October timing, once the documentation-site work is complete.
- Adopt the presented interface redesign as the working base for further development, while remaining open to alternative proposals; share the full presentation with the wider community for comment; then proceed through the ADR process before implementation. No ADR was adopted at this call and these minutes do not authorize implementation.
- Keep the standing call at its current Pacific time through the United States daylight-saving change (one hour later for attendees in non-observing regions), at least for next week's call; revisit when daylight saving resumes in spring.

These minutes are the canonical operational record for these items. Design decisions arising from the redesign will be canonical in their forthcoming ADRs.

## Release 0.9.1 and Documentation Site

The 0.9.1 milestone has three broad remaining areas. The documentation site is close to complete after a further round of pointers from a community reviewer and additional checks; closing commits were planned for the evening of the call, after which the site will be left to run. Progress on the next milestone was also noted. A plan was mentioned to publish a "diary"-style write-up telling the story of how community members have contributed to the project.

The documentation site currently uses a black-and-white palette, replacing the earlier design's orange, green, and yellow and the current application's green and white. Opinions were invited. One view was that any palette is acceptable and that having a helpful documentation site is what matters; a question was raised about the reasoning behind the choice, which led into the redesign presentation.

For [lq-ai PR #734](https://github.com/LegalQuants/lq-ai/pull/734) (documentation of unsupported headless boot), two reviewer suggestions can be applied directly in GitHub and committed, and it was agreed that this would be done. An outside contributor is also reviewing; a reminder will be sent if no response is received within one to two days.

## Interface Redesign Presentation

**Rationale.** The redesign reduces the number of colours so the application looks more professional and less like a generic web page, aiming at the look of current legal-tech applications and of Claude. This responds to earlier feedback about the colourful icons and to the concern that the previous look was not something a large in-house legal team would adopt. Icons move from full colour to outline style. The only colour retained is for governance (a lock icon, described on the call as red and later as orange), trust and privacy, and errors. Light and dark variants were shown.

**Layout.** Navigation changes from top tabs to a left-to-right workspace: a sidebar (Home, Tabular, Labs, Customize), the chat conversation in the centre, and a metadata panel on the right showing files, knowledge, and similar context. In the current interface, model, skills, and saved prompts sit beneath the chat box, which grows as more are attached; the message area is a small part of the screen and was described as getting in the way of work. The proposed layout was judged more space-efficient and simpler, with fewer things to click and therefore easier to engage with.

**Other elements presented.** Fewer words and clearer lists on the welcome screen, which may later be superseded by the Today View contemplated in the workspace-events ADR discussed at the previous call (see the [2026-10-18 record](../2026-10-18-weekly/notes.md)). Tabular output shown as tables rather than web-page-style text ("show the work, not a summary"). A read-only skill viewer rather than an editor, since editing skills is not something the application handles well at present. A "Customize" area (a term borrowed from Claude) housing skills, knowledge, and saved prompts. The "Autonomous" tab, whose purpose was unclear, becomes "Labs": a list of experimental features that can be switched on individually (automations, new harnesses, community skills), each with its own page and switch, offering a place to try new work before it is proven. A larger admin page with its own navigation. Use of the system typeface instead of Inter. The "playbook, not legal advice" notice is removed (the transcript is unclear whether it is retained under the playbook itself; to be confirmed). Two features are cut: the prompt-enhancement button (current models follow instructions well enough that prompt rewriting is not needed) and the save-skill-work screen (per-run notes used to evaluate skills), which is expected to get a more formal, dedicated space when the open-source LQ skills work is done.

**Status.** The screens are static mock-ups, not wired to working code. Implementation is expected to take about two months or longer, similar to the documentation-site effort; much of it may be visible in December and January. The full presentation of roughly fifty screens will be shared in the main community chat group for comment.

**Process.** The redesign was produced by directing Claude (Opus 5.5): pointing it at the LQAI repository, supplying existing feedback and the target direction, and asking it to study Mike OSS (an open-source legal AI platform) and Harvey for differences to move toward; the model found reference material itself. Side-by-side renderings of current and proposed screens were generated for every key screen and then iterated (for example, reducing headers to keep a conversational chat feel). Most screenshots were produced in one to two days. It was observed that the tool's dedicated design mode behaves differently from its general chat mode for visual work, and that with strong references it produced a good result.

## Feedback and Open Questions

- The removal of the prompt-enhancement button was supported; the view was expressed that prompt improvement belongs with users rather than in the interface, even though some commercial products retain the feature.
- The professional look was judged a significant improvement that helps the product feel like a tool a large in-house team would adopt; the reorganisation of functionality was seen as more important than colour, which is comparatively easy to change.
- Governance (orange) and error (red) colours are too close in shade and could confuse users. The choice of orange for governance was not a conscious one. The palette includes an "info" colour that does not appear in the screenshots; this was acknowledged as a gap.
- It was suggested that the design should not run from colour altogether: colour can provide a welcoming feel and guidance, and need not be limited to errors.
- Concern was raised that the design now closely resembles generic chat applications (such as Open WebUI) and, while professional, lacks a welcoming or distinctive character. The group discussed the tension between looking like established competitors (to signal parity) and expressing what makes LQAI different, including its open-source nature; this remains open for exploration.
- It was noted that giving the assistant a named persona in a deployment can lend the interface character and make it more approachable; this was offered as one way to address the identity question.

## Meeting Time

The United States daylight-saving change next week moves the call one hour later for attendees in regions that do not observe it. The call will keep its Pacific time, unchanged for US attendees, at least for next week; when daylight saving resumes in spring the time will shift back accordingly. Coordinating the call across the world was noted to have worked well so far.

## Action Items

*IDs match the private record. Individual owners are not published. These are follow-ups, not verified completion.*

- [ ] **O25-01:** Make the final documentation-site commits (evening of the call).
- [x] **O25-02:** Apply the two reviewer suggestions on [lq-ai PR #734](https://github.com/LegalQuants/lq-ai/pull/734) and resubmit. (Completed 2026-10-25.)
- [ ] **O25-03:** Follow up if the outside contributor reviewing PR #734 has not responded within one to two days.
- [ ] **O25-04:** Share the redesign presentation (roughly fifty screens) in the main community chat group for comment.
- [ ] **O25-05:** Palette items noted for follow-up: distinguish governance from error colours; express the "info" colour; explore ways to make the interface more welcoming and distinctive while keeping it professional.
- [ ] **O25-06:** Introduce the redesign to the wider community, collect comments, and take the design through the ADR process.
- [ ] **O25-07:** Prepare the "diary" write-up of community contributions (timing not stated).
- [ ] **O25-08:** Hold next week's call at the unchanged Pacific time; revisit the arrangement when daylight saving resumes.
- [ ] **O25-09:** Circulate October 25 minutes (internal and public) to the group (standing process item).

## Review, approval, and publication

*This record was circulated while lq-ai [PR #721](https://github.com/LegalQuants/lq-ai/pull/721) remained open (still open at the 2026-11-01 check), so the prior public-posting rule formally applies under the [transition clarification](../README.md#transition-clarification-2026-10-13); the seven-day internal review was run in any event, consistent with the preceding record.*

- **Draft prepared:** October 25, 2026.
- **Internal circulation:** 2026-10-25, 09:08 (Pacific), LQAI Slack channel.
- **Objection deadline:** 2026-11-01, 09:08 Pacific Daylight Time as circulated (08:08 Pacific Standard Time after the 2026-11-01 clock change; circulation + 7 days).
- **Approval date:** 2026-11-01
- **Approval basis and confirmation:** No objections were raised by the deadline. Houfu Ang confirmed the notes on the circulation post; Julian Bryant confirmed in person. Confirmed by Joel Kaufmann.
- **Attendee-list publication review:** Confirmed by Houfu Ang and Julian Bryant; recorded by Joel Kaufmann on 2026-11-01.
- **GitHub publication (merged):** Pending merge
- **Objection-window close (prior rule):** Merge date + 7 days.
- **Status:** Approved for publication — open for public objections for seven days after merge.

These notes summarize the Zoom transcript of the call; statements about release timing, implementation estimates, and tooling reflect participants' reports and were not independently verified. Corrections after publication are added as dated entries.
