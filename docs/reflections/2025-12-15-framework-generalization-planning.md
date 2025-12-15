# Session Reflection: Framework Generalization Planning

**Date**: 2025-12-15
**Task**: Transform docs-team-api into a generic team-api-framework
**Outcome**: Comprehensive implementation plan created and validated

---

## Problems and Reflections

### 1. Scope question came too late

I asked five rounds of clarifying questions before discovering the user only wanted a plan, not implementation. The "Plan only" vs "Full implementation" question was in Round 5. Earlier rounds included detailed questions about parallel development and research methodology that would have been framed differently if I knew upfront this was planning-only.

**Impact**: Wasted cognitive load considering implementation details prematurely.

### 2. Relied on exploration summary instead of verifying file inventory

The Explore agent reported "14 framework documents" but the actual count was 12 in `/docs/`. I wrote the initial plan based on this approximation, then discovered discrepancies during validation:
- Templates: 10 files exist, plan only listed 6 for `/core/templates/`
- Examples: 15 files exist, plan didn't enumerate them
- Missing template: `last-minute-changes-template.md` doesn't exist but was listed in the plan

**Impact**: Initial plan had inaccurate migration tables; required correction during validation.

### 3. Team type options were incomplete

When asking which team types to include, my options were:
- Design/UX teams
- Platform/Infrastructure
- Data/Analytics teams
- Support/Customer Success

The user selected: Design, Engineering, Product, Marketing - three of which weren't in my options. They had to use "Other" to specify their actual preferences.

**Impact**: Poor question design required user to work around my assumptions.

### 4. Missed the "parallel development" decision in plan structure

User explicitly selected "Docs first + Parallel development" but my Phase 3 was structured sequentially ("For each domain: research, create, quality check"). I only caught this during validation.

**Impact**: Plan didn't reflect the user's stated preference until correction.

### 5. Delayed validation until prompted

I created the plan and marked it complete. The user then asked me to validate it with ultrathink. The validation found 10+ issues including:
- Structural issues (missing files, wrong counts)
- Conceptual issues (Product team model inverted, Engineering dual modes)
- Process issues (parallel development not reflected)
- Missing elements (no hybrid teams guidance, no build-your-own-domain guide)

**Impact**: Validation should have been automatic, not user-prompted.

### 6. $PLANS_PATH confusion

The user's CLAUDE.md specifies `$PLANS_PATH` as `~/dotfiles/docs/plans/`. I initially tried `~/dotfiles/docs/plans/` which didn't exist, then discovered it was `~/.dotfiles/docs/plans/`. The environment variable would have resolved this.

**Impact**: Minor - one extra command to find correct path.

---

## Insights

### 1. Scope and effort questions should come first

For any non-trivial task, immediately clarify:
- Is this planning only, or planning + implementation?
- What's the expected depth/completeness?
- What's the timeline context?

This shapes all subsequent questions and prevents over-engineering the discovery phase.

### 2. File inventory verification is mandatory for migration planning

Any plan involving file moves must start with an exact inventory:
```bash
find /path -name "*.md" | wc -l  # Get exact counts
ls -la /path/  # List actual files
```

Never trust summaries or approximations for migration tables.

### 3. Conceptual model analysis reveals hidden complexity

Recognizing that Product teams "initiate" rather than "receive" work fundamentally changes how their Team API should be structured. This conceptual insight came late (during validation). Such analysis should happen earlier, perhaps as part of initial exploration.

Pattern: When adapting a framework to new domains, explicitly ask "Does this domain follow the same interaction model as the original?"

### 4. User decisions must be traced through the plan

When a user makes an explicit choice (like "parallel development"), I should:
1. Note it prominently
2. Trace it through every relevant section
3. Verify it's reflected before presenting the plan

### 5. Validation is a distinct phase, not optional polish

The validation found substantial issues that would have caused problems during execution. This suggests a pattern:
- **Create** → **Validate** → **Present**

Not:
- **Create** → **Present** → (maybe validate if asked)

### 6. Clarifying questions work best with open-ended fallbacks

My team type question failed because I assumed I knew the options. Better pattern:
- Round 1: Open-ended ("What team types are you most interested in?")
- Round 2: Confirm/refine specific selections

Or include genuinely useful "Other" guidance in multi-select questions.

### 7. The exploration agent is for discovery, not inventory

The Explore agent excels at understanding purpose, patterns, and relationships. It's not optimized for exact file counts. Use the right tool:
- **Explore agent**: "What is this repo about? What patterns exist?"
- **Glob/ls**: "Exactly how many files? What are their names?"

---

## Suggested Changes and Improvements

### For This Workflow

1. **Add scope question to Round 1**: Always ask "Plan only, plan + partial implementation, or full implementation?" before detailed discovery.

2. **Verify inventory before planning migrations**: Before writing any file migration table, run:
   ```bash
   find . -name "*.md" -type f | head -50
   ```

3. **Build validation into plan creation**: After writing a plan, automatically:
   - Re-read the plan
   - Compare against stated user decisions
   - Verify file references against actual filesystem
   - Check for conceptual consistency

4. **Trace decisions explicitly**: When user makes a choice, add a comment in the plan: `<!-- User decision: parallel development for Phase 3 -->`

### For Skills (umami-marketplace)

1. **Update `asking-clarifying-questions` skill**:
   - Add guidance to ask scope/effort questions in first round
   - Recommend open-ended questions before constrained options
   - Include pattern for tracing decisions through artifacts

2. **Create `planning-migration` skill** (or add to existing planning skills):
   - Mandate file inventory verification
   - Template for migration tables with source verification
   - Checklist for migration plan completeness

3. **Create `validating-plans` skill** (or enhance `scrutinizing-plans`):
   - Systematic validation checklist
   - Decision tracing verification
   - File reference verification
   - Conceptual consistency check

### For CLAUDE.md (Global)

Add to the Planning section:

```markdown
### Migration Planning

When creating plans that involve moving or restructuring files:
1. Always verify exact file inventory with Glob before writing migration tables
2. Never trust summaries or approximations for file counts
3. Validate file references in the plan against actual filesystem before presenting

### Plan Validation

After creating any implementation plan:
1. Re-read the plan in full
2. Verify all user decisions are reflected in relevant sections
3. Check file references against actual filesystem
4. Validate conceptual consistency across domains/sections
5. Present validation findings alongside the plan, not as a separate step
```

### For Project CLAUDE.md (docs-team-api)

Add domain-specific guidance once restructuring begins:

```markdown
### Domain Conceptual Models

Not all team types follow the same interaction pattern:
- **Service teams** (Docs, Design, Support): Receive requests, deliver outputs
- **Orchestrating teams** (Product, Program): Initiate work, coordinate others
- **Executing teams** (Engineering): May operate in either mode depending on org structure

When creating new domain implementations, first identify which conceptual model applies.
```

---

## Summary

The session was successful - a comprehensive, validated plan was created. However, the validation phase revealed issues that should have been caught during initial creation. The key learnings center on:

1. **Front-load scope questions** to avoid over-engineering discovery
2. **Verify inventories** before creating migration plans
3. **Treat validation as mandatory**, not optional
4. **Trace user decisions** through all plan sections
5. **Match tools to tasks** (Explore for patterns, Glob for inventory)

These patterns would have saved approximately 30% of the session time and produced a higher-quality first draft.
