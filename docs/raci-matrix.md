# RACI matrix

A RACI matrix is a responsibility assignment framework that clarifies who does what in cross-functional processes. For docs teams, it prevents common coordination failures: duplicate work, missed handoffs, unclear ownership, and conflicting expectations during feature launches or content projects.

## Why docs teams need a RACI matrix

Documentation work involves multiple stakeholders across product, engineering, design, and marketing. Without explicit responsibility assignments, teams encounter:

- **Ownership gaps:** No one knows who should write the first draft or approve final content.
- **Duplicate effort:** Multiple people work on the same task without coordination.
- **Missed inputs:** Subject matter experts aren't consulted early enough to provide critical information.
- **Blocked workflows:** Unclear approval chains delay publication.
- **Inconsistent processes:** Each project follows different ad-hoc patterns.

A RACI matrix makes implicit assumptions explicit. It documents your team's agreed-upon process, creating a shared reference point for coordination.

## Core concepts

### The four responsibility types

Each activity in your process gets assigned one or more of these responsibility types:

- **R (Responsible):** Does the work. The person or people who execute the activity. Multiple roles can share responsibility when work requires collaborative effort.
- **A (Accountable):** Ultimately answerable for completion and approves the work. The single person who owns the outcome and ensures the activity happens. Only one person should be Accountable for each activity.
- **C (Consulted):** Provides input before or during the work. People whose expertise or perspective is needed for the activity to succeed.
- **I (Informed):** Kept updated on progress or outcomes. People who need to know about the activity but don't directly contribute to it.

The key distinction: **Responsible** parties do the work. **Accountable** parties own the outcome.

### Role identification

Your RACI matrix needs clearly defined roles that map to actual people or teams in your organization. Common roles for docs teams include:

- **Writers and editors:** Technical writers, content designers, documentation engineers
- **Product stakeholders:** Product managers, product owners, product marketing
- **Engineering stakeholders:** Engineers, engineering managers, tech leads, architects
- **Design stakeholders:** UX designers, UX researchers, design leads
- **Documentation leadership:** Docs team leads, content strategy, documentation managers

Use role names that make sense in your organization. The roles should be specific enough to assign responsibility but generic enough to remain stable as people change positions.

### Activity categorization by phase

Organize activities into phases that reflect your actual workflow. Documentation processes typically include:

- **Planning phase:** Requirements gathering, scope definition, resource allocation
- **Development phase:** Drafting, technical review, editing
- **Review and approval phase:** Stakeholder review, final approvals, sign-offs
- **Publishing phase:** Publication, announcement, launch coordination
- **Maintenance phase:** Updates, corrections, feedback incorporation

Your phases should represent distinct stages where handoffs occur or accountability shifts between teams.

### Handling shared responsibility

When multiple roles appear in the Responsible column, document how they collaborate:

- **Sequential collaboration:** Different roles contribute at different stages. Example: PM defines requirements, Eng provides technical details, Writer creates the documentation plan.
- **Parallel contribution:** Multiple roles work simultaneously on different aspects. Example: Eng develops the feature while Writer drafts documentation based on specifications.
- **Conditional responsibility:** The responsible party varies by project. Example: Either Eng or Writer might draft depending on technical complexity.

Use footnotes to explain shared responsibility patterns. This prevents confusion about who actually does what when you see multiple names in a cell.

## Creating your RACI matrix

### 1. Identify your process phases

Map out your end-to-end documentation workflow from initial feature planning through post-launch updates. Break it into distinct phases where responsibility typically shifts between teams.

Ask: "What are the major stages of work between when we first hear about a feature and when the documentation is stable?"

### 2. List key activities in each phase

For each phase, identify the specific activities that must happen. Focus on activities that:

- Require coordination between teams
- Have caused confusion or conflicts in the past
- Involve handoffs or approvals
- Impact project timelines or quality

Avoid listing every minor task. Focus on coordination points and decision points.

### 3. Define the roles involved

List all the roles that participate in your documentation process. Include:

- All docs team roles (writers, editors, leads)
- Cross-functional partners (product, engineering, design, marketing)
- Leadership or approval roles
- Any external contributors

Use role titles, not individual names. The matrix should work regardless of who currently fills each role.

### 4. Assign RACI designations

For each activity, assign responsibility types to roles:

1. Start with **A (Accountable):** Who owns the outcome? Only one role should be Accountable.
2. Assign **R (Responsible):** Who does the work? May be one or more roles.
3. Identify **C (Consulted):** Whose input is needed before or during the work?
4. Determine **I (Informed):** Who needs to know about progress or results?

Not every role needs a designation for every activity. Empty cells are fine.

### 5. Document shared responsibility patterns

When multiple roles are Responsible, add footnotes explaining:

- How the work is divided
- The sequence of contribution
- Conditions that determine who does what
- Examples from past projects

This context prevents the matrix from becoming ambiguous.

### 6. Validate with stakeholders

Review the matrix with all teams involved in the process. Ask:

- Does this match how we actually work?
- Are there gaps or conflicts?
- Is anyone over- or under-loaded?
- Do the handoffs make sense?

Much of the value comes from the discussion during creation, not just the final document.

### 7. Test and iterate

Apply the matrix to an actual project. Note where reality diverges from the documented process. Update the matrix to reflect what actually works, not what you wish would work.

A RACI matrix is a living document. Expect to revise it as your team structure, processes, or coordination needs change.

## Best practices

### Keep it simple

Start with high-level activities. You can always add detail later if needed. An overly detailed matrix becomes difficult to maintain and reference.

### One Accountable per activity

If you can't identify a single Accountable role, the activity might be too vague or your process has an ownership gap. Split the activity or clarify accountability.

### Document the why, not just the what

Add context about why certain roles are assigned to certain activities. This helps future team members understand the reasoning and make better decisions about when to deviate.

### Use it as a communication tool

Reference the RACI matrix when onboarding new team members, planning projects, or resolving coordination conflicts. It should be a working tool, not a document that lives forgotten in a repository.

### Update it when processes change

When you change your workflow, update the matrix. When the matrix doesn't match reality, update it to match actual practice (or fix the practice if the documented process is better).

## Example

See [Sample RACI matrix](../examples/sample-raci.md) for a complete example demonstrating these concepts.
