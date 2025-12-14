# Documentation Team API overview

The Documentation Team API defines how teams work with the docs team. It specifies what information the docs team needs to support your work, what the docs team delivers, expected timelines, and what to do when things don't go as planned.

## Communication channels

The docs team uses specific communication channels for different types of interactions. Choose the appropriate channel based on urgency and the nature of your request.

| Channel | Purpose | When to use |
|---------|---------|-------------|
| Cross-functional status channel | Cross-functional coordination for product initiatives. | Escalations, priority conflicts, capacity discussions, urgent requests, mid-cycle changes, last-minute scope changes, and any situation requiring cross-functional decision-making. |
| Product-docs channel | Product manager and docs team collaboration. | Day-to-day questions and coordination between product managers and the docs team. |
| General docs channel | General documentation discussions. | Day-to-day questions from anyone outside the product team, general documentation inquiries. |

In addition to communication channels, the cross-functional sync meeting is where cross-functional decisions about product initiatives are discussed and made. Use the status channel to flag topics for the meeting agenda or to communicate issues that cannot wait until the next meeting.

## How to request documentation support

### When is documentation required?

If a feature or change impacts customers, it requires documentation. This means most product initiatives need documentation support.

The product manager decides whether documentation is required when creating the parent initiative. The docs team reviews all parent initiatives in the cross-functional sync to verify this decision. The decision can be discussed and adjusted during the sync if documentation needs were initially missed.

Documentation is not required for internal-only projects such as CI/CD workflows, DevOps tasks, and similar internal tooling.

### How to request support for a feature launch

Follow these steps to ensure your feature launch gets proper documentation support:

1. Create a parent initiative for your feature
2. Create a documentation request under the parent initiative
3. Add a link to the project document in the documentation request's description field
4. Fill out all required fields on the documentation request

See [minimum requirements for writer assignment](../docs/minimum-requirements.md) for details.

## What the docs team delivers

The docs team provides comprehensive support throughout the feature launch lifecycle, from initial planning through publication.

### Documentation outputs

For feature launches, the docs team delivers:

- Collaboration on the documentation plan section of the project document
- Assistance estimating documentation complexity
- Validation of the documentation plan
- Editorial collaboration and review of the feature documentation
- Assistance identifying related documentation topics (when required)
- Editorial collaboration and review of the changelog
- Publishing the documentation and the changelog

### How timelines are determined

Documentation timelines depend on the feature's complexity, which is assessed using the complexity framework.

| Complexity | Writer review lead time |
|------------|------------------------|
| Low | 1-2 business days |
| Medium | 2-6 business days |
| High | More than 8 business days |

These are general guidelines. Features vary widely, and the documentation complexity for each one is assessed on a case-by-case basis.

### What happens when things change late?

Terminology and brand name changes must be finalized no later than two weeks before launch. Features and functionality that require documentation must also be locked in no later than two weeks before launch.

If changes occur after these cut-off dates, the person who discovers them must notify all involved parties immediately using the status channel and bring it up in the next cross-functional sync. One of the following must then happen:

- The launch is postponed until the documentation is updated
- The scope of documentation is restricted to what's documented correctly, with additional documentation following during the two-week post-launch period

The decision on which option to take is made collaboratively on a case-by-case basis.

For more information, refer to the last-minute changes protocol.

## How writers are assigned

Writers are assigned to documentation requests based on availability, domain expertise, and workload. See the [writer assignment process](../docs/writer-assignment.md) for detailed information.

## Cross-functional processes

Cross-functional processes describe how multiple teams coordinate on specific activities, referencing this docs team API for docs-specific requirements.

The RACI matrix defines responsibilities for all teams involved in launching a feature. It covers the planning phase through post-launch and specifies who is responsible, accountable, consulted, and informed for each activity.

## When things go wrong

This section covers how to handle exceptions, urgent requests, and situations where the standard process isn't followed.

### Who to contact

For questions about documentation support or issues with the process, see the communication channels section above.

### How urgent requests are handled

Exceptions exist for urgent releases, but these require discussion and buy-in from everyone involved. If you believe your release qualifies as urgent, post a message in the status channel immediately and bring it up in the next cross-functional sync.

### What happens if requirements aren't met?

The product manager is ultimately responsible for the success of a release. If the product manager doesn't follow the process or the initiative doesn't meet the minimum requirements for documentation requests:

- There's no guarantee that the project will have documentation support
- Because documentation is required for customer-facing releases, this could result in the release being postponed

If you're concerned that your initiative might not meet the requirements in time, initiate a discussion in the status channel as soon as possible to explore options.

### Override process

In extreme circumstances, the docs team's decision to block publication due to quality concerns can be overridden. This requires leadership approval.

This override process exists for exceptional situations only and should not be treated as a standard path.
