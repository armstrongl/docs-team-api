# Complexity framework template

Use this template to create your team's documentation complexity assessment framework.

**How to use this template:**

- Replace all example content with your team's specific criteria, timelines, and patterns
- Keep sections that are relevant to your product and workflow; remove sections that don't apply
- Update example features to reflect actual features from your product history
- Adjust lead times based on your team's capacity and review cycles
- For detailed guidance on creating complexity frameworks, refer to [Documentation complexity framework](../docs/complexity-framework.md)
- For a complete example, see [Sample complexity framework](../examples/sample-complexity-framework.md)

---

## Framework overview

This framework categorizes documentation work into three complexity levels based on feature characteristics. Each level maps to a typical review timeline, helping product managers and writers coordinate effectively.

Replace this paragraph with a brief description of how your team uses this framework. Explain the purpose and who should reference it when planning documentation work.

## Assessment factors

This framework evaluates three primary dimensions when assessing complexity:

Customize the number of assessment factors to match what actually drives documentation effort for your product. The three factors below (terminology, interfaces, components) are common starting points. Add, remove, or modify factors based on your domain. For example, API-focused products might emphasize endpoint count and authentication complexity, while SaaS products might focus on UI touchpoints and workflow variations.

### New terminology and concepts

Does the feature introduce new terminology, concepts, or syntaxes? How does it fit into the existing product ecosystem?

- **Lower complexity:** Uses existing terminology and builds on familiar concepts
- **Higher complexity:** Introduces new mental models, configuration syntaxes, or terminology that must be carefully distinguished from existing terms

### Number of interfaces

How many interfaces must a user interact with to use this feature?

Interfaces include admin dashboards, CLIs, APIs, configuration files, environment variables, third-party integrations, and any other touchpoint where the user takes action.

- **Lower complexity:** Single interface
- **Higher complexity:** Multiple interfaces requiring coordinated actions

### Number of components

How many components or systems are involved in getting the feature working?

- **Lower complexity:** Single configuration point
- **Higher complexity:** Multiple systems requiring configuration and coordination (for example, source and destination systems plus admin settings)

## Complexity tiers

Adjust the number of tiers, tier names, lead times, and pattern examples to reflect your team's actual documentation work patterns. Most teams use 2-4 tiers. The three-tier structure below (low/medium/high) is a common starting point.

### Low complexity

A low-complexity feature is easy to explain, relatively simple to use, does not introduce any new syntaxes, and only requires interaction with a single interface.

**Example patterns:**

Replace these examples with actual low-complexity features from your product history. Good examples help teams quickly recognize which tier applies to their current feature.

- A new option or setting that controls a straightforward behavior
- A new CLI flag that extends existing functionality in a predictable way
- A minor enhancement to an existing feature that does not change how users think about it

**Example writer review lead time:** 1-2 business days

Replace this lead time with realistic estimates for your team. Consider your team's review bandwidth, typical iteration cycles, time required for testing and validation, and documentation tooling overhead.

**Example draft deadline calculation:**

- Launch date: March 15
- Lead time: 1-2 business days
- Draft deadline: March 13-14

### Medium complexity

A medium-complexity feature has some complicating factors but no single aspect that makes it exceptionally difficult to document.

**Example patterns:**

Replace these examples with actual medium-complexity features from your product history.

- Introduces new terminology but uses familiar interfaces and workflows
- Involves multiple interfaces but the interactions follow established patterns
- Requires updating a few related documentation topics but not a major overhaul
- Adds a new capability that builds naturally on existing concepts

**Example writer review lead time:** 2-6 business days

Replace this lead time with realistic estimates for your team.

**Example draft deadline calculation:**

- Launch date: March 15
- Lead time: 2-6 business days
- Draft deadline: March 7-11

### High complexity

A high-complexity feature meets any of the following criteria: it touches many other features and likely requires updates to many documentation topics; it introduces a new syntax (for example, a configuration file format or policy syntax); it requires interaction with multiple interfaces or configuring multiple components; or it is inherently difficult to explain or use.

**Example patterns:**

Replace these examples with actual high-complexity features from your product history.

- A feature that introduces a new way of thinking about the product or significantly extends its conceptual model
- A feature that requires coordinating configuration across multiple systems and interfaces
- A feature with a new configuration file format or syntax that users must learn
- A feature that affects or interacts with many existing features, requiring documentation updates across multiple topics

**Example writer review lead time:** 8+ business days

Replace this lead time with realistic estimates for your team.

**Example draft deadline calculation:**

- Launch date: March 15
- Lead time: 8+ business days
- Draft deadline: March 5 or earlier

## Edge case handling

This section helps teams resolve ambiguous assessments. Customize these guidelines based on how your team prefers to handle disagreements and mixed signals.

### Elevating complexity for single exceptional factors

If any single factor is exceptionally complex, that typically elevates the overall complexity level. For example, a feature that uses a single familiar interface but introduces a fundamentally new concept with extensive new terminology may warrant medium or high complexity despite being simple in other respects.

### Mixed signals

When factors point to different levels, lean toward the higher level. It is better to plan for more review time and not need it than to underestimate and create timeline pressure.

Customize this guidance based on your team's risk tolerance and capacity constraints.

### Resolving ambiguity

Discuss ambiguous cases with the assigned writer. They can provide perspective on how similar features have played out in the past and what level of effort to expect.

Specify who makes the final determination if stakeholders disagree. Common approaches: writer has final authority, PM and writer discuss and jointly decide, or technical writing lead makes the call for contested assessments.

## Adaptation guidance

Teams adapting this framework should consider:

1. **Timeline adjustments:** The review lead times shown here are illustrative. Adjust based on team capacity, documentation tooling, and typical review cycles
2. **Complexity factors:** The three factors (terminology, interfaces, components) reflect common documentation challenges. Add or modify factors to match your product domain
3. **Tier granularity:** This example uses three tiers. Some teams may need more granular distinctions or broader categories
4. **Definition refinement:** The pattern examples should reflect actual features from your product to improve recognition accuracy

Delete this section after you've customized the framework, or replace it with guidance specific to your team's context (for example, how often to review and update the framework, or how new team members should learn to use it).
