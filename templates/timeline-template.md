# Documentation timeline template

Use this template to define your organization's documentation timeline structure, establishing milestones and dependencies from initial planning through publication.

**How to use this template:**

- Replace the example content with your organization's specific milestones, timelines, and criteria
- Adjust complexity levels and lead times based on your team's capacity and documentation requirements
- Customize milestone names and dependencies to match your development process
- For detailed guidance on timeline concepts, refer to the [documentation timeline framework](../docs/timeline.md)
- For a complete example demonstrating these concepts, see the [sample timeline](../examples/sample-timeline.md)

---

## Timeline diagram

This diagram illustrates the key milestones and their temporal relationships throughout the documentation lifecycle. Customize this to reflect your organization's specific milestones and timing.

```
Planning period starts
│
├─ Week 1: Parent initiative created
│           Documentation request created
│           Documentation plan completed
│           Writer assigned
│
├─ Week 2-10: Development phase
│              (Adjust duration based on typical project length)
│
├─ Code complete - 2 weeks: Notification to docs team
│                            (Advance notice allows writer planning)
│
├─ Code complete
│
├─ Launch - Lead time: Reviewable draft due
│  │
│  │  Low complexity:    Launch - 1 week
│  │  Medium complexity: Launch - 2 weeks
│  │  High complexity:   Launch - 4 weeks
│  │
│  └─ Writer review period
│
├─ Launch - 2 weeks: Documentation cut-off
│  │                 (No new changes accepted after this point)
│  │
│  └─ Final changes window closes
│
└─ Launch
```

## Milestone descriptions

Define each milestone in your timeline, explaining its purpose, deliverables, and dependencies. The milestones below represent a typical documentation lifecycle - customize them to match your organization's process.

### Planning period starts (Week 0)

The planning period begins when the product team starts defining the scope and timeline for the upcoming work. This marks the beginning of the documentation process and triggers the creation of the parent initiative.

**Key activities:** Initial scope definition, stakeholder identification, timeline estimation

**Deliverables:** High-level project brief or initiative outline

**Dependencies:** Product strategy or roadmap commitment

### Week 1: Initial setup

Four critical activities happen in the first week to establish the documentation foundation. Completing these activities early ensures writers have sufficient context and lead time.

**Parent initiative created.** Product manager creates the parent initiative in the project tracker, providing overall project context and timeline.

**Documentation request created.** Product manager creates the documentation request as a child of the parent initiative, formally requesting documentation support.

**Documentation plan completed.** Product manager fills out the documentation plan template with all required information, including feature summary, scope, and complexity estimate.

**Writer assigned.** Documentation lead assigns a writer to the project based on the completed plan, considering writer expertise and workload.

**Dependencies:** Approved project scope, available documentation resources

### Week 2-10: Development phase

The team builds the feature while the writer monitors progress and stays informed about changes. The writer may conduct early research, review design documents, and establish relationships with engineering stakeholders.

**Key activities:** Code development, design refinement, writer monitoring

**Writer responsibilities:** Track scope changes, review technical specifications, prepare documentation structure

**Dependencies:** Development resources, technical specifications

### Notification to docs team (Week 8, Code complete - 2 weeks)

Two weeks before code complete, the product manager notifies the docs team of the upcoming code complete date. This advance notice allows the writer to plan their review work and prepare for draft delivery.

**Key activities:** Confirm code complete date, verify feature scope stability, coordinate reviewer availability

**Required information:** Expected code complete date, any scope changes, testing environment access

**Dependencies:** Development progress visibility, stable feature scope

### Code complete (Week 10)

The feature implementation is complete and ready for testing. Code may still change during the review period based on testing feedback, but major functionality is in place and APIs are stable.

**Definition of "code complete":** All planned functionality implemented, feature available in testing environment, APIs and interfaces finalized

**Allowable changes after this point:** Bug fixes, minor refinements, test-driven adjustments

**Not allowed after this point:** New features, API changes, major refactoring

**Dependencies:** Completed development work, available testing environment

### Reviewable draft due (Week 10, Launch - 2 weeks)

The engineer or product manager provides a reviewable draft to the writer. Lead time varies based on complexity - this medium-complexity example requires a draft two weeks before launch.

**Draft quality expectations:** Technically accurate, includes all configuration options and examples, covers primary use cases

**Acceptable omissions:** Polish and formatting, comprehensive edge cases, final screenshots

**Writer responsibilities:** Review for technical accuracy, identify gaps, provide feedback, begin editing

**Dependencies:** Code stability, testing environment access, SME availability for questions

### Documentation cut-off (Week 10, Launch - 2 weeks)

Two weeks before launch, the documentation enters final preparation. No new changes are accepted except for critical corrections (security issues, breaking bugs, legal requirements).

**Rationale:** Final preparation requires stable content for editing, production, translation, and quality assurance

**Change criteria after cut-off:** Critical security issues, breaking functionality, legal or compliance requirements

**Escalation process:** Changes after cut-off require documentation lead approval with written justification

**Dependencies:** Completed draft review, stable code

### Launch (Week 12)

The feature ships and documentation publishes simultaneously, ensuring users have access to accurate information when they begin using the feature.

**Publication checklist:** Content reviewed and approved, production formatting applied, links verified, search indexing updated

**Coordination required:** Align with product launch timing, coordinate with marketing announcements

**Dependencies:** Completed documentation, approved launch readiness

## Timeline variations

Document how your timeline adapts to different project circumstances. This guidance helps teams make informed decisions when standard timing is not feasible.

### Complexity-based variations

Documentation lead time varies based on scope and complexity. Define your complexity criteria and corresponding lead times.

**Low complexity examples:** Single configuration option added, minor UI change, small API endpoint

**Low complexity lead time:** Launch - 1 week for reviewable draft

**Medium complexity examples:** New feature with 2-3 components, multi-step configuration, several related API endpoints

**Medium complexity lead time:** Launch - 2 weeks for reviewable draft

**High complexity examples:** Major architectural change, new product area, extensive API surface, multiple user types

**High complexity lead time:** Launch - 4 weeks for reviewable draft

**Rationale for lead times:** Low complexity requires basic review only. Medium complexity needs iteration on structure and examples. High complexity demands multiple review rounds and comprehensive testing.

### Compressed planning timelines

When planning starts late or schedules compress, teams must evaluate tradeoffs to maintain documentation quality.

**If planning starts in week 3 instead of week 1:**

Writer assignment delays until week 4, reducing total documentation time by 3 weeks. Options:

- **Extend launch date:** Add 3 weeks to maintain quality and review time
- **Reduce scope:** Limit documentation to essential content only (quick start, critical configuration)
- **Accept risk:** Proceed with compressed timeline, acknowledging potential quality issues or post-launch updates

**Decision criteria:** Customer impact of missing or incomplete documentation, competitive pressure for launch date, availability of post-launch documentation resources

### Extended development timelines

For longer projects spanning quarters or half-years, some milestones may be deferred to avoid premature assignment and context loss.

**Projects longer than 12 weeks:**

- Planning and documentation request creation remain at week 1
- Writer assignment may be deferred to 8-10 weeks before expected code complete
- Writer conducts mid-project check-ins to track scope changes

**Projects spanning multiple quarters:**

- Treat each major phase as a separate documentation cycle
- Writer assignment occurs for each phase individually
- Maintain continuity through documentation lead oversight

### Phased feature delivery

Features shipping in multiple phases follow the timeline multiple times, with each phase treated as a separate documentation project.

**Phase 1:** Complete full timeline for initial release, establishing foundational documentation

**Subsequent phases:** May use abbreviated timelines focusing on delta documentation (what changed, new capabilities)

**Documentation strategy:** Decide whether to version documentation separately for each phase or maintain single current version

## Customization guidance

Adapt this template to your organization's specific needs by considering these factors:

### Development cycle alignment

Align documentation milestones with your development methodology:

- **Agile/Sprint-based:** Milestones may align with sprint boundaries; adjust week numbers to sprint numbers
- **Waterfall:** Milestones align with development phases (requirements, design, implementation, testing)
- **Continuous delivery:** Establish rolling timeline with fixed lead times rather than specific weeks

### Team capacity and constraints

Consider your documentation team's capacity:

- **Small team:** May need longer lead times or more selective project acceptance
- **Distributed team:** May require additional coordination time or asynchronous review periods
- **Specialized team:** May assign writers based on domain expertise rather than availability

### Publication infrastructure

Account for your publication process requirements:

- **Translation required:** Add translation lead time before cut-off
- **Editorial review:** Add editorial review period between draft and cut-off
- **Multi-channel publication:** Coordinate timing across web, in-app, PDF, and other formats

### Product release model

Adapt to your release cadence:

- **Fixed release trains:** Documentation cut-off aligns with code freeze
- **On-demand releases:** Documentation timeline triggers from individual feature completion
- **Continuous deployment:** Documentation publishes independently, may precede or follow code

## Related documents

- **[Documentation timeline framework](../docs/timeline.md)** provides detailed guidance on timeline concepts and implementation
- **[Sample timeline](../examples/sample-timeline.md)** demonstrates a complete timeline for a medium-complexity feature
- **[Documentation plan template](../templates/documentation-plan.md)** defines the information needed to initiate documentation work
- **[Complexity framework](../docs/complexity-framework.md)** helps assess documentation complexity for lead time estimation
