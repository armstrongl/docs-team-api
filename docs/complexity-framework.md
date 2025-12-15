# Documentation complexity framework

A documentation complexity framework provides a systematic approach to estimating how much effort a feature's documentation will require. This helps teams plan timelines, allocate resources, and set realistic expectations for documentation reviews.

## What is a complexity framework?

A complexity framework categorizes documentation work into distinct tiers based on feature characteristics. Each tier corresponds to an estimated effort level, typically expressed as review lead time or writer hours. The framework helps product managers, engineers, and technical writers communicate about documentation scope using shared vocabulary and expectations.

Unlike project estimation tools that track hours or story points, a complexity framework focuses on pattern recognition. Teams read tier descriptions and identify which category best matches their feature's characteristics rather than calculating scores or summing weighted factors.

## Why docs teams need complexity frameworks

### Timeline planning

Documentation work must fit into product release cycles. A complexity framework enables teams to answer the critical question: "When does the draft need to be ready so the writer has enough time to review before launch?" Without this framework, teams frequently underestimate documentation effort, leading to rushed reviews, delayed launches, or shipping documentation with known quality issues.

### Scope calibration

Complexity assessments help product teams and writers align on what level of documentation effort is appropriate for a given feature. This alignment prevents scope mismatches where product managers expect minimal documentation updates for features that actually require substantial documentation work, or vice versa.

### Resource allocation

When multiple features ship concurrently, a complexity framework helps docs teams prioritize review work and identify when they need additional capacity.

### Cross-functional communication

A shared complexity vocabulary enables clearer communication between product managers, engineers, and writers. Rather than discussing vague "small" or "large" documentation efforts, teams can reference specific complexity tiers with defined characteristics and timelines.

## Core components

Effective complexity frameworks typically include four core components:

### 1. Complexity tiers

Most frameworks define 2-4 complexity levels (for example, low/medium/high or simple/moderate/complex/extensive). Each tier represents a distinct effort category with recognizable characteristics.

The number of tiers should balance granularity with simplicity. Too few tiers (for example, just "small" and "large") make it difficult to distinguish between genuinely different effort levels. Too many tiers create unnecessary cognitive overhead and assessment debates.

### 2. Assessment criteria

Assessment criteria are the factors teams evaluate when determining complexity. Common criteria include:

- **Conceptual novelty:** Does the feature introduce new mental models or terminology?
- **Interface count:** How many user touchpoints are involved?
- **Component scope:** How many systems or subsystems require configuration?
- **Documentation breadth:** How many existing documentation pages need updates?
- **User journey complexity:** How many steps or decisions are involved in using the feature?

Teams should select criteria that reflect the actual drivers of documentation effort in their domain.

### 3. Timeline mapping

Each complexity tier maps to an estimated review lead time or total effort. This mapping translates abstract complexity levels into concrete planning numbers.

Lead times typically represent the buffer needed for writer review and collaboration, starting from when a reviewable draft exists. Some frameworks additionally specify total documentation hours or writer capacity requirements.

### 4. Edge case guidance

Features rarely fit perfectly into predefined categories. Frameworks should include guidance for:

- **Mixed signals:** When different assessment criteria point to different tiers
- **Exceptional factors:** When a single characteristic dominates the complexity assessment
- **Ambiguity resolution:** How to handle disagreements between product managers and writers

## Creating your own complexity framework

### 1. Analyze historical work

Review past documentation projects and identify patterns. Look for natural groupings based on effort, timeline, or characteristics. Consider:

- What features required minimal documentation effort?
- What features required moderate effort?
- What features consumed significant writer time?
- What characteristics distinguished these groups?

### 2. Define tiers based on actual patterns

Create complexity tiers that reflect the natural groupings you observed. Name tiers descriptively and provide concrete examples from your product for each tier.

Avoid creating tiers based on theoretical distinctions that don't correspond to real effort differences in your domain.

### 3. Identify assessment criteria

Determine which feature characteristics reliably predict documentation effort for your product. Common criteria work for many teams, but domain-specific products may require specialized factors.

For example:

- API-focused products might emphasize endpoint count and authentication complexity
- Infrastructure products might prioritize configuration model depth and component dependencies
- SaaS products might focus on UI touchpoints and workflow variations

### 4. Calibrate timelines

Map each tier to realistic lead times based on your team's typical review cycles and capacity. Start conservatively and adjust based on experience.

Consider:

- Your team's review bandwidth
- Typical iteration cycles between drafts
- Time required for testing and validation
- Documentation tooling and publishing overhead

### 5. Document edge case handling

Specify how to resolve common assessment challenges:

- When factors point to different tiers, which takes precedence?
- How should single exceptional characteristics affect the overall assessment?
- Who makes the final determination if stakeholders disagree?

### 6. Establish the assessment workflow

Define when and how complexity gets assessed. Common approaches:

- **Product manager initiates:** PM assesses complexity when completing project documentation template
- **Writer validates:** Assigned writer reviews and may adjust the assessment
- **Joint assessment:** PM and writer discuss complexity together during kickoff

Specify what happens when assessments diverge and who has final authority.

### 7. Validate and iterate

Test the framework with upcoming features. After each release cycle, review whether complexity assessments matched actual effort. Adjust tier definitions, criteria, or timelines based on observed patterns.

## Common pitfalls

### Over-specification

Frameworks that try to account for every possible scenario become too complex to use effectively. Aim for "good enough" categorization rather than perfect precision.

### Treating timelines as commitments

Lead times are planning estimates, not guarantees. Actual effort varies based on draft quality, subject matter expert availability, and competing priorities. Frameworks should acknowledge this variability.

### Ignoring context

Complexity assessments depend on team capacity and expertise. A framework that works for a well-staffed team with mature documentation may not work for a team building documentation from scratch.

### Static frameworks

Product evolution changes documentation patterns. Frameworks should be reviewed and updated periodically to reflect current reality.

## What complexity frameworks don't do

Frameworks don't replace communication. They provide shared vocabulary for discussions, but they don't eliminate the need for writers and product teams to collaborate on scope and approach.

## Related concepts

- **[Documentation plan](./documentation-plan.md)**: Structured templates that capture documentation scope, audience, and delivery details. Complexity assessment often occurs within these templates.
- **Definition of done**: Criteria for considering documentation complete. Complexity frameworks inform timeline planning, but definition of done determines quality standards.
- **Documentation review process**: The workflow for reviewing and approving documentation. Complexity frameworks estimate the duration of this process but don't define the process itself.

## Example

See [Sample complexity framework](../examples/sample-complexity-framework.md) for a complete example demonstrating these concepts.
