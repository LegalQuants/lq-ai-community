# LQ.AI Committee — Weekly call — 2026-08-16

*Public meeting notes. Discussion and action items are summarized without naming or attributing individual speakers or owners, per the committee's notes process.*

| | |
|---|---|
| **Date** | 2026-08-16; time and time zone not recorded in source notes |
| **Platform** | Zoom (standing platform) |
| **Facilitator** | Not recorded in source notes |
| **Minutes** | Joel Kaufmann |
| **Attendees** | Alexios, Emily, Ang Houfu, Joel Kaufmann, Julian, Peter Scripps |
| **Attendee-list approval** | Confirmed by Joel Kaufmann (minutes-taker) |
| **Regrets** | Not recorded in source notes |

## Decisions

<!-- Canonical text of each architectural/product decision lives in lq-ai (ADR/PR/issue).
     A matching row for each decision is added to ../../decisions/README.md in the same commit. -->

1. **Document-ingestion dependency: decision deferred.** The alternatives — completing the intended integration, replacing or removing the dependency, or adopting a pluggable document-ingestion layer — will be framed in an ADR for group review at the next meeting. *These minutes are the canonical operational record for this deferral; the eventual decision will have its own ADR.*

## Discussion summary

### Key Outcomes

The committee examined a foundational question about LQAI's direction: whether it should primarily be a polished, ready-to-use product, a modular toolkit that practitioners and developers tailor to particular needs, or a combination of both. No final product-versus-platform choice was made. The discussion converged on several immediate priorities: enable real-world deployments, collect direct user feedback, clarify near-term milestones, and use evidence from actual practice to guide feature priorities.

The committee also reviewed contributor incentives, downstream forks, the inherited roadmap, the documentation-site product requirements document (PRD), and a reported issue involving an unused document-ingestion dependency that materially increases the deployment footprint. A decision on that dependency was deferred pending a formal Architecture Decision Record (ADR).

### Agenda

1. Project identity and target users
2. Contributor engagement and incentives
3. End-user discovery and feedback loops
4. Downstream forks and contribution routing
5. Backlog and roadmap priorities
6. Documentation-site PRD
7. Document-ingestion dependency

### Project Identity and Direction

- The project continues to face a **product-versus-platform** tension. One model emphasizes a polished experience that delivers immediate value to a specific end user; another emphasizes high-quality infrastructure that practitioners and developers can tailor for different clients and workflows.
- A combined model may be possible: a polished default deployment for new users, supported by a modular foundation that advanced users can simplify or customize.
- The current ambiguity affects participation. Potential contributors may not know who the primary user is, what the project is ultimately trying to deliver, how priorities are set, or where their work would fit.
- The documentation-site process is expected to help make the project's purpose, target users, and first-use experience more explicit.

### Contributor Engagement and Incentives

- The discussion identified a **negative contribution loop**: unclear scope discourages contribution; the backlog and review burden then grow; and the lack of visible releases further reduces momentum.
- Because the project is voluntary, sustainable participation depends on clear intake and review paths, manageable commitments, and value for contributors. The discussion included the possibility that implementation and customization services could create an economic incentive around an open toolkit.
- Lightweight operating structure — visible priorities, regular notes, short feedback cycles, and a dependable contribution cadence — could improve momentum without over-formalizing the community.
- The discussion noted that synchronous attendance may not fully measure engagement because participation also occurs through asynchronous discussion, one-to-one conversations, code, and downstream deployments across different time zones and work schedules.
- Tailored applications do not always flow back upstream because preparing a narrowly focused solution for general use can slow delivery and require substantial additional work.

### End Users and Feedback Loops

- The project's potential users include both practitioners completing legal work and technically capable practitioners or developers who build customized deployments on top of LQAI.
- Real-world use may remain invisible to the core project when deployments do not produce issues, pull requests, or structured feedback.
- Forks and issue reports provide useful signals, but the discussion emphasized the greater value of direct user feedback.
- The committee can support product discovery by bringing a range of practitioner and organizational perspectives into roadmap review.
- Feature priorities should be tested against demonstrated user needs so that technically impressive work does not outrun practical demand.

### Downstream Forks and Contribution Routing

- Downstream forks can contain substantial custom work that does not naturally return upstream.
- The project will review relevant downstream work and distinguish between features suited to the core codebase and capabilities better delivered through skills or extensions.
- These examples illustrate both the value of a modular platform and the friction involved in upstreaming tailored deployments.

### Backlog and Roadmap Priorities

- The existing pool of open pull requests may be useful as a backup backlog, but it should not automatically determine the priority queue.
- Limited contributor time should focus on work with meaningful value to the broader community rather than mechanically completing every deferred enhancement.
- The inherited roadmap is useful guidance, but it is not a binding sequence and does not itself define what constitutes a finished 1.0 release.
- Clearer next steps and a loose launch or milestone plan would give contributors a more understandable target while leaving room for evidence-driven changes.

### Documentation-Site PRD

- The documentation-site PRD is open for community review and refinement.
- Feedback grounded in contributors' actual difficulties, deployments, and user experiences is especially valuable at this stage.
- Four framing questions are guiding the work:
  - Why is LQ doing LQAI?
  - What is the alpha and frontier?
  - Why is this only now possible?
  - What is the "first-run aha" moment?

### Document-Ingestion Dependency

- The committee reviewed a reported issue in which the current stack declares a document-conversion dependency and downloads related machine-learning models, including models intended for PDF table detection.
- According to the discussion, the corresponding connector was never implemented, so the dependency is not currently called by the application. PDF uploads instead use a separate direct parsing path.
- The reported result is several gigabytes of additional deployment-image size without current functional value.
- Options discussed included completing the intended integration, replacing it with a newer document-ingestion approach, or making OCR and document conversion pluggable so operators can choose the service or model that fits their requirements.
- The discussion raised input completeness and extraction accuracy as foundational concerns: missing text at ingestion cannot be reliably recovered at later reasoning stages.
- **Decision deferred:** the alternatives will be framed in an ADR for group review at the next meeting (see Decisions above).

### Current Status

- **Product versus platform:** unresolved; a combined default-plus-modular model remains under consideration.
- **Near-term emphasis:** real deployments, direct feedback, clearer milestones, and evidence-based prioritization.
- **Inherited roadmap:** treated as guidance rather than a mandatory sequence.
- **Document-ingestion dependency:** no change approved; ADR review is pending.

## Action items

*Action ownership is maintained in the internal record; owners are not published, per the committee's anonymized-notes process.*

- [ ] Draft an ADR comparing whether to keep and integrate the current document-ingestion dependency, replace or remove it, or adopt a pluggable document-ingestion layer.
- [ ] Review relevant downstream work and identify candidates for the core codebase versus skills or extensions.
- [ ] Publish clearer near-term milestones and a rough launch plan.
- [ ] Develop a framework for structured contributor and end-user discovery.
- [ ] Gather community responses to the four documentation-site framing questions.
- [ ] Document lessons from real-world deployments, including local or offline use and customization where applicable.
- [ ] Review the inherited roadmap against practical user and organizational needs.
- [ ] Triage open pull requests according to broad contributor and user value.
- [ ] Maintain a regular cadence for public meeting notes and project updates.

## Takeaway

LQAI's central strategic question remains open: it can create value as a polished end-user experience, as adaptable infrastructure, or through a deliberate combination of the two. The immediate path does not require that question to be resolved in the abstract. Real deployments, direct user discovery, and transparent near-term priorities can generate the evidence needed to shape the project while also improving contributor momentum.

## Ratification

- **Posted (committed to main):** 2026-08-23
- **Objection window closes:** 2026-08-30 (posted + 7 days)
- **Attendee-list publication review:** Confirmed by Joel Kaufmann (minutes-taker)
- **Status:** Open for objections through 2026-08-30

<!-- Per GOVERNANCE.md (lq-ai PR #311): committee members who miss a call may register
     agreement or objection within 7 days of posting; silence after 7 days is assent.
     On window close, set Status to "Ratified (silence is assent)" or record the
     objection outcome. Posted minutes are append-only — corrections are added as
     dated "Correction (YYYY-MM-DD):" entries. -->
