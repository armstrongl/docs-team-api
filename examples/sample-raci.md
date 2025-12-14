# Sample RACI matrix: Docs team for feature launches

This example demonstrates a generic RACI matrix structure for a docs team coordinating on feature launches with product, engineering, and design teams. Use this as a starting point and adapt it to your organization's specific roles, phases, and activities.

---

## Key

This section defines the four responsibility types used throughout the matrix to clarify roles and accountability for each activity.

- **R (Responsible):** Does the work.
- **A (Accountable):** Ultimately answerable for completion; approves the work.
- **C (Consulted):** Provides input before or during the work.
- **I (Informed):** Kept updated on progress or outcomes.

## Roles

This section lists all role abbreviations used in the responsibility matrices below. Customize these roles to match your organization's structure.

- **PM:** Product manager.
- **EM:** Engineering manager or tech lead.
- **Eng:** Engineer.
- **Writer:** Technical writer or documentation specialist.
- **Docs Lead:** Docs team lead.
- **Designer:** UX/UI designer.
- **Marketing:** Product marketing manager or marketing team.

## How to interpret shared responsibility

When multiple roles appear in the R (Responsible) column, it indicates collaborative work where each party contributes specific expertise:

- **Sequential collaboration:** Different roles contribute at different stages (e.g., PM initiates, Eng provides technical input, Writer validates).
- **Parallel contribution:** Multiple roles work simultaneously on different aspects of the same deliverable.
- **Conditional responsibility:** The actual responsible party varies based on project circumstances (e.g., complexity, team availability, specific expertise required).

The **A (Accountable)** column clarifies who ultimately owns the outcome and ensures completion. When in doubt about who should do what, consult the accountable party to determine the specific division of labor for your situation. See footnotes on specific activities for examples of how shared responsibility works in practice.

## Planning phase

This phase covers initial feature scoping, requirements gathering, and documentation planning activities that occur before development begins.

| Activity | R | A | C | I |
|----------|---|---|---|---|
| Create feature specification. | PM | PM | Eng, EM, Designer | Writer |
| Define documentation requirements. | PM | PM | EM | Writer |
| Create documentation plan.<sup>1</sup> | Writer, Eng, PM | PM | EM | Docs Lead |
| Determine if documentation is needed.<sup>2</sup> | Writer, PM | PM | Writer, Eng, EM | Designer |
| Estimate documentation effort. | Writer, PM | PM | Eng, EM | |
| Assign writer to feature. | Docs Lead | Docs Lead | | EM, PM |

**Notes:**

1. **Create the documentation plan:** PM initiates and owns the plan based on product requirements. Eng provides technical details about implementation scope. Writer validates the plan's feasibility and advises on documentation approach and effort.

2. **Determine if documentation is needed:** PM makes the initial determination based on feature scope and user impact. Writer reviews and validates this decision to ensure alignment with documentation standards and priorities.

## Development phase

This phase covers feature implementation and documentation creation activities that occur in parallel.

| Activity | R | A | C | I |
|----------|---|---|---|---|
| Develop feature code. | Eng | EM | PM | Writer |
| Write first documentation draft.<sup>3</sup> | Eng, PM, Writer | PM | EM | Docs Lead |
| Identify and update related documentation. | Writer | PM | Eng | EM |
| Review documentation for technical accuracy. | Eng | PM | Writer | EM |
| Review documentation for style and quality. | Writer | Writer | PM | EM |
| Approve documentation for release. | PM | PM | EM | Writer |

**Notes:**

3. **Write first documentation draft:** PM is accountable for ensuring the first draft exists and meets the deadline, but may delegate the actual writing to Eng, a subject matter expert, or Writer. The responsible party writes the initial draft. The accountable party ensures it happens on time.

## Publishing phase

This phase coordinates the final publication activities across documentation and feature deployment.

| Activity | R | A | C | I |
|----------|---|---|---|---|
| Coordinate publishing timeline. | PM | PM | Eng, Writer | Marketing |
| Publish documentation. | Writer | PM | | EM, Marketing |
| Publish feature. | Eng | EM | PM | Marketing, Writer |
| Create changelog entry. | Writer | PM | PM | EM |

## Post-launch phase

This phase handles documentation updates and corrections identified after the feature has been released.

| Activity | R | A | C | I |
|----------|---|---|---|---|
| Notify docs team of post-launch changes. | PM | PM | EM | Docs Lead |
| Prioritize documentation fixes. | Docs Lead | Docs Lead | PM | EM |
| Make documentation corrections. | Writer | Docs Lead | PM | EM |
| Approve and publish corrections. | Writer | Writer | PM | EM |

---

## Customization guidance

This example demonstrates common patterns you can adapt:

### Variation 1: Engineering-led documentation

If engineers typically write first drafts, adjust the Development phase to make Eng primarily Responsible with Writer in a Consulted role during drafting, then flip to Writer Responsible for review and refinement.

### Variation 2: Embedded writers

If writers are embedded in product teams, you might combine PM and Writer accountability in some activities, or shift more Accountable roles to Docs Lead for centralized quality control.

### Variation 3: External contributors

If you work with external contributors (contractors, community members), add them as a role and define their responsibilities in specific phases where they contribute.

### Key principles to maintain

- Only one person is Accountable (A) for each activity
- At least one person must be Responsible (R) for each activity
- Not every role needs to appear in every activity
- Document shared responsibility in footnotes for clarity

Adapt the phases, activities, and roles to reflect your team's actual workflow, not an idealized process.
