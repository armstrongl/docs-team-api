# Last-minute changes protocol

A last-minute changes protocol establishes what happens when product changes occur after documentation work has reached advanced stages. This protocol creates accountability, defines decision-making authority, and ensures that documentation quality doesn't suffer from late-breaking changes.

## Why docs teams need this protocol

Docs teams face a recurring problem: features change late in the development cycle, often after documentation drafts are complete or nearing completion. Without a formal protocol, these situations default to unstructured negotiation. Writers absorb the impact, timelines slip without visibility, or teams ship with documentation that doesn't match the product.

This protocol exists to make these situations visible and structured. It doesn't prevent late changes—those happen regardless—but it ensures that when they do occur, the team makes conscious decisions about trade-offs rather than defaulting to "the writer will handle it somehow."

## Core components of a change management protocol

An effective last-minute changes protocol consists of several interconnected components that work together to manage the impact of late changes on documentation quality and timelines.

### Cut-off date definitions

Cut-off dates establish when changes trigger the formal protocol. These dates aren't arbitrary deadlines; they represent the point after which changes create significant risk to documentation quality or launch readiness.

The cut-off should be defined relative to the launch date and may vary by change type. Terminology changes might have earlier cut-offs than minor UI adjustments because they affect documentation more broadly. The cut-off serves as a signal that changes after this point require explicit discussion and decision-making.

Cut-off dates are guidelines that create visibility, not rigid rules that prevent all changes. Their purpose is to ensure that late changes receive appropriate scrutiny and that stakeholders understand the documentation impact before proceeding.

### Change impact categories

Different types of changes have different impacts on documentation work. A protocol should define categories that help teams quickly assess what a specific change means for documentation.

Common categories include terminology changes, functionality additions or modifications, UI changes, and architectural changes. Each category describes typical documentation impact: how many topics might be affected, whether new content is needed, and how complex the revision work might be.

These categories serve as a shared language for discussing impact. Instead of debating whether a change is "big" or "small," the team can discuss whether it's a terminology change affecting all topics or a UI change affecting only screenshots.

### Notification requirements

When someone discovers a change after the cut-off, the protocol must specify who notifies whom, how quickly, and through what channels. Notification requirements ensure that all stakeholders learn about the change with enough time to discuss options.

The protocol should specify what information the notification must include: what changed, when it was discovered, what the current launch date is, and who is assigned to the documentation work. This ensures that initial notifications provide enough context for stakeholders to assess urgency.

Notification requirements should also address escalation: when can the discussion wait for the next scheduled meeting, and when does it require immediate attention? Clear escalation criteria prevent both unnecessary urgency and dangerous delays.

### Resolution framework

The protocol must define available options when a late change occurs and specify who makes the decision. Without explicit options and decision authority, discussions can become circular or default to unstated assumptions.

Most protocols offer two primary resolutions: adjust the product timeline to allow for documentation updates, or restrict documentation scope to what can be completed on time while deferring the rest. Some protocols may include additional options like shipping with known documentation gaps (documented as such) or adjusting the launch scope to exclude changed features.

The key is that these options are explicit and known to all stakeholders before a crisis occurs. When a late change happens, the team discusses which option fits the situation rather than inventing solutions under time pressure.

### Decision authority structure

The protocol must specify who makes the decision when a late change occurs. Ambiguous authority leads to either decision paralysis or unilateral choices that ignore stakeholder concerns.

Decision authority might rest with a single role (like a product manager), require consensus among a defined group (product manager, engineering lead, and documentation lead), or escalate to leadership if the immediate stakeholders can't agree. The structure should match the organization's broader decision-making patterns.

What matters is clarity. Everyone involved should know, before a late change occurs, who has the authority to decide how to proceed.

### Documentation and tracking requirements

Decisions made under time pressure are easily forgotten. The protocol should require that all decisions are documented in specific locations that ensure both immediate visibility and long-term traceability.

Documentation typically happens in two places: a communication channel where the team is coordinating (for immediate visibility to all stakeholders), and the work item tracking system (for permanent record and retrospective review). The protocol should specify exactly what information must be recorded.

If documentation scope is restricted, the protocol should require creating tracked work items for deferred tasks immediately, not after launch. This prevents deferred work from being forgotten or deprioritized after the immediate launch pressure subsides.

### Post-launch accountability

When documentation scope is restricted, someone must be accountable for completing the deferred work. The protocol should specify who owns this work, what the timeline expectations are, and how deferred work is tracked.

Post-launch accountability often falls to the same writer who handled the initial launch, ensuring continuity of context. The timeline for completion should be explicit—not "soon" or "after launch," but a specific window like "within two weeks of launch."

The protocol should also address what happens if the assigned person realizes they can't meet the post-launch timeline. Early escalation requirements prevent deadline surprises and allow the team to provide support or adjust expectations before the deadline passes.

## Creating your own change management protocol

Teams implementing this protocol should start by understanding their specific pain points. What actually happens when late changes occur today? Where does the current process break down? The protocol you create should address your actual problems, not hypothetical ones.

Begin by defining your cut-off dates based on your team's actual production timeline. How long does documentation typically take from draft to publication? When do late changes historically cause the most disruption? Your cut-off should provide enough buffer for quality work while being realistic about your development process.

Identify the stakeholders who must be involved in decisions about late changes. In most organizations, this includes product management, engineering leadership, and documentation leadership at minimum. The protocol should name these roles explicitly, not refer to vague groups like "stakeholders" or "the team."

Define your resolution options based on what your organization can actually do. If postponing launches is culturally impossible, don't include it as an option. If your team can ship with known documentation gaps (properly disclosed), that might be a valid option. The protocol works only if the stated options are real choices, not theoretical possibilities.

Establish where decisions will be documented. Use systems and channels your team already checks regularly. A protocol that requires documentation in a system nobody uses will be ignored.

Test the protocol with a retrospective exercise. Review a past late change situation and walk through how the protocol would have applied. Did it provide the structure you needed? Did it specify who would make decisions? Would it have resulted in a better outcome? Adjust based on what you learn.

## Customizing the protocol for your context

Different teams need different levels of formality. A small docs team supporting a single product might need only a lightweight protocol with simple escalation paths. A large organization with multiple docs teams might need more structure to ensure consistency across teams.

Consider whether your cut-off dates should vary by change type or product maturity. New products under rapid development might need more flexible protocols than mature products where late changes are rare. Some teams use stricter cut-offs for major releases than for minor updates.

The notification and escalation requirements should match your team's working patterns. If your team has daily standups, the protocol might use those as the default escalation path. If you work asynchronously across time zones, you need different notification mechanisms.

Decision authority should reflect your organization's culture. Some organizations prefer consensus-based decisions; others prefer designated decision-makers. The protocol should codify what actually works in your environment, not what seems ideal in theory.

Post-launch timelines should be realistic for your team's capacity and sustainable for your writers. A two-week window works for some teams; others might need three weeks or one week depending on how they balance new work with maintenance.

## Related concepts

- **[Documentation intake process](intake-process.md)**: Defines how documentation requests enter the system under normal circumstances
- **[RACI matrix](raci-matrix.md)**: Establishes standard roles and responsibilities that may need adjustment when late changes occur
- **[Timeline](timeline.md)**: Defines milestone relationships and cut-off dates that trigger this protocol
- **[Overview](overview.md)**: Describes communication channels and escalation paths for late changes

## Example

See [Sample last-minute changes protocol](../examples/sample-last-minute-changes.md) for a complete example demonstrating these concepts.
