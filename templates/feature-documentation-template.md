# Feature documentation template

Use this template to define feature documentation requirements for your organization. This template helps you establish clear standards for what content must be included in feature documentation, how it should be structured, and who is responsible for creating and maintaining it.

**How to use this template:**

- Replace example content with your organization's specific requirements and terminology
- Adapt sections to match your product development workflow and release processes
- Modify role responsibilities to reflect your team structure
- Adjust release stage terminology (e.g., "early access" and "generally available") to match your product lifecycle
- Remove or add sections based on your product's technical characteristics (APIs, CLI tools, UI features, etc.)
- For detailed guidance and context, refer to:
  - [Feature documentation requirements](../docs/feature-documentation.md)
  - [Sample feature documentation requirements](../examples/sample-feature-documentation.md)

---

## Overview

This document defines requirements for documenting product features at different release stages. It establishes what content must be included, how it should be structured, and who is responsible for creating and maintaining it.

Replace this paragraph with a brief overview customized to your organization's documentation philosophy and goals.

## Customization guidance

When adapting this template for your organization:

- **Release stage terminology:** Replace "early access" and "generally available" with your own release stage terminology (alpha, beta, preview, experimental, GA, etc.)
- **Content requirements:** Adjust content requirements to match your product's technical characteristics. For example:
  - API-focused products should emphasize endpoint documentation, request/response schemas, and authentication details
  - CLI-focused products should emphasize command syntax, flags, and examples
  - UI-focused products should emphasize screenshots, workflow descriptions, and settings explanations
  - Platform products may need all of the above
- **Role responsibilities:** Modify role responsibilities to reflect your team structure (product managers, technical writers, documentation engineers, developer advocates, etc.)
- **Lead times:** Define appropriate lead times based on your release cadence and team capacity
- **Format requirements:** Adapt format requirements to your documentation platform and structure (single vs. multi-page, navigation systems, search requirements)
- **Complexity framework:** If your organization uses a complexity estimation framework, reference it in the timing section

## What is a feature guide?

A feature guide is documentation that provides everything a user needs to know about a feature. The structure and depth of a feature guide depends on the feature's release stage. Feature guides evolve through distinct documentation stages as the feature matures.

Replace the subsections below with your organization's release stage definitions.

### Early access documentation

Early access documentation is a single, self-contained topic that provides everything a user needs to know about a feature in the early access stage. Because early access features are experimental and evolving, the documentation must be focused, practical, and easy to update as the feature changes.

Early access documentation may be "hidden" (not appearing in navigation or search results) to allow controlled distribution to early testers while keeping experimental features from appearing in general documentation.

**Characteristics:**

- Single, self-contained topic for rapid iteration
- Focused on getting started rather than comprehensive coverage
- May be hidden from general navigation and search
- Clear stability indicators so users know what to expect
- Lightweight maintenance requirements as the feature evolves

### Generally available documentation

As a feature matures and becomes generally available, the documentation evolves from a single topic into a properly structured set of documentation. This typically includes how-to guides, reference documentation, conceptual explanations, and troubleshooting content organized according to your documentation structure.

**Characteristics:**

- Multiple topics organized by information type (concepts, procedures, reference, troubleshooting)
- Comprehensive coverage of all common use cases
- Fully integrated with navigation and search
- Higher quality standards (accuracy, clarity, consistency, completeness)
- Ongoing maintenance as the feature evolves

## When to write feature documentation

Write feature documentation for any release that is customer-facing. If users will interact with the feature in any way, it requires documentation.

The timing for creating documentation depends on the feature's complexity:

- **High complexity features** require more lead time. Start documentation [specify timeframe, e.g., "at least 4 weeks before release"] to allow for thorough review and iteration.
- **Medium complexity features** require moderate lead time. Start documentation [specify timeframe, e.g., "at least 2 weeks before release"].
- **Low complexity features** can be documented closer to the release date. Start documentation [specify timeframe, e.g., "at least 1 week before release"].

For guidance on assessing complexity, refer to [your team's complexity framework or link to complexity documentation].

**Critical requirement:** Documentation must be ready to publish by [specify deadline, e.g., "the day before the feature release" or "the release date"].

### Complexity assessment

Consider these factors when estimating documentation complexity:

- **Technical scope:** How many interfaces, APIs, commands, or configuration options does the feature include?
- **Terminology:** Does the feature introduce new concepts or terminology that require explanation?
- **Integration points:** How many existing features, services, or workflows does this feature interact with?
- **Use case variety:** How many distinct use cases or workflows need to be documented?
- **User audience:** How many different user roles or personas will use this feature?

## Content requirements

Feature documentation must include the following content. Items marked as **Required** must be included in every feature guide. Items marked as **Variable** depend on the feature's technical characteristics. Items marked as **Optional** are encouraged but not required.

Customize these requirements based on your product's technical characteristics and user needs.

### Required

All feature documentation must include:

- **Release stage indicator**
  - Clearly indicate whether the feature is in early access, generally available, deprecated, or another relevant stage
  - Example: Display a banner or badge showing "Early Access" or "Beta"

- **Plan or tier availability**
  - Indicate which pricing plans or tiers have access to the feature (for commercial products)
  - For open source or enterprise products, indicate which deployment configurations or editions support the feature
  - Example: "Available on Enterprise and Pro plans" or "Requires self-hosted deployment"

- **High-level description**
  - Explain what the feature is, how it works, and why the user should care
  - Frame from the user's perspective, focusing on benefits and outcomes
  - Example: "Real-time monitoring displays server health metrics and alerts you when performance degrades, helping you identify issues before they impact users."

- **Use cases**
  - List core use cases for the feature with concrete examples
  - If you're still discovering use cases during early access, describe the feature's intent instead
  - Example: "Use real-time monitoring to: detect memory leaks before crashes occur, identify slow database queries, track error rates across services"

- **Prerequisites**
  - List what the user needs before using the feature
  - Include permissions, roles, dependencies, required configurations, or other features that must be enabled
  - Example: "Before enabling monitoring, you need: Admin role, PostgreSQL 12 or later, network access to metrics endpoint"

- **How to get started**
  - Provide happy-path instructions for using the feature
  - At minimum, include a getting started guide
  - For complex features, also provide how-to guides for additional tasks
  - Use clear, step-by-step instructions with expected outcomes

- **Limitations and known issues**
  - List current limitations (what the feature cannot do or does not support)
  - Document known issues with workarounds where available
  - Set clear expectations about what the feature can and cannot do
  - Example: "Monitoring does not currently support: custom metrics from third-party services, alerting via SMS, retention beyond 30 days"

### Variable

Include the following content when applicable to your feature:

- **Terminology and concepts**
  - If the feature introduces new terminology or concepts, explain them clearly
  - Describe how new terms connect to existing terminology, concepts, and features
  - Provide definitions that help users understand the mental model
  - Example: "A 'health check' is an automated test that verifies a service is responding correctly. Health checks run every 30 seconds and report status to the dashboard."

- **Reference documentation**
  - Include reference documentation appropriate to your feature's technical characteristics
  - **CLI command syntax and examples:** Document all commands, subcommands, flags, and arguments
  - **Environment variables:** List variable names, expected values, defaults, and what they control
  - **Configuration file schemas:** Provide schema documentation and annotated examples
  - **API endpoints:** Document HTTP methods, paths, request/response formats, authentication requirements, and error codes
  - **UI elements:** Document settings, controls, and their functions

### Optional

Include the following content when it adds significant value:

- **Examples**
  - Include one or two examples that cover core use cases
  - Provide complete, runnable examples with instructions
  - Include any necessary commands, configuration files, or implementation details
  - Example: "Setting up monitoring for a Node.js application" with complete code and configuration

- **Feedback instructions**
  - Include instructions for how users can provide feedback, report bugs, or contact the team
  - This is particularly valuable during early access when actively gathering user input
  - Example: "Share feedback on this feature in our [community forum](link) or contact <support@example.com>"

## Format requirements

Feature documentation format requirements differ based on the feature's release stage. Early access documentation prioritizes simplicity and rapid iteration, while generally available documentation requires comprehensive structure and organization.

Customize these format requirements to match your documentation platform and workflow.

### Early access documentation format

Documentation for features in early access should follow these format requirements:

- **Single, self-contained topic**
  - All content must be in a single documentation topic
  - Unlike generally available documentation, early access documentation should not be split across multiple topics
  - This enables rapid updates without navigating complex topic structures

- **Marked as hidden (if applicable)**
  - The topic may be marked as hidden so it doesn't appear in navigation or search results
  - This allows controlled distribution to early testers
  - Specify your platform's mechanism for hiding content (metadata, unlisted URLs, authentication gates, etc.)

- **Focused on getting started**
  - Content should prioritize helping users get started quickly
  - Document the happy path and core use cases
  - Avoid documenting every possible configuration or edge case
  - Save comprehensive coverage for general availability

- **Clear expectations about stability**
  - Documentation should make it clear that the feature is experimental and may change
  - Include appropriate disclaimers about API stability, feature completeness, or support limitations
  - Example: "This feature is in early access. APIs and behavior may change in future releases. See our [versioning policy](link) for details."

### Generally available documentation format

Documentation for features in general availability should follow these format requirements:

- **Properly categorized**
  - Documentation should be organized according to your documentation structure
  - Separate content by information type: concepts, how-to guides, reference, troubleshooting
  - Follow your organization's information architecture and navigation patterns
  - Example structure: Concepts → Getting Started → How-to Guides → API Reference → Troubleshooting

- **Linked from navigation**
  - Documentation should appear in appropriate navigation menus
  - Content must be discoverable via search
  - Include cross-references to related features and topics
  - Ensure proper metadata for categorization and discovery

- **Comprehensive coverage**
  - Documentation should cover all common use cases, not just the happy path
  - Include configuration options, troubleshooting guidance, and examples
  - Address known limitations and edge cases
  - Provide reference documentation for all APIs, commands, or configuration options

- **Quality standards**
  - Content must meet your organization's quality standards for accuracy, clarity, consistency, and completeness
  - Follow established style guidelines and terminology conventions
  - Include code examples that are tested and runnable
  - Provide clear, actionable instructions with expected outcomes

## Responsibilities

Documentation responsibilities are shared between product managers and the docs team, with clear accountability for each role. The product manager owns content accuracy and completeness, while the docs team ensures quality and consistency.

Customize these responsibilities to reflect your organization's team structure and workflow.

### Product manager responsibilities

The product manager is accountable for feature documentation. This means:

- **Ensuring initial documentation is created**
  - You may write it yourself or delegate to an engineer, subject matter expert, or another team member
  - Contact the docs team early to discuss complexity, timeline, and resource needs
  - Provide all necessary information (technical details, use cases, limitations, examples)

- **Ensuring documentation accuracy**
  - Documentation must accurately reflect the current state of the feature
  - Verify technical accuracy before submitting for review
  - Validate examples and instructions against the actual feature behavior

- **Managing documentation updates**
  - Ensure documentation is updated when the feature changes
  - Create work items for all updates and communicate changes to the docs team
  - Notify the assigned writer promptly if significant changes occur during development

- **Working with the docs team**
  - Address feedback during the review process
  - Respond to questions and requests for clarification within agreed-upon timelines
  - Participate in reviews and approve documentation for release

- **Planning and timing**
  - Determine appropriate lead time based on feature complexity
  - Ensure documentation is ready by the required deadline
  - Alert stakeholders if documentation blockers threaten release timelines

### Docs team responsibilities

The docs team is responsible for:

- **Reviewing documentation**
  - Work with the author to get documentation ready to publish
  - Provide feedback within agreed-upon SLAs (specify your team's SLA)
  - Conduct iterative reviews as needed until documentation meets quality standards

- **Peer review**
  - Conduct peer reviews for style, grammar, and quality
  - Ensure documentation follows style guidelines and terminology standards
  - Validate structure, clarity, and completeness

- **Maintaining quality and consistency**
  - Ensure documentation meets quality standards across all features
  - Identify related documentation requiring updates or cross-references
  - Maintain consistency in terminology, formatting, and structure

- **Structuring and organization**
  - Provide guidance on how to structure documentation
  - Plan restructuring when features transition from early access to generally available
  - Ensure documentation fits appropriately within existing information architecture

### Accountability

The product manager is ultimately accountable for feature documentation. This means ensuring the documentation exists, meets requirements, and is approved for release by the release date. The docs team is accountable for the quality of their reviews and providing timely feedback.

**Important:** If documentation isn't ready by the release date, [specify your organization's policy - e.g., "the release may be postponed" or "the feature cannot be announced until documentation is complete"].

## Maintaining documentation during early access

Between the initial release and general availability, feature documentation changes as necessary to reflect the current state of the feature. The feature is expected to evolve, and the documentation must evolve with it.

During the early access stage:

- **Product manager accountability**
  - The product manager remains accountable for ensuring documentation accurately reflects the feature
  - Monitor feature changes and proactively identify documentation updates needed
  - Communicate updates to the docs team through [specify your communication mechanism, e.g., "the cross-functional sync meeting" or "Slack channel"]

- **Update process**
  - Engineers, product managers, and other authors can update documentation as often as needed
  - Notify the assigned writer of any significant changes
  - All updates follow the same review process as the initial draft
  - Create work items for tracking updates (link them to the original documentation request)

- **Writer involvement**
  - The assigned writer identifies related documentation that may need updates or cross-references
  - Writers provide ongoing support and review for updates
  - Writers monitor documentation quality and flag issues proactively

- **Handling feature pivots**
  - Feature pivots are expected during early access
  - While pivots rarely require starting documentation from scratch, they may require substantial revisions
  - If significant changes occur, notify the assigned writer promptly
  - For guidance on handling changes after documentation is in progress, refer to [your team's change management protocol or link to last-minute changes documentation]

## Transitioning to generally available

As the feature approaches general availability, the docs team begins planning how to restructure the single early access topic into properly categorized documentation. The product manager continues to own content creation, but the docs team takes a more active role in structuring and organizing the documentation.

### Transition planning

Specify your organization's process for transitioning documentation from early access to generally available:

- **Trigger for transition**
  - What event triggers the documentation transition? (e.g., "feature moves from beta to GA" or "product manager requests GA transition")

- **Planning responsibility**
  - Who plans the restructuring? (e.g., "docs team leads planning with input from PM" or "collaborative planning between PM and docs team")

- **Timeline**
  - When does restructuring occur? (e.g., "restructuring begins [X weeks] before GA release" or "restructuring happens during GA documentation sprint")

- **Scope of changes**
  - What changes are required? Common changes include:
    - Splitting single topic into multiple topics organized by information type
    - Adding comprehensive reference documentation
    - Expanding examples and use cases
    - Adding troubleshooting content
    - Updating navigation and cross-references
    - Removing early access disclaimers and updating release stage indicators

### Ownership after general availability

By general availability, the docs team fully owns the documentation, with the product manager serving as a subject matter expert for updates.

Specify how ongoing maintenance works after GA:

- **Docs team ownership**
  - Docs team maintains documentation accuracy and quality
  - Docs team plans and executes updates as features evolve
  - Docs team coordinates with product managers and engineers for technical accuracy

- **Product manager involvement**
  - Product managers provide subject matter expertise for updates
  - Product managers review documentation changes for accuracy
  - Product managers communicate upcoming feature changes that require documentation updates

- **Update process**
  - Specify how updates are requested and tracked after GA
  - Define review and approval workflows
  - Establish SLAs for updates based on urgency

---

## Customization checklist

When adapting this template for your organization, ensure you've customized:

- [ ] Release stage terminology (early access, generally available, etc.)
- [ ] Content requirements to match your product's technical characteristics
- [ ] Role titles and responsibilities to reflect your team structure
- [ ] Documentation lead times based on your release cadence
- [ ] Format requirements to match your documentation platform
- [ ] Links to your complexity framework, style guide, or other reference documentation
- [ ] Communication mechanisms (sync meetings, Slack channels, ticketing systems)
- [ ] SLAs for reviews and feedback
- [ ] Consequences for missing documentation deadlines
- [ ] Transition process from early access to generally available
- [ ] Ongoing maintenance workflows after general availability
