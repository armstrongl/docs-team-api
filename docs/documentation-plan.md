# Documentation plan framework

A documentation plan captures the essential information technical writers need to create accurate, complete documentation for a new feature or initiative. This framework guides you in creating documentation plan templates that work for your team's processes and documentation needs.

## What is a documentation plan

A documentation plan is a structured set of information that bridges the gap between feature development and documentation creation. It captures key details about what is being built, how it should be described, and what documentation deliverables are needed.

The documentation plan serves as the initial handoff from feature teams to docs teams. It provides writers with enough context to understand the feature, identify what needs to be documented, and ask informed follow-up questions.

## Why documentation plans matter

Without structured planning information, docs teams face several challenges:

- **Missing context:** Writers lack understanding of what the feature does or why it matters to users.
- **Inconsistent terminology:** Different team members use different names for the same concepts, leading to confusion in documentation.
- **Incomplete coverage:** Important aspects of the feature (limitations, prerequisites, edge cases) are discovered late or missed entirely.
- **Inefficient communication:** Writers spend time hunting down information through ad-hoc conversations instead of focused review.

Documentation plans solve these problems by establishing a single source of truth for planning information. Feature teams invest time upfront to provide clear context, enabling writers to work more efficiently and produce better documentation.

## Core components of a documentation plan

Effective documentation plans typically include the following components. Adapt these to your organization's needs and processes.

### Feature summary

**Purpose:** Help writers quickly understand what they are documenting and why it matters.

The feature summary provides essential context in 1-2 sentences. It should:

- Frame the feature from the user's perspective, not an internal or technical perspective.
- Explain what the feature does and why a user would need it.
- Use language appropriate for customer-facing documentation.

A feature summary is not a complete feature description. It provides enough context for a writer to understand the scope without requiring them to decode internal jargon or track down planning documents.

**Anti-patterns to avoid:**

- Describing internal implementation details instead of user-facing value
- Using internal code names or referring to internal planning documents
- Assuming the reader already understands the context

### Terminology

**Purpose:** Establish consistent language for new concepts, features, or brand names.

The terminology section captures new terms the feature introduces and provides usage guidance. This ensures consistency across all documentation and helps writers understand how to talk about the feature correctly.

**What to include:**

- Terms the feature introduces that do not exist in current documentation
- Existing terms used in new or different ways
- Brand names or product names associated with the feature
- Acronyms or abbreviations users will encounter
- Terms that need specific capitalization or formatting
- Terms that could be confused with similar existing concepts

**Usage guidance to provide:**

For each term, document:

- Correct capitalization (always capitalized, lowercase, title case)
- Formatting (one word, hyphenated, two words)
- Appropriate articles ("a" vs. "an," "the" vs. no article)
- Common mistakes to avoid ("Don't call it...")
- How the term relates to or differs from similar concepts
- Whether acronyms should be spelled out on first use

### Documentation scope

**Purpose:** Define what the documentation must cover to ensure completeness.

The documentation scope helps writers understand the boundaries of their work and ensures critical information is not missed. It lists the specific topics, concepts, and details the documentation needs to address.

**Coverage areas to consider:**

- **Core concepts:** What users need to understand about how the feature works and why they would use it
- **Requirements:** Prerequisites, permissions, plan tiers, dependencies, or configuration needed before use
- **Limitations:** Constraints, unsupported scenarios, known issues, or edge cases
- **Instructions:** Step-by-step guidance for setup, configuration, and use
- **Reference information:** Technical details like API endpoints, CLI flags, configuration syntax, or error codes
- **Troubleshooting:** Known problems and their solutions

Not every feature requires coverage in all areas. Use this framework to identify which areas apply, then list specific items that fall under each applicable area.

**Specificity matters:** Vague scope statements like "Document the feature" or "Explain how it works" do not help writers. List concrete items: "Explain how custom policies differ from default policies" or "Document the three policy types: device compliance, network access, and data classification."

### New and existing topics

**Purpose:** Identify whether the feature needs new documentation pages or updates to existing content.

This section helps writers understand the structural impact on the documentation set.

**New topics:** List topics that need their own dedicated pages because the functionality does not fit into existing documentation structure. You do not need to propose exact titles or detailed outlines—focus on what each topic should cover.

**Existing topics:** List documentation pages that need updates, with a brief description of what changes are required. This might include adding new options to existing procedures, updating conceptual explanations, adding cross-references, or revising terminology.

### Complexity estimate

**Purpose:** Help docs teams allocate resources and set realistic timelines.

Provide an assessment of the documentation effort required (typically low, medium, or high complexity) along with brief reasoning. Consider factors like:

- Number of new concepts to explain
- Number of pages to create or update
- Technical complexity of the feature
- Integration with other features or systems
- Number of edge cases or special scenarios

The assigned writer will validate and potentially adjust the complexity estimate based on their assessment. If you are unsure, provide your best guess and note your uncertainty.

## Creating your own documentation plan template

To create a documentation plan template for your organization:

1. **Review the core components** described above and determine which apply to your documentation process.
2. **Identify additional fields** specific to your workflow (target release date, stakeholder contacts, design review links, etc.).
3. **Create a template document** with clear instructions for each field, explaining what information is needed and why it matters.
4. **Provide examples** showing well-formed and poorly-formed entries for each field to guide contributors.
5. **Integrate with your workflow** by adding the template to your project tracking system, issue templates, or planning documents.
6. **Iterate based on feedback** from both feature teams filling out plans and writers using them.

## Stakeholder input and validation

Documentation plans are most effective when they include input from multiple perspectives:

- **Feature teams** provide technical accuracy and context about what is being built.
- **Product teams** clarify user-facing value and expected use cases.
- **Docs teams** identify gaps, ask clarifying questions, and validate that the plan provides sufficient information to begin writing.

Build review and validation into your process. The initial plan does not need to be perfect—it establishes a baseline that the assigned writer refines through follow-up questions and review cycles.

## Related concepts

- **[Complexity framework](./complexity-framework.md):** Detailed guidance for assessing documentation complexity levels
- **[Feature documentation](./feature-documentation.md):** Requirements for the documentation that writers create from plans
- **[Intake process](./intake-process.md):** How documentation plans fit into the overall documentation lifecycle

## Example

See [Sample documentation plan](../examples/sample-documentation-plan.md) for a complete example demonstrating these concepts.
