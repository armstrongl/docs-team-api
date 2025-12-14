# Documentation plan template

Use this template to complete the documentation plan section of your project document.

**How to use this template:**

- Sections marked **(Required)** must be completed for every feature
- Sections marked **(If applicable)** should be included when relevant to your feature
- Delete any inapplicable checklist items from the Documentation scope section
- For detailed guidance on any section, refer to the [feature documentation requirements](../docs/feature-documentation.md) and the [documentation plan requirements](../docs/documentation-plan.md) document.

---

## Feature summary (Required)

Write 1-2 sentences describing what the feature is and how customers will experience it. Frame from the customer's perspective.

Example: "Health monitoring lets administrators see which components are online, how much traffic they're handling, and whether they're configured correctly. Administrators access this information through the dashboard and the `/api/v1/health` API endpoint."

## Terminology (If applicable)

Include terms the feature introduces, existing terms used in new ways, or terms requiring specific capitalization/formatting. Document both technical terms and customer-facing language to ensure consistent usage across all interfaces.

| Term | Usage notes |
|------|-------------|
| term | Example: "access policy - Lowercase. Two words, not hyphenated. Don't call it 'security policy' or 'device policy.'" |
| term | Include: capitalization, hyphenation, article usage (a/an/the), what NOT to call it |

## Documentation scope (Required)

Delete checklist items that don't apply to your feature. Add specific details for items that remain. This section defines the boundaries of what documentation needs to cover for users to successfully understand, configure, and use the feature.

### What users need to know (Always required)

This subsection covers the foundational understanding users need before working with the feature.

- Core concepts and how the feature works
- Why users would use this feature

### Requirements (If applicable)

This subsection documents access controls, plan limitations, and dependencies that must be satisfied before using the feature.

- Permissions or roles required
  - Include specific permission names or role-based access control (RBAC) requirements
- Plan or tier requirements
  - Specify which subscription tiers or pricing plans include this feature
- Prerequisites and dependencies
  - List required services, configurations, or other features that must be enabled first

### Limitations (If applicable)

This subsection clarifies what the feature cannot do and scenarios where it may not work as expected.

- Constraints and unsupported scenarios
  - Document technical limitations, rate limits, and use cases that are explicitly not supported
- Known issues
  - Include workarounds where available; contact @engineering for issue tracking details
- Edge cases
  - Describe boundary conditions and unusual scenarios that may produce unexpected results

### Instructions needed (Typically required)

This subsection outlines the procedural documentation required for users to implement and operate the feature.

- Setup instructions
  - Cover initial installation, registration, or enablement steps
- Configuration instructions
  - Document all configuration options, including `.yaml`, `.json`, or other config file formats
- Usage instructions
  - Provide step-by-step guidance for common workflows and operations

### Reference documentation (If applicable)

This subsection catalogs technical reference material that users need to look up syntax, parameters, and return values.

- CLI flags or commands
  - Document command syntax, subcommands, and all available flags
- API endpoints
  - List HTTP methods, paths (e.g., `POST /api/v1/resource`), request/response schemas
- Environment variables
  - Specify variable names (e.g., `DATABASE_URL`), expected values, and defaults
- Configuration file syntax
  - Provide schema documentation and example configurations
- Error codes
  - Document error codes, their meanings, and recommended actions

### Troubleshooting (Include if known issues exist)

This subsection helps users diagnose and resolve common problems without requiring support escalation.

- Common problems and solutions
  - Include symptoms, root causes, and step-by-step remediation procedures

## New topics needed (Required)

List new documentation topics that need to be created and what they should cover. If no new topics are needed, write "None - updates to existing topics only."

## Existing topics to update (Required)

List existing documentation topics that need updates and describe the changes required. If no existing topics need updates, write "None - new topics only."

## Complexity estimate (Required)

**Level:** Low / Medium / High

**Reasoning:** Explain your assessment based on terminology, number of interfaces, and number of components. See the complexity framework for guidance.
