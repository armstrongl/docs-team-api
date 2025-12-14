# Sample glossary

This example demonstrates how a docs team might structure a shared glossary of terms for collaboration with product and engineering teams. Your glossary should define terms that are commonly used in your team's workflow but may have ambiguous or varying interpretations.

## Example terms

**Code complete:** Code complete occurs when feature code is merged and deployed (possibly behind a feature flag). Bugs can be fixed after this point, but major functionality is complete. Changes after code complete should not affect documentation scope.

**Cross-functional sync:** A recurring meeting to review all launches for the current period. This includes product and engineering releases. Attendees typically include the docs team, product team, and engineering managers.

**Documentation plan:** A section in the project document for a launch. It must meet the documentation plan requirements defined by the docs team's process.

**Docs work item:** A work item (epic, ticket, or project) for the documentation work related to a product launch. It should exist under the parent launch work item in your project management system.

**Early access:** A release stage where a feature is available to a limited set of users for testing and feedback before general availability. Documentation is typically a single, self-contained topic.

**Estimated code complete date:** An estimate of when a feature will be code complete. The engineering manager or tech lead is responsible for this estimate.

**Estimated launch date:** An estimate of when a feature will launch. The product manager is responsible for this estimate. It depends on the estimated code complete date.

**Feature flag:** A mechanism that allows code to be deployed but not visible to users until the flag is enabled. Enables separating code deployment from feature launch.

**Generally available (GA):** A release stage where a feature is fully released to all users. Documentation is comprehensive and properly categorized.

**Hidden documentation:** Documentation that exists but does not appear in navigation or search results. Used for early access features to enable controlled distribution.

**Launch:** A feature is launched when announced to users. This typically involves publishing documentation, a changelog, and marketing communications.

**Parent initiative:** Your product team's work item (for example, a Jira epic, Linear project, or Azure DevOps feature) for a feature launch.

**Project document:** The collaborative source of truth for information about a project (typically a feature launch). It contains sections for different teams to complete. Use a template to maintain consistency without making it cumbersome for stakeholders.

**Release:** A feature is released when code is complete. The functionality might be hidden behind a feature flag until launch. Code is considered live when deployed to production.

**SME (subject matter expert):** A person with deep knowledge of a specific feature or system, typically an engineer. Provides technical accuracy review for documentation.

**Team API:** A documented interface that defines how other teams interact with a team. It specifies what information is required for requests (input contracts), what the team delivers (output contracts), timing expectations (SLAs), and what happens when something goes wrong (error handling). The goal is to make implicit collaboration patterns explicit.

## Variations by organization type

Different organizations may need to adapt these terms:

### SaaS company

- May distinguish between **deployment** (code in production) and **release** (feature visible to users)
- Often uses **beta** instead of or in addition to early access
- May have multiple GA stages (GA for specific plan tiers)

### Enterprise software company

- May use **limited availability** instead of early access
- Often distinguishes between **on-premises release** and **cloud release**
- May include terms for **maintenance releases** vs **feature releases**

### Developer tools or API company

- May use **preview** or **experimental** for pre-GA features
- Often includes terms for **API versioning** and **deprecation timelines**
- May distinguish between **client library release** and **API endpoint release**

### Platform or infrastructure company

- May use **rollout** to describe gradual feature deployment
- Often includes terms for **region availability** and **rollback procedures**
- May distinguish between **control plane updates** and **data plane updates**
