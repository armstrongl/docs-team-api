# Docs team API

A framework for docs teams to define how other teams work with them. Based on the concept of a "team API," this framework makes implicit collaboration patterns explicit by defining input contracts, output contracts, SLAs, and error handling.

You can adapt this framework for other types of teams beyond docs teams.

## What is a team API?

A team API is a documented interface that defines how other teams interact with your team. It specifies:

- **Input contracts**: What information you need to do your work.
- **Output contracts**: What you deliver and in what form.
- **SLAs**: Expected timelines and response times.
- **Error handling**: What happens when things don't go as planned.

The goal is to make collaboration patterns explicit, reducing friction and misunderstandings.

For more information, check out [what's a team API?](docs/whats-a-team-api.md).

## Why use this framework?

Docs teams often struggle with:

- Requests that lack necessary information
- Unclear expectations about timelines
- Last-minute changes that derail planning
- Ambiguity about who is responsible for what

This framework addresses these challenges by providing:

- Clear requirements for documentation requests
- A complexity framework for realistic timeline planning
- Protocols for handling changes and exceptions
- RACI matrices that clarify responsibilities

## Prerequisites and assumptions

This framework is designed for organizations with specific structures and practices. Before adopting it, consider whether your context aligns with these prerequisites and assumptions.

### Organizational prerequisites

Your organization should have these basic structures in place before adopting this framework.

This framework assumes you have:

- A docs team or dedicated documentation function
- A product development process with defined releases or launches
- Cross-functional collaboration mechanisms (meetings, Slack channels, planning sessions)
- A work tracking system (epics, issues, tickets, or similar)

### Assumptions this framework makes

These are the working assumptions that inform the framework's structure and processes.

The framework is built on these assumptions:

- Planning happens in cycles (quarterly, monthly, or similar periods)
- Product managers own feature launches and coordinate cross-functional work
- Documentation is required for customer-facing changes
- Technical writers review and edit documentation (not just write from scratch)
- Teams have regular touchpoints for planning and coordination

### When this framework may not fit

Consider whether significant adaptation is needed before implementing this framework in your organization.

This framework may require significant adaptation if your organization has:

- Very small teams where individuals wear multiple hats
- No dedicated documentation resources
- Fully async teams with no synchronous touchpoints
- Continuous deployment without discrete launches or releases
- Ad hoc processes without formal planning cycles

The framework can be adapted for different contexts by modifying roles, timelines, and processes to match your organizational reality. Start with the pieces that provide the most value and evolve from there.

## Document index

Navigate the framework documentation organized by category: core framework documents, templates, and examples.

### Core framework

| Document | Description |
|----------|-------------|
| [Overview](docs/overview.md) | Main framework document defining how teams work with docs. |
| [What's a team API?](docs/whats-a-team-api.md) | Explains the Team API concept and its benefits. |
| [Intake process](docs/intake-process.md) | How documentation requests enter the system. |
| [Timeline](docs/timeline.md) | Milestone relationships from planning to launch. |
| [Complexity framework](docs/complexity-framework.md) | Low, medium, high estimation patterns for timeline planning. |
| [Documentation plan](docs/documentation-plan.md) | What requesters must provide in their documentation plan. |
| [Writer assignment](docs/writer-assignment.md) | How writers get assigned to projects. |
| [Minimum requirements](docs/minimum-requirements.md) | Prerequisites for writer assignment. |
| [Last-minute changes](docs/last-minute-changes.md) | Protocol for handling changes after cut-off dates. |
| [RACI matrix](docs/raci-matrix.md) | Responsibility assignments for launch activities. |
| [Glossary](docs/glossary.md) | Shared terminology definitions. |
| [Feature documentation](docs/feature-documentation.md) | Requirements for documenting features. |

### Templates

Ready-to-use templates for implementing the framework in your organization.

| Template | Description |
|----------|-------------|
| [Overview template](templates/overview-template.md) | Template for team API overview documents. |
| [Intake template](templates/intake-template.md) | Template for documentation intake requests. |
| [Timeline template](templates/timeline-template.md) | Template for milestone timelines. |
| [Complexity framework template](templates/complexity-framework-template.md) | Template for complexity assessment criteria. |
| [Documentation plan](templates/documentation-plan.md) | Fill-in template for documentation plans. |
| [Writer assignment template](templates/writer-assignment-template.md) | Template for writer assignment processes. |
| [Minimum requirements template](templates/minimum-requirements-template.md) | Template for intake prerequisites. |
| [RACI template](templates/raci-template.md) | Blank RACI for customization. |
| [Glossary template](templates/glossary-template.md) | Template for terminology definitions. |
| [Feature documentation template](templates/feature-documentation-template.md) | Template for feature documentation requirements. |

### Examples

Sample implementations showing how the framework works in practice.

| Example | Description |
|---------|-------------|
| [Sample overview](examples/sample-overview.md) | Sample team API overview document. |
| [Sample intake](examples/sample-intake.md) | Completed intake for a fictional feature. |
| [Sample intake (high complexity)](examples/sample-intake-high-complexity.md) | Completed intake for a fictional high-complexity feature introducing a new syntax and multi-system coordination. |
| [Sample intake process](examples/sample-intake-process.md) | Detailed intake process example with variations and customization notes. |
| [Sample timeline](examples/sample-timeline.md) | Timeline diagram and milestone descriptions for a medium-complexity feature. |
| [Sample complexity framework](examples/sample-complexity-framework.md) | Example complexity assessment framework with three tiers. |
| [Sample documentation plan](examples/sample-documentation-plan.md) | Completed documentation plan for a fictional feature. |
| [Sample writer assignment](examples/sample-writer-assignment.md) | Writer assignment process example with planning cycle management. |
| [Sample minimum requirements](examples/sample-minimum-requirements.md) | Example of minimum requirements checklist for project intake. |
| [Sample last-minute change](examples/sample-last-minute-change.md) | Complete last-minute change scenario from notification through resolution. |
| [Sample last-minute changes](examples/sample-last-minute-changes.md) | Protocol document for handling late changes. |
| [Sample RACI](examples/sample-raci.md) | RACI adapted for a support team. |
| [Sample feature documentation](examples/sample-feature-documentation.md) | Example feature documentation requirements and standards. |
| [Sample glossary](examples/sample-glossary.md) | Sample glossary with common documentation process terms. |

## Adapting the framework

This framework is designed to be customized to fit your organization's specific tools, roles, and processes.

Key areas to adapt:

### Tools

The framework references generic concepts like "project tracker" and "communication channels." Replace these with your specific tools:

- Project tracker: Jira, Linear, Asana, GitHub Issues, and others
- Communication channels: Slack, Teams, Discord, and others
- Project documents: Google Docs, Notion, Confluence, and others

### Roles

The framework uses common roles like product manager, engineering manager, and technical writer. Map these to your organization's titles and responsibilities.

### Timelines

The complexity framework provides baseline timelines. Adjust these based on your team's capacity, typical workload, and organizational velocity.

### Processes

The RACI matrix and intake process reflect one approach. Modify phases, activities, and responsibilities to match how your organization actually works.

## Contributing

See [`CONTRIBUTING.md`](CONTRIBUTING.md) for guidelines on improving this framework.

## License

This framework is available under the MIT License. See [`LICENSE`](LICENSE) for details.
