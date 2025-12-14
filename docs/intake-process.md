# Documentation intake process

An intake process defines how documentation requests enter your team's workflow and what constitutes a complete, actionable request. A well-designed intake process ensures that writers have the information they need to succeed, prevents last-minute surprises, and establishes clear accountability for documentation quality.

This document explains the core components of a documentation intake process and provides guidance on designing one that fits your team's needs.

## What is a documentation intake process?

A documentation intake process is a formalized system for managing how documentation work enters your team's queue. It establishes criteria for when documentation is needed, who is responsible for requesting it, what information must be provided, and how requests are prioritized and assigned.

Without a clear intake process, docs teams often face:

- Incomplete or missing information that delays work
- Last-minute requests that compromise quality
- Unclear accountability when documentation doesn't meet standards
- Difficulty prioritizing competing requests
- Inconsistent documentation coverage across products or features

A well-defined intake process addresses these challenges by establishing shared expectations between docs teams and the stakeholders who request documentation support.

## Why documentation intake processes matter

Documentation intake processes serve multiple purposes:

**For docs teams:**

- Ensures writers have the context and information needed to produce quality documentation
- Provides a mechanism to manage workload and set realistic timelines
- Establishes quality gates to maintain documentation standards
- Creates visibility into upcoming work for better resource planning

**For stakeholders requesting documentation:**

- Clarifies what information is needed and when
- Provides predictable timelines for documentation deliverables
- Establishes accountability for providing necessary inputs
- Creates a framework for collaboration between technical experts and writers

**For the organization:**

- Ensures consistent documentation coverage across products and features
- Prevents documentation gaps that could impact customer experience
- Aligns documentation work with product and business priorities
- Provides metrics and visibility into documentation capacity and throughput

## Core components of an intake process

A comprehensive intake process typically includes the following components. Your team should define each component based on your organizational structure, workflows, and constraints.

### 1. Criteria for determining if documentation is needed

Define clear criteria for when documentation work is required. This might be based on:

- Customer impact (any customer-facing change requires documentation)
- Change type (new features, deprecations, breaking changes)
- Compliance or regulatory requirements
- Support ticket volume or customer questions
- Internal team needs (onboarding documentation, runbooks)

Establish who makes the initial determination and how exceptions are handled. Some teams empower product managers to make this call, while others have docs teams review all planned work during regular syncs.

### 2. Notification requirements and timelines

Specify when and how stakeholders must notify the docs team of upcoming work. Key considerations:

**Timing:**

- How much advance notice is required? (Common ranges: 1-4 weeks before completion)
- Should notification happen at the planning stage, implementation stage, or a fixed time before release?
- How do urgent requests or emergency releases affect timing requirements?

**Communication channels:**

- Where should notification occur? (Team meetings, issue tracking systems, email, chat)
- Is automated notification possible based on project labels or categories?
- Who must be notified? (Specific individuals, team aliases, documentation leads)

### 3. Documentation request creation

Define what information must be provided to constitute a complete documentation request. This typically includes:

**Minimum required information:**

- Work description and scope
- Target audience and use cases
- Release or publication timeline
- Stakeholder contact information
- Links to relevant technical specifications, designs, or research
- Customer impact statement

**Optional but helpful information:**

- Competitive analysis or market context
- Known limitations or trade-offs
- Related work or dependencies
- Success metrics or business objectives

Consider using templates, intake forms, or structured fields in your project tracking system to standardize request creation.

### 4. Draft and content requirements

Establish expectations for who creates the first draft and what it should contain. Common approaches:

**Draft creation responsibility:**

- Technical writers create drafts from specifications
- Subject matter experts create drafts that writers refine
- Product managers create outlines that writers expand
- Collaborative drafting between multiple stakeholders

**Content requirements:**

- What sections or information must be included?
- What level of completeness is expected in the first draft?
- Are there different requirements for different documentation types (tutorials vs. reference vs. conceptual guides)?
- When must the draft be submitted relative to the publication deadline?

### 5. Review and approval workflows

Define who must review and approve documentation before publication, and what each reviewer is responsible for verifying:

**Common reviewer roles:**

- Technical accuracy (subject matter experts, engineers)
- Product alignment (product managers, product marketing)
- Style and standards (peer writers, documentation leads)
- Overall quality and completeness (assigned writer)
- Additional stakeholders (legal, security, compliance, accessibility specialists)

**Review process details:**

- In what order do reviews occur? (Parallel or sequential)
- What is the expected turnaround time for each reviewer?
- Who has final approval authority?
- Can documentation be published over objections? If so, who can authorize this?

### 6. Accountability and consequences

Clarify who is ultimately accountable for ensuring documentation support and what happens if the intake process is not followed:

**Accountability:**

- Who is responsible for ensuring documentation requests are complete and timely?
- How is accountability different for different types of work or initiatives?
- What support is available for stakeholders unfamiliar with the process?

**Consequences of non-compliance:**

- Can docs teams refuse to support work that doesn't follow the process?
- Can releases be delayed if documentation isn't ready?
- Who makes the final decision in conflicts between release timelines and documentation quality?
- How are repeated process violations addressed?

## Defining your intake process

When defining or refining your documentation intake process:

**Start with your constraints:**

- How much advance notice does your team realistically need?
- What workload can your team handle given current staffing?
- What information is already captured in existing workflows?
- What authority does your docs team have to block or delay releases?

**Involve stakeholders:**

- Work with product managers, engineering leads, and other frequent requesters to understand their constraints
- Test your proposed process with a small pilot group before rolling it out broadly
- Gather feedback and iterate based on real-world usage

**Make it as simple as possible:**

- Minimize the number of steps and required fields
- Integrate with existing tools and workflows rather than introducing new systems
- Provide templates, examples, and clear instructions
- Automate what you can (notifications, status updates, reminders)

**Build in flexibility:**

- Define how urgent or emergency requests are handled
- Establish escalation paths for conflicts or edge cases
- Allow for different processes based on documentation type or project size
- Include a mechanism for process exceptions with appropriate approvals

**Make it measurable:**

- Track compliance with intake requirements
- Measure time from request to publication
- Monitor documentation quality metrics
- Use data to identify bottlenecks and improvement opportunities

## Common variations

Documentation intake processes vary significantly based on team size, organizational structure, and product complexity:

**Small teams or startups:**

- May use informal processes with direct communication
- Often have writers embedded with product teams
- May create documentation after release rather than as part of the release process

**Large organizations:**

- Often have formal ticketing systems and service level agreements
- May have specialized roles (information architects, API documentation specialists)
- Typically require more extensive approval chains

**API-focused products:**

- May require code-complete APIs before documentation can begin
- Often have automated documentation generation from code
- May have different processes for reference documentation vs. guides

**Open source projects:**

- May rely on community contributions for first drafts
- Often have lower barriers to entry but higher quality bars for merging
- May separate documentation for end users vs. contributors

## Related concepts

An intake process works in conjunction with other docs team processes and frameworks:

- **[Minimum requirements for writer assignment](minimum-requirements.md)**: Defines the specific information needed before a writer can be assigned to work
- **[RACI matrix](raci-matrix.md)**: Clarifies roles and responsibilities across the documentation lifecycle
- **[Feature documentation guidelines](feature-documentation.md)**: Establishes content and quality standards for documentation deliverables
- **Service level agreements (SLAs)**: Defines expected turnaround times and response times for documentation requests
- **Documentation prioritization frameworks**: Provides criteria for prioritizing competing documentation requests
- **Quality standards and style guides**: Establishes the bar for publication-ready documentation

## Example

See [Sample intake process](../examples/sample-intake-process.md) for a complete example demonstrating these concepts.
