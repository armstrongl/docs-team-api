# Minimum requirements

Minimum requirements define the baseline conditions a project must meet before your team commits resources. They create a clear contract between your team and stakeholders: meet these requirements, and you can expect support; fail to meet them, and support is not guaranteed.

## Why minimum requirements matter

Docs teams have limited capacity. Without clear intake criteria, teams face constant triage decisions and stakeholders have no visibility into what determines priority. Minimum requirements solve both problems by establishing transparent, predictable criteria.

Minimum requirements also protect documentation quality. Projects that arrive without essential information (target audience, subject matter experts, review contacts) produce documentation that misses the mark or requires extensive rework.

## Core components

Effective minimum requirements share four characteristics: a structured checklist, a clear accountability model, defined consequences, and integration with work tracking systems.

### Checklist structure

Organize requirements as a checklist with clear pass/fail criteria. Avoid subjective requirements like "sufficient detail" in favor of binary checks like "target audience is specified." Checklists eliminate ambiguity about whether a project qualifies for support.

Each checklist item should be:

- **Verifiable**: Someone can confirm whether the requirement is met without judgment calls.
- **Necessary**: The requirement exists because its absence causes real problems.
- **Documented**: The requirement links to guidance on how to satisfy it.

### Accountability model

Someone must own ensuring requirements are met. This is typically the project lead, product manager, or whoever initiates the documentation request. Clear accountability prevents the "I thought someone else was handling that" failure mode.

The accountable party should:

- Understand what the requirements are and why they exist.
- Have authority to gather the necessary information from stakeholders.
- Receive clear feedback when requirements are not met.

### Consequences framework

Requirements without consequences are suggestions. Define what happens when requirements are not met: deprioritization, no dedicated resources, delayed delivery, or requiring the requesting team to provide draft content.

Consequences should be:

- **Proportional**: The consequence matches the severity of missing requirements.
- **Predictable**: Stakeholders know in advance what will happen.
- **Consistently applied**: Everyone receives the same treatment.

### Work tracking integration

Minimum requirements should connect to your work tracking system (epics, tickets, requests). This creates an auditable record, enables automation (blocking workflows until requirements are met), and ensures requirements are checked at the right time in the process.

Common integration patterns:

- A documentation request ticket type with required fields.
- Parent-child relationships between project epics and documentation requests.
- Automated validation that blocks incomplete requests.

## Defining your own minimum requirements

Start by identifying the information your team needs to begin work effectively. Work backward from common problems: What causes rework? What missing information leads to delays? What ambiguity creates scope creep?

### Questions to consider

- What information do writers need on day one?
- Who must be available for technical questions?
- What existing materials should accompany the request?
- When is the target delivery date, and is it realistic given the scope?
- Who must review and approve the documentation?

### Balancing rigor and accessibility

Too few requirements, and your team wastes time on incomplete requests. Too many requirements, and stakeholders avoid the formal process entirely. Aim for the minimum set of requirements that prevents the most common failure modes.

Start conservative. Add requirements only when you see repeated problems that a new requirement would prevent. Remove requirements that rarely cause issues when unmet.

### Making requirements visible

Document your minimum requirements where stakeholders can find them. Link to them from your intake forms, request templates, and team documentation. When rejecting incomplete requests, reference the specific requirements that were not met.

## Related concepts

- **[Intake process](./intake-process.md)**: The workflow for submitting and reviewing documentation requests.
- **Prioritization criteria**: How accepted requests are ordered in the backlog.
- **Service level agreements**: Commitments about response time and delivery timelines.
- **Escalation paths**: What happens when disagreements arise about priorities or requirements.

## Examples

See the [examples folder](../examples/) for sample minimum requirements documents, including:

- [Sample minimum requirements](../examples/sample-minimum-requirements.md): A complete example showing checklist structure, required fields, and accountability model.
