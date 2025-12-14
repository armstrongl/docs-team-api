# Sample intake process for feature releases

This example demonstrates how a documentation intake process might work for a docs team supporting product feature releases. Adapt the roles, timelines, terminology, and requirements to match your organization's needs.

## Determining if documentation is required

All customer-facing features require documentation. If a change impacts customers in any way, the docs team must be involved. Internal-only projects (for example, CI/CD workflows, internal tooling) typically do not require documentation unless they affect how team members support customers.

**In this example:**
- The product manager makes the initial determination when creating the parent initiative
- The docs team reviews all parent initiatives during the cross-functional sync to verify that documentation needs are correctly identified
- This determination can be overridden by anyone involved during the sync if they identify documentation needs that were initially missed

**Variations:**
- Some teams use automated triggers based on issue labels or project categories
- Some organizations require engineering managers or release coordinators to make the determination
- Some teams maintain a checklist or decision tree to standardize the determination

## Notifying the docs team

If documentation is required, the product manager must notify the docs team at least two weeks before the estimated code complete date, even if all details are not finalized. This communication should occur in the cross-functional sync and through a message in the appropriate team communication channel.

**Variations:**
- Timeline might be 3-4 weeks for complex features or 1 week for minor updates
- Notification might happen through automated issue creation, email, or project management tools
- Some teams require notification at the planning stage rather than at a fixed time before code complete

## Creating the documentation request

Every parent initiative that involves customer-facing changes must have a corresponding documentation request that meets minimum requirements for writer assignment. If these requirements are not met, the docs team will not assign a writer to the work.

**In this example, minimum requirements include:**
- Feature name and description
- Target release date
- Customer impact statement
- Links to technical specifications or design documents
- Primary stakeholder contact information

**Variations:**
- Some teams use templates in their issue tracking system
- Some teams require additional information like competitive analysis, customer research, or marketing messaging
- Some teams use a formal intake form or ticketing system

## First draft requirements

The product manager is accountable for ensuring that a first draft of the documentation is created as a pull request (or equivalent). While the product manager does not need to write the draft themselves, they must ensure it is written, whether by an engineer, a subject-matter expert, the assigned writer, or multiple individuals.

**In this example:**
- The first draft must contain everything the user needs to know about the feature
- The draft must be submitted at least one week before the planned publication date
- The draft should include all required sections: overview, prerequisites, step-by-step instructions, examples, and troubleshooting (when applicable)

**Variations:**
- Some teams have the technical writer create the first draft from specifications
- Some teams require only an outline or bullet points rather than a full draft
- Some teams use different draft requirements based on documentation type (API reference vs. tutorial vs. conceptual guide)

## Documentation approval

Before documentation can be published, it must receive approval from all of the following stakeholders to ensure technical accuracy, style consistency, and overall quality:

**In this example:**
- The product manager verifies that the documentation aligns with product requirements and business objectives
- A subject matter expert (typically an engineer) confirms technical accuracy and implementation details
- A peer writer (different from the assigned writer) reviews for style consistency and adherence to documentation standards
- The assigned writer ensures overall quality and completeness

Each approver verifies different aspects of the documentation, from technical accuracy to style and quality.

The docs team can block publication if quality standards are not met. Under extreme circumstances, this can be overridden, but leadership approval is required.

**Variations:**
- Some teams require approval from security, legal, or compliance
- Some teams use a single-approver model for minor updates
- Some teams require customer validation or beta user feedback before publication
- Some teams use automated checks (linting, link validation, accessibility) as part of the approval process

## Accountability and consequences

The product manager is ultimately accountable for ensuring that a feature release has documentation support. This means ensuring the documentation request is created correctly, all required fields are populated, minimum requirements are met, and a first draft is produced on time.

**In this example:**
If the product manager does not follow this process or fails to meet the minimum requirements for writer assignment, there is no guarantee that the release will have documentation support. Because documentation is required for customer-facing releases, this could result in the release being postponed until documentation is ready.

**Variations:**
- Some teams have the engineering manager or technical lead hold accountability
- Some teams have escalation paths to resolve conflicts (e.g., leadership decision on whether to ship without docs)
- Some teams use metrics or KPIs to track intake process compliance
- Some teams have consequences for repeated non-compliance (e.g., reduced docs support priority for future releases)

## Handling exceptions and edge cases

**Urgent or emergency releases:**
- For security patches or critical bug fixes, the docs team may accept incomplete requests with the understanding that documentation will be backfilled within a specified timeframe
- Requires approval from docs team lead and product leadership

**Release date changes:**
- If a release date moves earlier, the product manager must notify the docs team immediately
- If a release date moves later, the updated timeline should be reflected in the documentation request

**Scope changes after writer assignment:**
- Significant scope increases may require renegotiating timelines or writer assignments
- The product manager must notify the assigned writer and docs team lead as soon as scope changes are identified

**Documentation discovered missing after release:**
- If a customer-facing feature ships without documentation, it becomes the highest priority for the docs team
- The product manager must work with the docs team to create the documentation within one week of discovery
