# Last-minute changes protocol

This protocol defines what happens when changes to a feature occur after the documentation cut-off date. It establishes notification requirements, resolution options, and accountability for any work that must be deferred to the post-launch period.

## Relationship to other processes

This protocol works alongside the standard intake process and the RACI matrix. The intake process defines how documentation requests enter the system under normal circumstances. This protocol defines what happens when those circumstances change late in the release cycle.

When last-minute changes occur, the resolution might affect timelines and responsibilities defined in the RACI. Any adjustments to RACI commitments must be documented as described in the recording decisions section.

## Cut-off dates

The following cut-off dates establish when changes require this protocol to be invoked.

| Change type | Cut-off |
|-------------|---------|
| Terminology and brand name changes | Two weeks before launch. |
| Features and functionality changes | Two weeks before launch. |

These cut-off dates are guidelines, not rigid rules. They exist because changes after this point create significant risk to documentation quality and launch readiness. However, the actual impact of a change depends on its scope and the current state of the documentation.

## Types of changes and their impact

Not all changes have the same impact on documentation. The following categories provide context for discussions about how to handle a specific change. All changes that occur after the cut-off require a discussion; these categories help inform that conversation.

- **Terminology changes** have broad impact. A terminology change affects all documentation that references the term, the changelog, and potentially marketing materials. Even a single term change can require updates across multiple topics.
- **Functionality additions** require new documentation. If a feature gains a new capability after the cut-off, the documentation must be extended to cover it. This typically requires new sections or new how-to guides.
- **Functionality modifications or removals** require revisions to existing documentation. These changes can be deceptively complex because they may affect instructions, requirements, limitations, and examples throughout the existing draft.
- **Minor UI changes** might require only screenshot updates or minor wording adjustments. These are generally lower impact, but even small changes need time to implement and review.

## Notification process

When someone discovers a change after the cut-off date, they must notify all involved parties immediately. The person who discovers the change is responsible for initiating notification, though this is typically the engineering manager or product manager.

### How to notify

Post a message to the appropriate team communication channel as soon as the change is identified. The message should include:

- A clear description of what changed.
- When the change was discovered.
- The current launch date.
- The assigned writer (tag them directly).

### When to escalate

If the next scheduled cross-functional sync provides enough time to discuss the change and implement a resolution before launch, the discussion can wait for that meeting.

If the next sync is too close to the launch date to allow for implementation, the product manager must coordinate an immediate discussion. This discussion must include at minimum:

- The product manager.
- The engineering manager or tech lead.
- The assigned writer.

Other stakeholders might be included as needed based on the nature of the change.

## Resolution options

Every discussion of a last-minute change must result in one of two outcomes. There is no option to proceed with launch while leaving documentation inaccurate or incomplete.

### Option 1: Postpone the launch

The launch is postponed until the documentation is updated to reflect the change. This option is appropriate when:

- The change is significant enough that launching with incomplete documentation would harm users.
- The documentation can be updated within a reasonable timeframe.
- Postponing the launch is acceptable to stakeholders.

### Option 2: Restrict documentation scope

The documentation scope for the launch is restricted to what can be accurately documented before the launch date. The remaining documentation work is addressed during the two-week post-launch period. This option is appropriate when:

- The change affects a portion of the feature that can be temporarily excluded from documentation.
- Users can still benefit from the feature with partial documentation.
- The team commits to completing the remaining documentation promptly after launch.

When this option is selected, the product manager, engineering manager, and writer must agree on exactly what documentation will be included at launch and what will be deferred. This agreement must be explicit, not assumed.

### Decision authority

The decision on which option to take is made collaboratively by the product manager, engineering manager, and assigned writer. There is no single decision-maker; the group must reach agreement. If agreement cannot be reached, the issue should be escalated to leadership.

## Recording decisions

All decisions made under this protocol must be recorded in two locations to ensure both immediate visibility and long-term traceability.

### Communication channel record

Post a summary of the decision to the thread where the issue was initially raised. This summary should include:

- The change that triggered the discussion.
- The resolution chosen (postpone or restrict scope).
- If scope was restricted: what documentation is included at launch and what is deferred.
- Any adjusted timelines.

### Work item record

Add a comment to the documentation request for the launch that documents:

- The change that occurred after cut-off.
- The date the change was discovered.
- The resolution decision.
- If scope was restricted: the specific items deferred to post-launch.
- Links to any new issues created for deferred work.

This record serves as the permanent history and ensures that anyone reviewing the launch can understand what happened and why.

## Post-launch accountability

When the team chooses to restrict documentation scope, the deferred work must be completed during the two-week post-launch period.

### Responsibility

The assigned writer is responsible for completing deferred documentation work. This is the same writer who was assigned to the original launch, ensuring continuity and context.

### Tracking deferred work

All deferred documentation items must be created as separate issues under the same documentation request. These issues should be created immediately after the resolution decision, not after launch. Each issue should clearly describe:

- What documentation is needed.
- The context of why it was deferred.
- The two-week deadline for completion.

### Timeline and communication

The writer must complete deferred documentation within the two-week post-launch window. If the writer determines they cannot meet this deadline, they must communicate this concern to stakeholders as early as possible. Early communication lets other team members (such as engineers or the product manager) assist with drafting or review if needed.

Stakeholders who must be notified of deadline concerns include at minimum:

- The product manager.
- The engineer or SME who can provide technical information.
- The docs team lead (if capacity is the constraint).

Waiting until the deadline has passed to raise concerns is not acceptable. The goal of early communication is to enable the team to find solutions together.
