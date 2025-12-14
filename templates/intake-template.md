# Documentation intake template

Use this template to submit a documentation request for a new feature or significant change. Complete this intake form to help the documentation team understand what needs to be documented and plan the work accordingly.

**How to use this template:**

- Complete all sections to provide the documentation team with sufficient context
- Use the examples as a guide for the level of detail expected in each section
- Delete checklist items from the Documentation scope section that don't apply to your feature
- For detailed guidance, refer to the [Documentation intake process](../docs/intake-process.md)
- See example intakes: [medium complexity](../examples/sample-intake.md) | [high complexity](../examples/sample-intake-high-complexity.md)

---

## Feature summary

Write 1-3 sentences describing what the feature does and how users will interact with it. Frame from the user's perspective and mention all interfaces (dashboard, API, CLI, etc.).

Example: "Health monitoring lets administrators see which services are online, how much traffic they're handling, and whether they're configured correctly. Administrators access this information through the dashboard and the API."

## Terminology

Define standard terms and usage conventions for this feature. Include new terms introduced by the feature, existing terms used in new ways, or terms requiring specific capitalization, formatting, or article usage. Document both technical terms and customer-facing language.

| Term | Usage notes |
|------|-------------|
| term name, `code_format` | Specify: capitalization rules, singular vs. plural, hyphenation, when to use code formatting, preferred articles (a/an/the), and alternative terms to avoid. Example: "health check - Lowercase unless at the beginning of a sentence. Two words, not hyphenated. Don't call it 'status check' or 'ping.'" |
| term name | Add rows as needed for each term that requires definition or usage guidance. |

## Documentation scope

This section defines what users need to know to successfully understand, configure, and use the feature. Delete checklist items that don't apply and add specific details for items that remain.

### What users need to know

This subsection covers foundational concepts users need before working with the feature.

- Core concepts: what the feature is and how it works
  - Add details about the key mental models users need to develop
- Why users would use this: primary use cases and benefits
  - Include motivating scenarios or problems this feature solves
- Additional conceptual information (if applicable):
  - How components interact or relate to existing systems
  - Architecture or design considerations users should understand
  - Contact information for subject matter experts who can provide architectural review

### Requirements

This subsection documents prerequisites and constraints that must be satisfied before using the feature.

- Permissions: roles or specific permissions required to access the feature
  - Include role names and any special access controls
  - Document service account or API authentication requirements if applicable
- Plan: subscription tiers or pricing plans that include this feature
  - Contact information for sales enablement or product marketing teams if messaging coordination is needed
- Prerequisites: required services, configurations, or features that must be enabled first
  - List dependencies in the order they should be configured
  - Note any caveats about configuration sequence or integration requirements
- Version requirements (if applicable): minimum platform versions or version compatibility constraints
  - Document any breaking changes or migration requirements between versions

### Limitations

This subsection clarifies constraints, unsupported scenarios, and known issues.

- Technical constraints and capacity limits
  - Include: size limits, rate limits, timeout values, retention periods
  - Specify: maximum supported values, concurrent operation limits
  - Document any performance implications users should be aware of
- Unsupported scenarios or use cases
  - Clarify what the feature does not support
  - Include workarounds where available
- Known issues
  - Describe symptoms and impact
  - Include issue tracking numbers if available
  - Document workarounds or mitigation strategies
  - Note expected resolution timeframe or version if known
- Edge cases or boundary conditions
  - Describe unusual scenarios that may produce unexpected results
  - Contact information for engineering teams if technical clarification is needed

### Instructions needed

This subsection outlines procedural documentation required to implement and operate the feature.

- How to enable or configure the feature
  - Include initial setup or registration steps
  - Document configuration options and their effects
- How to perform common operations or workflows
  - List the primary tasks users will need to accomplish
  - Include step-by-step procedures for each workflow
- How to integrate with other systems (if applicable)
  - Document integration points and configuration requirements
- How to monitor, maintain, or manage the feature over time (if applicable)
  - Include operational procedures and best practices
- How to update, migrate, or roll back (if applicable)
  - Document upgrade paths and rollback procedures
- How to disable or archive (if applicable)
  - Include cleanup or decommissioning procedures

### Reference documentation

This subsection catalogs technical reference material for syntax, parameters, and return values.

- API endpoints (if applicable)
  - List HTTP methods and paths (e.g., `GET /api/v1/resource/{id}`)
  - Include request/response schemas and authentication requirements
  - Document error responses and status codes
- CLI commands (if applicable)
  - Document command syntax, subcommands, and available flags
  - Include environment variable overrides if supported
- Configuration options (if applicable)
  - Document configuration file formats (`.yaml`, `.json`, etc.)
  - Specify all configuration keys, data types, default values, and valid options
- Environment variables (if applicable)
  - List variable names (e.g., `FEATURE_MODE`), purpose, and valid values
  - Document defaults and precedence rules
- Error codes or messages (if applicable)
  - Catalog error codes with descriptions and resolution guidance
- Data schemas or structures (if applicable)
  - Document data models, schemas, or object structures
- Built-in functions, attributes, or syntax (if applicable)
  - For features introducing custom syntax or expression languages
  - Contact information for language/syntax specification owners

### Troubleshooting

This subsection helps users diagnose and resolve common problems.

- What to do when common failures occur
  - Include symptoms, diagnostic steps, and resolutions
- How to debug issues or gather diagnostic information
  - Document debugging tools, flags, or procedures
- How to identify and resolve performance problems (if applicable)
  - Include metrics to monitor and threshold recommendations
- How to resolve conflicts or validation errors (if applicable)
  - Document common validation failures and their causes

## New topics needed

List new documentation topics that must be created. For each topic, specify the topic type (conceptual, tutorial, how-to, reference, troubleshooting) and what it should cover. Include priority level and any subject matter expert contacts if available.

Example format:

- Topic title (type): brief description of what the topic covers
  - Priority: High/Medium/Low
  - Contact @subject-matter-expert for technical review

If no new topics are needed, write: "None - updates to existing topics only."

## Existing topics to update

List existing documentation topics that need updates. For each topic, describe what changes are required and why.

Example format:

- Topic title: description of what needs to be added, modified, or removed
  - Contact information for reviewers if cross-team coordination is needed

If no existing topics need updates, write: "None - new topics only."

## Complexity estimate

**Level:** Low / Medium / High

**Reasoning:** Explain your assessment based on these criteria:

- **Terminology:** Does this feature introduce new terms that users must learn? How many? Are concepts fundamentally new or extensions of familiar ideas?
- **Interfaces:** How many different interfaces (dashboard, API, CLI, configuration files, etc.) does the feature involve? Do users need to coordinate actions across multiple interfaces?
- **Components:** How many separate components or systems must be configured? Do they have dependencies or required configuration order?
- **Syntax:** Does this feature introduce new syntax, expression languages, or domain-specific languages users must learn?
- **Documentation impact:** How many new topics are required? How many existing topics need updates?
- **Technical depth:** Does this feature involve complex technical concepts that require detailed explanation?

See the [complexity framework documentation](../docs/feature-documentation.md) for detailed guidance on estimating complexity.
