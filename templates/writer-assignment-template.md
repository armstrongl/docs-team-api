# Writer assignment process template

Use this template to define how your docs team allocates writing resources to documentation requests. This process establishes transparent, predictable resource allocation while maintaining flexibility for changing priorities.

**How to use this template:**

- Replace example text with your organization's specific practices, timelines, and terminology
- Adapt section headings to match your planning cycle terminology (quarterly, sprint-based, release-based, etc.)
- Customize inline guidance to reflect your team's capacity management and prioritization approaches
- Delete the "Customization notes" subsections once you've tailored the content to your needs
- For detailed guidance on writer assignment concepts and best practices, refer to [Writer assignment process](../docs/writer-assignment.md)
- For a concrete implementation example, see [Sample writer assignment](../examples/sample-writer-assignment.md)

---

## Planning cycle assignment

The docs team assigns writers to documentation requests at the start of each planning period based on which parent initiatives meet predefined minimum requirements.

At the beginning of each planning cycle (quarterly, bi-annually, or sprint-based), the docs team meets to assign writers to documentation requests that meet the minimum requirements. Assignment happens during the first week of the period.

For this process to work, all parent initiatives and corresponding documentation requests should be created during planning before the period begins.

### Customization notes

- **Planning cycle terminology**: Replace "planning period" with your organization's terminology (quarter, sprint, release cycle, etc.). Ensure consistency throughout the document.
- **Minimum requirements**: Define what constitutes a "ready" documentation request based on your team's needs. Common criteria include:
  - Completed design documents or technical specifications
  - Approved product requirement documents (PRDs)
  - Stakeholder sign-off and commitment to support documentation
  - Clear timeline with realistic deadlines
  - Required approvals (legal, security, product) obtained or scheduled
- **Assignment timing**: Adjust the "first week" timeline based on your planning cycle length. Shorter cycles may require same-day assignment; longer cycles may allow for two-week assignment windows.
- **Assignment mechanism**: Specify whether assignment happens in a dedicated meeting, asynchronously through a tool, or via another process your team uses.

## Before the planning period starts

This section outlines the steps required to ensure your parent initiative is ready for writer assignment during the initial planning phase.

If your parent initiative is planned for the upcoming period:

- Create your parent initiative and corresponding documentation request during planning (before the period begins).
- Ensure your parent initiative meets the minimum requirements for writer assignment.

If the requirements are met, the docs team assigns a writer during the first week of the period.

If requirements are not met, the docs team will not assign a writer.

### Customization notes

- **Creation process**: Add specific details about where and how parent initiatives are created (specific project management tool, template to use, approval workflow, etc.).
- **Requirement validation**: Specify who validates that minimum requirements are met (docs team lead, program manager, automated checklist) and when this validation occurs.
- **Communication of assignment decisions**: Describe how requesters are notified about writer assignment or non-assignment (email notification, project management tool update, synchronous meeting, etc.).
- **Remediation path**: If requirements are not met, clarify what requesters need to do to make their initiative ready for future assignment.

## If your parent initiative becomes ready mid-period

Parent initiatives that miss the initial assignment window can still receive documentation support if they meet requirements and capacity is available.

If your parent initiative was not ready for assignment at the beginning of the period but becomes ready mid-period:

- Bring it up in the next cross-functional sync.
- If the minimum documentation request requirements are met, the docs team will assign a writer.

Mid-period changes should only happen if priorities shift in a way that makes it necessary to update the parent initiatives for a period. Flexibility is expected, but these situations are handled on a case-by-case basis.

### Customization notes

- **Escalation channel**: Replace "cross-functional sync" with your team's appropriate meeting or communication channel for mid-cycle requests. Options include:
  - Dedicated Slack channel with defined response SLA
  - Standing weekly triage meeting
  - Asynchronous request queue with regular review cadence
  - Direct escalation to docs team lead or manager
- **Mid-cycle policy**: Adjust the flexibility guidelines based on your organization's change management practices. Consider specifying:
  - What constitutes a legitimate priority shift (executive directive, customer emergency, regulatory requirement)
  - Maximum number of mid-cycle additions the docs team can accommodate
  - Impact on existing commitments when mid-cycle work is accepted
- **Capacity reassessment**: Describe how the docs team evaluates whether they can accept additional work mid-cycle (capacity dashboard review, team discussion, manager decision).
- **Tradeoff discussions**: Specify whether accepting mid-cycle work requires dropping existing work, and who makes that decision.

## Constraints

The docs team operates with finite resources and uses a collaborative prioritization process to allocate writer capacity across competing requests.

The docs team has limited capacity and might not be able to support all requests.

Capacity conflicts are resolved collaboratively in the cross-functional sync on a case-by-case basis. It is the docs team's responsibility to communicate when they are at capacity. Decisions about which documentation requests get resources are made collaboratively.

### Customization notes

- **Prioritization framework**: Add specific criteria your team uses for prioritization when capacity is constrained. Common factors include:
  - Business impact (revenue potential, strategic importance, customer commitments)
  - User impact (number of users affected, severity of user pain point)
  - Regulatory or compliance requirements
  - Risk mitigation (security, legal, operational risk)
  - Alignment with company OKRs or strategic initiatives
- **Escalation path**: Define what happens when collaborative resolution doesn't work. Options include:
  - Escalation to department leads or executives
  - Voting mechanism with defined stakeholders
  - Tie-breaker authority (VP of Engineering, Chief Product Officer, etc.)
- **Capacity visibility**: Determine how capacity constraints are communicated to stakeholders. Options include:
  - Real-time dashboard showing writer assignments and availability
  - Regular capacity reports distributed to stakeholder mailing list
  - Capacity noted in planning artifacts or project management tools
  - Discussed in standing cross-functional meetings
- **Capacity planning**: Specify how the docs team forecasts and communicates capacity for upcoming periods (historical velocity, current commitments, planned time off, etc.).

## Variations to consider

Different organizational contexts may require different approaches. Consider whether any of these variations better fit your team's needs:

- **Continuous assignment**: Some teams may prefer ongoing assignment rather than fixed planning cycles. This works well for smaller docs teams or organizations with continuous delivery practices.
- **Dedicated writers**: Projects with dedicated writer resources may not need this process. Large strategic initiatives often have embedded documentation specialists.
- **Self-service documentation**: Technical teams writing their own documentation may use this process for review capacity rather than writing capacity. The docs team provides editing, structure guidance, and publishing support.
- **External documentation**: Teams managing third-party documentation (partner docs, vendor content) may need additional approval gates or legal review before writer assignment.
- **Tiered service levels**: Some docs teams offer different service levels (full-service writing, documentation review only, consultation only) with different assignment processes for each tier.
- **Specialty assignments**: Technical domains requiring specialized expertise (API documentation, security docs, compliance content) may have dedicated writers or require specific qualifications.

### Customization notes

- **Select applicable variations**: Keep only the variations relevant to your organization and expand on how they're implemented.
- **Add organization-specific variations**: Include any unique approaches your team uses that aren't listed here.
- **Document exceptions**: If certain types of work bypass this process entirely (executive requests, incident response documentation, regulatory deadlines), document those exceptions clearly.
