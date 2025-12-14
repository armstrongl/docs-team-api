# Sample intake: Policy Engine feature

This example shows a completed documentation intake for a fictional high-complexity feature. Use it as a reference when completing documentation requests for features that introduce new syntaxes, affect multiple systems, or require coordinating actions across multiple interfaces.

---

## Feature summary

Policy Engine lets administrators define sophisticated access control rules that evaluate user attributes, resource metadata, and contextual conditions in real time. Administrators write policies using the Policy Definition Language (PDL), deploy them through the CLI or API, test them in the policy simulator, monitor enforcement through the dashboard, and audit decisions through structured logs. Policies can control access to services, data objects, API endpoints, and administrative functions.

## Terminology

| Term | Usage notes |
|------|-------------|
| Policy Engine | Capitalize both words. Refers to the entire subsystem, not individual policies. Don't abbreviate as "PE." |
| policy | Lowercase (unless at the beginning of a sentence) when referring to an individual rule document. Don't call it "rule," "permission," or "access control." |
| Policy Definition Language | Capitalize all words. Use the full name on first reference, then "PDL" for subsequent mentions. Don't call it "policy syntax" or "rule language." |
| policy evaluation | Lowercase unless at the beginning of a sentence. Two words, not hyphenated. The process of executing a policy against a request. Don't call it "policy execution" or "policy check." |
| evaluation context | Lowercase unless at the beginning of a sentence. The set of attributes, metadata, and conditions available during policy evaluation. Don't call it "request context" or "policy context." |
| policy set | Lowercase unless at the beginning of a sentence. Two words, not hyphenated. A collection of related policies that are evaluated together. Don't call it "policy group" or "ruleset." |
| principal | Lowercase unless at the beginning of a sentence. The entity making a request (user, service account, or API key). Don't call it "actor," "subject," or "requester." |
| resource | Lowercase unless at the beginning of a sentence. The entity being accessed (service, data object, API endpoint, or configuration). Don't call it "target" or "object." |
| effect | Lowercase unless at the beginning of a sentence. The outcome of a policy evaluation (`allow` or `deny`). Don't call it "result," "decision," or "verdict." |
| condition | Lowercase unless at the beginning of a sentence. A logical expression in a policy that must evaluate to `true` for the policy to apply. Don't call it "constraint," "predicate," or "requirement." |
| policy simulator | Lowercase unless at the beginning of a sentence. Two words, not hyphenated. The testing interface where administrators validate policies before deployment. Don't call it "policy tester" or "sandbox." |
| `policy deploy` | Lowercase, one word with space. CLI command to deploy policies to the system. Don't hyphenate or use camelCase. Always use code formatting. |
| `policy export` | Lowercase, one word with space. CLI command to export policies from the system. Don't hyphenate or use camelCase. Always use code formatting. |
| `policy rollback` | Lowercase, one word with space. CLI command to revert to a previous policy version. Don't hyphenate or use camelCase. Always use code formatting. |
| `policy_decision` | Lowercase, one word with underscore. Audit log event type for recording policy evaluation outcomes. Don't hyphenate or use camelCase. Always use code formatting. |

## Documentation scope

This section defines the full scope of documentation required for Policy Engine, organized by content type and user need.

### What users need to know

- Core concepts: what Policy Engine is, how it differs from role-based access control, and when to use it
  - Contact @sarah-iam for architectural diagrams and conceptual review
- Why users would use this: fine-grained access control, compliance requirements, conditional access based on context
  - Include real-world scenarios from the beta program; contact @beta-feedback for examples
- How policy evaluation works: evaluation order, precedence rules, default behavior when no policy matches
  - Caveat: default deny behavior changed in v3.2; document migration path from v3.1
- How PDL relates to other configuration formats (`JSON`, `YAML`) and when to use each
  - PDL is required for complex conditions; `JSON`/`YAML` only support static policies
- Security considerations: policy testing best practices, avoiding overly permissive policies, auditing policy changes
  - Contact @security-team for compliance review before publishing

### Requirements

- Permissions: Admin role required to create and deploy policies; Auditor role can view policies and audit logs
  - Service accounts require the `policy:write` scope for programmatic deployment
- Plan: Available on Enterprise plan only
  - Contact @sales-enablement for upgrade messaging and feature comparison
- Prerequisites: At least one service configured; identity provider integration configured for attribute-based policies
  - Caveat: SAML providers require attribute mapping configuration before Policy Engine can access user attributes
- Version requirements: Requires platform version 3.2 or later; PDL syntax version compatibility matrix
  - Document breaking changes between PDL v1 and v2 syntax

### Limitations

- Policy evaluation adds 10-50ms latency to requests depending on policy complexity
  - Contact @platform-perf for benchmark data and optimization guidance
- Maximum policy size: 256KB per `.pdl` file
- Maximum policies per policy set: 100 policies
  - Workaround: use nested policy sets for larger deployments
- Maximum evaluation depth: 10 nested conditions
  - Caveat: deeply nested conditions significantly impact evaluation performance
- Audit logs retained for 90 days; longer retention requires export to external storage
  - Document integration with supported SIEM providers
- Known issue: policy simulator does not support testing time-based conditions with custom time zones
  - Tracked in `ISSUE-4521`; expected fix in v3.4
- Known issue: policy changes may take up to 60 seconds to propagate across all nodes in distributed deployments
  - Contact @infrastructure for cache invalidation details

### Instructions needed

- How to enable Policy Engine for an organization
  - Requires org admin permissions; document the enablement workflow in the dashboard
- How to write a basic policy in PDL
  - Include a "Hello World" example that grants read access to a single resource
- How to define principals, resources, and conditions
  - Document all supported principal types: users, service accounts, API keys, and groups
- How to test a policy in the policy simulator
  - Include example test cases with expected outcomes
- How to deploy a policy using the CLI
  - Document the `policy deploy` command with common flags
- How to deploy a policy using the API
  - Include `curl` examples and SDK snippets
- How to organize policies into policy sets
  - Recommend naming conventions and organizational patterns
- How to configure policy evaluation order and precedence
  - Caveat: explicit deny always overrides allow; document this behavior clearly
- How to monitor policy evaluation metrics in the dashboard
  - Document key metrics: evaluation latency, cache hit rate, denial rate
- How to query audit logs for policy decisions
  - Include sample queries for common troubleshooting scenarios
- How to export policies for version control
  - Document the `policy export` command and recommended Git workflows
- How to import policies from version control
  - Include CI/CD integration examples
- How to update an existing policy without downtime
  - Document the blue-green deployment pattern for policy updates
- How to roll back a policy deployment
  - Document the `policy rollback` command and rollback limitations
- How to disable or archive a policy without deleting it
  - Caveat: archived policies still count toward the policy set limit

### Reference documentation

- PDL syntax specification: complete language reference with grammar, operators, functions, and data types
  - Contact @pdl-lang-team for grammar file and syntax highlighting definitions
- Built-in functions: string manipulation, date/time operations, array operations, cryptographic functions
  - Document function signatures with parameter types and return values
- Built-in attributes: user attributes, service attributes, request metadata, environmental attributes
  - Include the complete attribute namespace hierarchy
- CLI commands: `policy create`, `policy deploy`, `policy test`, `policy list`, `policy delete`, `policy export`, `policy import`
  - Document all flags and environment variable overrides
- API endpoints: `POST /api/v1/policies`, `PUT /api/v1/policies/{policy_id}`, `GET /api/v1/policies`, `DELETE /api/v1/policies/{policy_id}`, `POST /api/v1/policies/simulate`
  - Include request/response schemas and error responses
- Configuration file format: policy manifest structure, policy set configuration, evaluation engine configuration
  - Document the `policy.yaml` manifest schema
- Environment variables: `POLICY_ENGINE_MODE`, `POLICY_CACHE_TTL`, `POLICY_AUDIT_LEVEL`
  - Document default values and valid options for each variable
- Error codes: policy syntax errors (`PDL-1xxx`), evaluation errors (`PDL-2xxx`), deployment errors (`PDL-3xxx`)
  - Include resolution guidance for each error code
- Audit log schema: decision records, evaluation traces, performance metrics
  - Document the `policy_decision` event structure and queryable fields

### Troubleshooting

- What to do when a policy denies access unexpectedly
  - Include steps to retrieve the evaluation trace from audit logs
- How to debug complex condition logic
  - Document the `--dry-run` flag for `policy test`
- What to do when policy evaluation times out
  - Document the `POLICY_EVAL_TIMEOUT` configuration and optimization strategies
- How to identify performance bottlenecks in policy evaluation
  - Include dashboard metrics to monitor and threshold recommendations
- What to do when policy deployment fails validation
  - Document common validation errors and their resolutions
- How to resolve conflicts between multiple policies
  - Document the precedence algorithm and conflict detection tools
- What to do when the policy simulator produces different results than production
  - Caveat: simulator uses cached attribute data; document refresh procedures

## New topics needed

The following new documentation topics are required to fully cover Policy Engine functionality.

- Policy Engine overview (conceptual): explains the architecture, evaluation flow, and how Policy Engine fits into the broader access control system
  - Priority: High; prerequisite for all other Policy Engine topics
  - Contact @sarah-iam for architecture review
- Policy Engine quickstart (tutorial): walks through writing, testing, and deploying a first policy
  - Priority: High; primary onboarding path for new users
- Policy Definition Language specification (reference): complete PDL syntax reference with examples
  - Priority: High; required for any policy authoring
  - Contact @pdl-lang-team for grammar specification and syntax railroad diagrams
- Policy best practices (guide): patterns for writing maintainable policies, security considerations, performance optimization
  - Include lessons learned from beta customers
- Write a policy (how-to): step-by-step instructions for creating policies in PDL
  - Include templates for common access patterns
- Test a policy (how-to): using the policy simulator to validate policy behavior
  - Include guidance on creating comprehensive test suites
- Deploy a policy with the CLI (how-to): command-line workflow for policy deployment
  - Document `policy deploy`, `policy validate`, and related commands
- Deploy a policy with the API (how-to): programmatic policy deployment
  - Include code samples for Python, Go, and JavaScript SDKs
- Organize policies into policy sets (how-to): structuring related policies for easier management
  - Include recommended organizational patterns by use case
- Monitor policy evaluation (how-to): using the dashboard to track policy metrics and identify issues
  - Document the metrics dashboard panels and alert configuration
- Audit policy decisions (how-to): querying audit logs to understand access decisions
  - Include sample queries for common investigation scenarios
- Manage policy lifecycle (how-to): versioning, updating, and rolling back policies
  - Document Git integration and CI/CD workflows
- Policy Engine CLI reference: complete command documentation
  - Auto-generate from CLI source; contact @cli-team for generation scripts
- Policy Engine API reference: complete endpoint documentation with request/response schemas
  - Auto-generate from OpenAPI spec; contact @api-team for spec location
- Policy Engine configuration reference: configuration file format and environment variables
  - Document `policy.yaml` schema and all `POLICY_*` environment variables
- Policy Engine error reference: error codes and resolution guidance
  - Organize by error code prefix: `PDL-1xxx`, `PDL-2xxx`, `PDL-3xxx`
- Troubleshoot policy evaluation (troubleshooting): common issues and diagnostic techniques
  - Include decision tree for common failure modes

## Existing topics to update

The following existing topics require updates to incorporate Policy Engine content.

- Access control overview: add section explaining how Policy Engine extends role-based access control and when to use each approach
  - Contact @sarah-iam for positioning guidance
- Dashboard overview: add section on the policy evaluation metrics panel and policy management interface
  - Include screenshots of the new Policy Engine dashboard sections
- API reference index: add links to new Policy Engine endpoints
  - Add entries for `/api/v1/policies` and `/api/v1/policies/simulate`
- CLI reference index: add links to new `policy` commands
  - Add entries for `policy create`, `policy deploy`, `policy test`, etc.
- Configuration reference index: add links to Policy Engine configuration options
  - Add entries for `policy.yaml` and `POLICY_*` environment variables
- Audit logging guide: add section on policy decision audit logs and how to query them
  - Document the `policy_decision` event type and queryable fields
- Service configuration guide: add section on enabling Policy Engine for a service
  - Document the `policy_enabled` configuration flag
- Identity provider integration guide: add section on attribute mapping for attribute-based policies
  - Document SAML and OIDC attribute mapping requirements
- Security best practices: add section on policy security considerations and testing strategies
  - Contact @security-team for review before publishing
- Performance tuning guide: add section on optimizing policy evaluation performance
  - Include benchmarks and optimization recommendations
- Version compatibility matrix: add Policy Engine and PDL version requirements
  - Document PDL v1 vs v2 syntax compatibility
- Enterprise plan features: add Policy Engine to the feature comparison table
  - Contact @sales-enablement for feature messaging

## Complexity estimate

**Level:** High

**Reasoning:** This feature meets multiple criteria for high complexity:

1. **New terminology and concepts:** Introduces 10+ new terms (Policy Engine, PDL, policy evaluation, evaluation context, policy set, principal, resource, effect, condition, policy simulator) that must be carefully defined and consistently used. Introduces a fundamentally new way of thinking about access control that extends beyond the existing role-based model.

2. **New syntax:** Introduces PDL, a complete domain-specific language for defining policies. Users must learn PDL syntax, operators, functions, data types, and evaluation semantics. This requires comprehensive reference documentation and multiple tutorial/how-to topics.

3. **Multiple interfaces:** Requires coordinating actions across five distinct interfaces: writing policies in PDL (new syntax), testing in the policy simulator (dashboard), deploying via CLI or API, monitoring evaluation metrics in the dashboard, and querying audit logs. Each interface has its own learning curve.

4. **Multiple components:** Involves configuring the Policy Engine itself, individual services that enforce policies, identity providers for attribute-based policies, audit logging for policy decisions, and version control for policy management. These components must be configured in a specific order with dependencies between them.

5. **Extensive documentation updates:** Affects 11 existing documentation topics spanning access control, dashboard, API, CLI, configuration, audit logging, service configuration, identity integration, security, performance, and version compatibility. Requires careful coordination to maintain consistency across all topics.

6. **Technical depth:** Policy evaluation order, precedence rules, performance implications, and distributed deployment considerations add significant conceptual complexity that must be clearly explained.

This feature requires 17 new topics and updates to 12 existing topics, making it one of the most documentation-intensive features in this release cycle.
