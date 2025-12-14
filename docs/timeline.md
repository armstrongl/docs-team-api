# Documentation timeline framework

A documentation timeline defines the sequence of milestones from initial planning through publication, establishing when documentation work begins, when drafts are due, and when changes must stop. The timeline creates shared expectations between product teams and docs teams about delivery dates and quality gates.

## Why timelines matter

Documentation timelines serve three critical purposes:

**Predictability.** Teams know when documentation work will happen and when deliverables are due. This enables better resource planning and reduces last-minute scrambles.

**Quality assurance.** Fixed milestones create time for proper review, editing, and production work. Without clear cut-off dates, documentation quality degrades under pressure from ongoing changes.

**Dependency management.** Documentation depends on code stability, design decisions, and product direction. The timeline makes these dependencies explicit and ensures upstream work completes before downstream work begins.

## Core timeline components

### Milestone definition

A documentation timeline consists of key milestones that mark critical transition points in the documentation lifecycle. Each milestone represents either a deliverable or a decision point that enables subsequent work.

Common milestones include:

- **Planning initiation.** When the product team begins defining scope and timeline for the work.
- **Writer assignment.** When a specific writer takes responsibility for the documentation.
- **Code stabilization notification.** When product teams alert docs teams that code is approaching completion.
- **Draft delivery.** When the initial documentation draft becomes available for review.
- **Documentation cut-off.** When the documentation enters final preparation and stops accepting changes.
- **Publication.** When the documentation ships alongside the feature or product.

### Dependency mapping

Milestones have dependencies that constrain their timing. The timeline makes these dependencies explicit:

- Writer assignment typically depends on a completed documentation plan
- Draft delivery depends on code stability
- Cut-off date depends on publication requirements (editing, translation, production)
- Publication depends on feature launch or release

Understanding dependencies helps teams identify which milestones can flex and which are fixed. For example, publication date is often fixed by business requirements, making the cut-off date fixed as well.

### Complexity-based variations

Documentation lead time varies based on the scope and complexity of the work. More complex documentation requires longer review periods between draft delivery and cut-off.

Define complexity criteria relevant to your documentation type:

- **Low complexity.** Might require 1 week of review time
- **Medium complexity.** Might require 2 weeks of review time
- **High complexity.** Might require 4+ weeks of review time

The timeline should specify how complexity affects milestone timing, particularly the relationship between draft delivery, cut-off, and publication.

### Timeline flexibility

While some milestones are fixed (typically publication and cut-off), others can adapt to project circumstances:

**Compressed timelines.** When planning starts late or schedules accelerate, teams must decide whether to:

- Extend the publication date to maintain quality
- Reduce documentation scope
- Accept higher risk in the documentation process

**Extended timelines.** For longer projects (quarters or half-years), some milestones may be deferred. For example, writer assignment might happen when active development begins rather than at initial planning.

**Phased delivery.** Features that ship in multiple phases may follow the timeline multiple times, with each phase treated as a separate documentation project.

## Creating your documentation timeline

### Define your milestones

Identify the critical transition points in your documentation process. Start with these questions:

- When does documentation work begin?
- What deliverables must the product team provide?
- What deliverables must the docs team provide?
- When must changes stop to allow final preparation?
- When does documentation publish?

### Establish dependencies

For each milestone, identify what must happen before it can occur. Document these dependencies explicitly so teams understand the constraints.

### Set complexity criteria

Define what makes documentation "complex" in your context. Consider factors like:

- Amount of new content required
- Number of product areas affected
- Technical depth or novelty
- Number of user types or use cases
- Integration with existing documentation

### Determine lead times

Based on your complexity criteria, establish how much time is needed between milestones. Consider:

- Review and revision cycles
- Editing and production requirements
- Translation or localization needs
- Publication infrastructure constraints

### Document variations

Describe how the timeline adapts to different project circumstances. This helps teams make informed decisions when standard timing isn't possible.

## Related concepts

- **[Complexity framework](complexity-framework.md)** provides a systematic approach to assessing documentation complexity
- **[Documentation plan](documentation-plan.md)** defines the information needed to initiate documentation work
- **[Writer assignment](writer-assignment.md)** explains how writers are matched to projects based on plans and complexity
- **[Change management](last-minute-changes.md)** describes how to handle urgent changes after cut-off

## Example

See [Sample timeline](../examples/sample-timeline.md) for a complete example demonstrating these concepts.
