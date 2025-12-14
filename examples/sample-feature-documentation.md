# Sample: Feature documentation requirements

This example demonstrates how to define feature documentation requirements for your team. Adapt the structure, terminology, and requirements to match your organization's needs, product development workflow, and release processes.

## Overview

This sample defines requirements for documenting product features at different release stages. It establishes what content must be included, how it should be structured, and who is responsible for creating and maintaining it.

## Customization guidance

When adapting this example:

- Replace "early access" and "generally available" with your own release stage terminology
- Adjust content requirements to match your product's technical characteristics (APIs, CLI tools, UI features, etc.)
- Modify role responsibilities to reflect your team structure
- Define appropriate lead times based on your release cadence
- Adapt format requirements to your documentation platform and structure

## What is a feature guide?

A feature guide is documentation that provides everything a user needs to know about a feature. The structure and depth of a feature guide depends on the feature's release stage. Feature guides evolve through two distinct documentation stages: early access and generally available.

### Early access documentation

Early access documentation is a single, self-contained topic that provides everything a user needs to know about a feature in the early access stage. Because early access features are experimental and evolving, the documentation must be focused, practical, and easy to update as the feature changes.

Early access documentation may be "hidden" (not appearing in navigation or search results) to allow controlled distribution to early testers while keeping experimental features from appearing in general documentation.

### Generally available documentation

As a feature matures and becomes generally available, the documentation evolves from a single topic into a properly structured set of documentation. This typically includes how-to guides, reference documentation, conceptual explanations, and troubleshooting content organized according to your documentation structure.

## When to write feature documentation

Write feature documentation for any release that is customer-facing. If users will interact with the feature in any way, it requires documentation.

The timing for creating documentation depends on the feature's complexity:

- **High complexity features** require more lead time. Start documentation early enough to allow for thorough review.
- **Medium complexity features** require moderate lead time.
- **Low complexity features** can be documented closer to the release date.

For guidance on complexity, refer to your team's complexity framework or estimation system.

In all cases, documentation must be ready to publish by the day before the feature release.

## Content requirements

Feature documentation must include the following content. Items marked as Required must be included in every feature guide. Items marked as Variable depend on the feature. Items marked as Optional are encouraged but not required.

### Required

- **Release stage indicator.** Clearly indicate whether the feature is in early access or generally available.
- **Plan or tier availability.** Indicate which pricing plans or tiers have access to the feature (for commercial products) or which deployment configurations support it (for open source or enterprise products).
- **High-level description.** Explain what the feature is, how it works, and why the user should care.
- **Use cases.** List core use cases for the feature. If you're still discovering use cases during early access, describe the feature's intent instead.
- **Prerequisites.** List what the user needs before using the feature.
- **How to get started.** Provide happy-path instructions for using the feature. At minimum, include a getting started guide. Depending on complexity, you might also need how-to guides for other tasks.
- **Limitations and known issues.** List current limitations and known issues. This sets clear expectations about what the feature can and cannot do.

### Variable

- **Terminology and concepts.** If the feature introduces new terminology or concepts, explain them and describe how they connect to existing terminology, concepts, and features.
- **Reference documentation.** Depending on the feature, you might need reference documentation for commands, environment variables, configuration files, or other technical details.
  - Include CLI command syntax and examples
  - Document all relevant environment variables
  - Provide configuration file schemas or examples
  - Document API endpoints, parameters, and response formats
  - List UI elements and their functions

### Optional

- **Examples.** Include one or two examples that cover core use cases. These should include instructions specific to the example and any corresponding commands, configuration files, or other implementation details.
- **Feedback instructions.** Include instructions for how the user can provide feedback, report bugs, or contact the team with questions. This is particularly valuable during early access when you're actively gathering user input.

## Format requirements

Feature documentation format requirements differ based on the feature's release stage. Early access documentation prioritizes simplicity and rapid iteration, while generally available documentation requires comprehensive structure and organization.

### Early access documentation format

- **Single, self-contained topic.** All content must be in a single documentation topic. Unlike generally available documentation, early access documentation should not be split across multiple topics.
- **Marked as hidden (if applicable).** The topic may be marked as hidden so it doesn't appear in navigation or search.
- **Focused on getting started.** The content should prioritize helping users get started quickly rather than documenting every possible configuration or edge case.
- **Clear expectations about stability.** The documentation should make it clear that the feature is experimental and may change.

### Generally available documentation format

- **Properly categorized.** Documentation should be organized according to your documentation structure (concepts, how-to guides, reference, troubleshooting).
- **Linked from navigation.** Documentation should appear in appropriate navigation menus and be discoverable via search.
- **Comprehensive coverage.** Documentation should cover all common use cases, not just the happy path.

## Responsibilities

Documentation responsibilities are shared between product managers and the docs team, with clear accountability for each role. The product manager owns content accuracy and completeness, while the docs team ensures quality and consistency.

### Product manager responsibilities

The product manager is accountable for feature documentation. This means:

- Ensuring the initial documentation is created (you may write it yourself or delegate to an engineer, SME, or another team member).
  - Contact the docs team early to discuss complexity and timeline
- Ensuring the documentation accurately reflects the current state of the feature.
- Ensuring the documentation is updated when the feature changes.
  - Create work items under the documentation request for all updates
- Working with the docs team to address feedback during the review process.
- Determining appropriate lead time based on complexity.
- Approving the documentation for release.

### Docs team responsibilities

The docs team is responsible for:

- Reviewing the documentation and working with the author to get it ready to publish.
  - Provide feedback within agreed-upon SLAs
- Conducting a peer review for style, grammar, and quality.
- Ensuring the documentation follows style guidelines.
- Providing feedback on structure, clarity, and completeness.
- Maintaining quality and consistency across all documentation.
  - Identify related documentation requiring updates or cross-references

### Accountability

The product manager is ultimately accountable for feature documentation. This means ensuring the documentation exists, meets requirements, and is approved for release by the release date. The docs team is accountable for the quality of their reviews.

**Important:** If documentation isn't ready by the release date, the release may be postponed.

## Maintaining documentation during early access

Between the initial release and general availability, feature documentation changes as necessary to reflect the current state of the feature. The feature is expected to evolve, and the documentation must evolve with it.

During this stage:

- The product manager is accountable for ensuring documentation accurately reflects the feature.
- Engineers, product managers, and other authors can update documentation as often as needed.
  - Notify the assigned writer of any significant changes
- All updates follow the same review process as the initial draft.
- The assigned writer identifies related documentation that may need updates or cross-references.

When updates are needed, the product manager communicates them to the docs team through the cross-functional sync and by creating a work item under the documentation request.

Feature pivots are expected during the early access phase. While these pivots rarely require starting documentation from scratch, the product manager must ensure documentation stays accurate. If significant changes occur, notify the assigned writer promptly. For guidance on handling changes after documentation is in progress, refer to your team's change management protocol.

## Transitioning to generally available

As the feature approaches general availability, the docs team begins planning how to restructure the single early access topic into properly categorized documentation. The product manager continues to own content creation, but the docs team takes a more active role in structuring and organizing the documentation.

By general availability, the docs team fully owns the documentation, with the product manager serving as a subject matter expert for updates.
