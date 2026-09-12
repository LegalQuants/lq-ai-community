# LQAI Committee — Weekly Call (2026-08-23)

*Public meeting notes. Discussion and action items are summarized without naming or attributing individual speakers or owners.*

| | |
|---|---|
| **Date** | 2026-08-23; time and time zone not recorded in source notes |
| **Platform** | Zoom (standing platform) |
| **Facilitator** | Not recorded in source notes |
| **Minutes** | Joel Kaufmann |
| **Attendees** | Artur, Hou Fu, Joel Kaufmann, Peter Scripps |
| **Attendee-list publication review** | Hou Fu reviewed the circulated notes on 2026-08-23 with “Looks good”; Joel Kaufmann authorized publication on 2026-09-11 |
| **Regrets** | Not recorded in source notes |

## Decisions

1. **Delay the planned v0.7.1 release by one week** to include a pending web UI dependency update. These minutes are the canonical operational record of the scheduling decision; this is not a statement of the eventual release date.
2. **Accept removal of the unused upstream Docling integration; defer pluggable ingestion as DE-387.** Canonical record: [ADR 0026](https://github.com/LegalQuants/lq-ai/blob/main/docs/adr/0026-document-ingestion-parser-and-docling.md), which records committee acceptance on 2026-08-23; [PR #528](https://github.com/LegalQuants/lq-ai/pull/528) merged on 2026-08-26. The ADR decision and subsequent implementation are separate events.
3. **Use a survey rather than a binding ballot** to gather community input on 1.0. These minutes are the canonical operational record of this framing decision. No final 1.0 scope or roadmap decision was made at this call.

## Discussion summary

### Key Outcomes

The committee focused on three themes: launching a community survey to shape the LQAI 1.0 roadmap, debating whether 1.0 should carry a marquee feature, and a broader strategic discussion of enterprise adoption, open-source sustainability, and agentic capability as a differentiator. No final roadmap decisions were locked. The survey will be refined and distributed within days, with a first tally expected at the next call and the resulting direction confirmed the following week.

The call recorded a one-week delay of the planned 0.7.1 release and acceptance of the Docling-removal decision, and noted the prior closure of an out-of-scope integration proposal. A licensing risk affecting enterprise deployments was flagged for further research.

### Agenda

1. Community survey for the 1.0 roadmap
2. Release status and scope decisions
3. Enterprise adoption and open-source sustainability
4. Agentic capability as a differentiator
5. Open questions and action items

### Other status and issues recorded

- The Clio/Filevine practice-management integration proposal was reported closed as out of scope, with future contributions welcomed if appropriately scoped. [PR #530](https://github.com/LegalQuants/lq-ai/pull/530) was closed without merge on 2026-08-22; this records a status discussed at the call, not a new closure on August 23.
- The discussion flagged PyMuPDF licensing as a potential enterprise-adoption concern for further research; no legal conclusion or replacement-parser selection was made.

### 1.0 Roadmap and Community Survey

- The working target for 1.0 is the **end of Q1 2027**, with the primary constraint identified as a single reviewer/merger bottleneck.
- The survey is organized around three key questions:
  1. **What is 1.0?** — proposed as an operator-trust milestone rather than a marquee-feature release.
  2. **API use case** — proposed as acknowledged but unsupported, to avoid added documentation complexity.
  3. **Marquee/headline features** — the timeline and scope for candidate capabilities (e.g., work ingestion, jurisdiction packs, meta-memory, multi-user, voice).
- A downstream fork with a working **Docling** integration was discussed; the committee intends to contact its author about upstreaming useful components. ADR 0026 records the distinction between the unused upstream integration and that working downstream implementation.
- On sequencing, the survey tally will receive a first update at the next call, with direction confirmed the following week.

### Enterprise Adoption and Sustainability

- A core adoption problem was identified: large organizations default to named or backed vendors, and an open-source, community-driven project can trigger automatic distrust regardless of capability.
- The discussion included an example of an enterprise team choosing an internally supported approach over adopting the upstream project, illustrating the importance of organizational backing and support.
- A **two-track model** was proposed: maintain a measured open-source upstream while pursuing a separate commercial/sponsorship track (for example, a major technology partner, an educational institution, or a Red Hat–style in-house consortium).
- It was suggested that academic affiliation — for example, positioning LQAI within a computational law research center — could serve as a credibility signal.
- A separate showcase-fork concept was revisited as a possible demonstration vehicle, though it was acknowledged as potentially confusing alongside the main project.

### Agentic Capability as a Differentiator

- The discussion identified a true agentic harness, beyond fixed workflow automation, as a potential differentiator for enterprise legal use. This was a strategic view expressed at the meeting, not a verified survey of competing products.
- A demonstrated fork illustrated several capabilities: practice-area agents (commercial, privacy, employment), skill/playbook attachment, three-layer context injection (house brief → agent brief → matter memory), and a human-correction memory tab.
- A **knowledge graph** (nodes and edges for entities, contracts, and directors) was identified as a potential marquee capability that could reduce manual context assembly. Comparative claims about commercial products were not independently verified.
- A **human-in-the-loop interface** (an agent inbox supporting accept/reject/comment) was highlighted as a compelling showcase feature.
- An open-source agent-to-agent communication platform was referenced as a potential integration point; no integration decision was made.
- Building the agentic layer properly was estimated at roughly one month of sustained, focused work, with significant UI refactoring required; one demonstrated approach replaced the existing web UI framework with a component-based stack.

### Open Questions

- Whether 1.0 should include a marquee feature and, if so, which one given resource constraints.
- How to address the document-parsing (PyMuPDF AGPL) licensing question for enterprise deployments.
- Whether to pursue a business/sponsorship track, and who would lead outreach — some members were noted as having relevant networks.
- How to make the survey accessible to non-technical members — for example, by adding short explainers or enabling AI-assisted reading.

## Action items

*Action ownership is maintained in the internal record.*

- [ ] Update the Docling Architecture Decision Record and refine the survey (adding explainers for non-technical members); distribute it to the community channels.
- [ ] Contact the downstream fork author about upstreaming Docling and other useful components.
- [ ] Present the first survey tally at the next call.
- [ ] All members: complete the survey before the next call.

## Takeaway

The committee's central near-term question is how LQAI reaches 1.0 and whether that release should be defined by operator trust or by a marquee capability. The community survey is the mechanism chosen to resolve that question with broader input. In parallel, the strategic discussion underscored that credibility with enterprise adopters — through a recognizable backer, academic affiliation, or a differentiated agentic harness — may matter as much as raw capability to real-world adoption.

## Record notes

- **Terminology:** the circulated draft used “docking.” This public record uses **Docling**, reconciled against ADR 0026 and PR #528.
- **Review follow-up:** the reviewer asked which alternative to PyMuPDF had been mentioned. The alternative's name was not recorded in the available meeting notes or resolved in that review thread; no selection is implied here.
- **Scope:** this records the August 23 discussion. Later roadmap changes belong in later meeting records. Canonical-artifact status above was checked on 2026-09-11.

## Ratification

- **Posted (merged):** 2026-09-11
- **Objection window closes:** 2026-09-18 (posted + 7 days)
- **Attendee-list publication review:** Hou Fu reviewed the circulated notes on 2026-08-23; Joel Kaufmann authorized publication on 2026-09-11.
- **Status:** Open for objections through 2026-09-18.

Corrections after posting are added as dated entries; the seven-day public objection window runs from posting, not from the meeting or the earlier Slack review.
