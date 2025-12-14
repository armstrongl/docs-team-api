# Sample last-minute change resolution

This example demonstrates how the last-minute changes protocol operates in practice. The scenario involves a terminology change discovered after the documentation cut-off date. The example shows the complete process from initial notification through post-launch completion.

---

## Scenario

The API Analytics Dashboard feature is scheduled to launch on March 15. The feature allows developers to visualize API usage patterns, track response times, and monitor error rates through a web-based dashboard.

On March 5, the product team discovers that the term "workspace" conflicts with existing platform terminology. User research shows that this conflict will cause confusion. The term needs to change to "project" throughout the feature and all documentation.

This discovery occurs 10 days before launch, which is inside the two-week cut-off for terminology changes.

## Initial notification

This section illustrates how the product manager communicated the last-minute change to stakeholders and initiated the decision-making process.

The product manager posts the following message to the `#api-analytics` channel on March 5 at 2:47 PM:

> **Last-minute terminology change - Launch impact**
>
> We need to change "workspace" to "project" throughout the API Analytics Dashboard feature. User research conducted this week showed that "workspace" conflicts with the existing workspace concept in the platform's collaboration features. This is causing confusion in testing.
>
> **Details:**
>
> - **Change:** Rename "workspace" to "project" everywhere in the feature
> - **Discovered:** March 5 (today)
> - **Launch date:** March 15 (10 days from now)
> - **Assigned writer:** @Jordan Chen
>
> This is past our two-week cut-off for terminology changes. We need to discuss how to handle this. Engineering is updating the UI now. The change affects approximately 15 screens and all related API endpoints.
>
> @Jordan Chen @Alex Rivera (EM) @Sam Okafor (Eng Lead) - Can we meet tomorrow to discuss options?

Jordan Chen (the assigned writer) replies at 3:12 PM:

> Thanks for flagging this quickly. I've reviewed the current documentation draft. The term "workspace" appears in:
>
> - The overview topic (8 instances)
> - The getting started tutorial (12 instances)
> - Two how-to guides (16 instances total)
> - The API reference (23 instances)
> - Three conceptual topics (14 instances)
>
> Total: 73 instances across 9 topics, plus screenshots showing the term in the UI.
>
> I can attend a meeting tomorrow. Given the scope, we need to discuss whether to postpone or restrict documentation scope for launch.

## Discussion and decision-making

The team evaluates two primary options: postponing the launch to allow time for complete documentation updates, or restricting the documentation scope to meet the existing launch timeline.

The team meets on March 6 at 10:00 AM. Attendees include:

- Sam Okafor (Product Manager)
- Alex Rivera (Engineering Manager)
- Jordan Chen (Technical Writer)
- Taylor Kim (Engineering Lead)

### Option 1 discussion: Postpone the launch

This option explores delaying the feature release to accommodate comprehensive documentation updates including all terminology changes and screenshot updates.

Sam Okafor presents the business context:

"Postponing would mean missing our Q1 launch commitment. We've already communicated the March 15 date to customers who participated in the beta program. Marketing has scheduled announcements and webinars."

Alex Rivera provides the engineering perspective:

"Engineering can complete the code changes by March 8. The terminology change is straightforward in the code. QA needs three days to retest, which brings us to March 11. That gives Jordan four days to update documentation before March 15."

Jordan Chen assesses the documentation work:

"Four days is tight but possible for the text changes themselves. However, we have 23 screenshots that show the old term. I need to retake those screenshots from the updated UI, which won't be available until March 11 after QA completes. That leaves me one business day for screenshots, final review, and publishing. That's high risk for quality."

**Team assessment of Option 1:** Postponing by one week (to March 22) would allow time for quality documentation, but conflicts with business commitments. This option is possible but not preferred.

### Option 2 discussion: Restrict documentation scope

This option considers launching with core documentation only, deferring advanced topics to a post-launch completion phase.

Jordan Chen proposes the scope restriction:

"We could launch with the overview, getting started tutorial, and API reference updated. Those are the critical pieces users need to start using the feature. The two how-to guides and three conceptual topics could be deferred to post-launch.

"The overview and tutorial have fewer screenshots (6 total). I can update those text and screenshots in the four-day window. The API reference is primarily text, so that's manageable. The how-to guides and conceptual topics have 17 screenshots between them—that's where the time crunch is worst."

Taylor Kim evaluates user impact:

"The how-to guides cover advanced filtering and custom metrics. Those are important features, but not required for initial use. The conceptual topics explain performance optimization and best practices. Users can access the feature effectively without those topics at launch."

Sam Okafor considers business implications:

"This approach gets the feature launched on time with documentation for core functionality. The advanced topics can follow within two weeks. That timeline still supports our customer commitments."

Alex Rivera confirms engineering support:

"Engineering can prioritize helping Jordan with the post-launch documentation. Taylor can review drafts and answer questions to speed up the work on the deferred topics."

**Team assessment of Option 2:** Restricting scope allows on-time launch with quality documentation for core functionality, while deferring advanced topics to post-launch. This approach balances business needs with documentation quality.

### Final decision

The team commits to restricting documentation scope with specific deliverables for launch and a clear timeline for post-launch completion.

The team agrees to restrict documentation scope. The decision is:

**Include at launch (March 15):**

- API Analytics Dashboard overview
- Getting started tutorial
- API reference documentation

**Defer to post-launch (by March 29):**

- How-to: Create custom filters for analytics queries
- How-to: Build custom metrics and visualizations
- Concept: Analytics performance optimization
- Concept: Dashboard best practices
- Concept: Understanding analytics data models

## Recording the decision

The team documents the decision in both the team communication channel for visibility and in the work tracking system for formal project records.

### Channel summary

Jordan Chen posts this summary to the `#api-analytics` channel on March 6 at 11:15 AM:

> **Resolution: API Analytics Dashboard terminology change**
>
> **Change:** Rename "workspace" to "project" throughout the feature (discovered March 5, inside two-week cut-off)
>
> **Decision:** Restrict documentation scope for March 15 launch
>
> **Documentation included at launch:**
>
> - API Analytics Dashboard overview
> - Getting started tutorial
> - API reference documentation
>
> **Documentation deferred to post-launch (deadline: March 29):**
>
> - How-to: Create custom filters for analytics queries
> - How-to: Build custom metrics and visualizations
> - Concept: Analytics performance optimization
> - Concept: Dashboard best practices
> - Concept: Understanding analytics data models
>
> **Timeline:**
>
> - March 8: Engineering completes terminology change in code
> - March 11: QA completes testing of updated UI
> - March 11-14: Documentation updates and review for launch scope
> - March 15: Launch with core documentation
> - March 15-29: Complete and publish deferred documentation
>
> **Decision made by:** Sam Okafor (PM), Alex Rivera (EM), Jordan Chen (Writer), Taylor Kim (Eng Lead)

### Work item record

Jordan Chen adds this comment to issue `DOCS-ISSUE-847` (the documentation request for the API Analytics Dashboard launch) on March 6:

> **Last-minute change requiring scope adjustment**
>
> **Change:** Terminology change from "workspace" to "project" discovered after documentation cut-off.
>
> **Discovery date:** March 5, 2025 (10 days before planned March 15 launch)
>
> **Reason for change:** User research showed "workspace" conflicts with existing platform terminology, causing user confusion.
>
> **Impact:** 73 instances of the term across 9 documentation topics, plus 23 screenshots requiring updates.
>
> **Resolution:** Restrict documentation scope at launch, defer advanced topics to post-launch period.
>
> **Launch scope:** Overview, getting started tutorial, and API reference (6 screenshots, manageable within timeline).
>
> **Deferred work:** Created separate issues for post-launch documentation (see links below). All deferred work must be completed by March 29.
>
> **Deferred issues:**
>
> - `DOCS-ISSUE-892`: How-to: Create custom filters for analytics queries
> - `DOCS-ISSUE-893`: How-to: Build custom metrics and visualizations
> - `DOCS-ISSUE-894`: Concept: Analytics performance optimization
> - `DOCS-ISSUE-895`: Concept: Dashboard best practices
> - `DOCS-ISSUE-896`: Concept: Understanding analytics data models
>
> **Decision participants:** Sam Okafor (PM), Alex Rivera (EM), Jordan Chen (Writer), Taylor Kim (Eng Lead)

## Post-launch follow-up

Jordan Chen tracks progress on the deferred documentation topics through regular status updates to maintain visibility and accountability.

### Week 1 progress (March 16-22)

Jordan Chen begins work on the deferred topics immediately after launch. On March 19, Jordan posts a progress update to the `#api-analytics` channel:

> **Post-launch documentation update**
>
> Progress on deferred API Analytics topics:
>
> - `DOCS-ISSUE-892` (Custom filters how-to): Draft complete, in review with Taylor
> - `DOCS-ISSUE-893` (Custom metrics how-to): Draft complete, in review with Taylor
> - `DOCS-ISSUE-894` (Performance optimization): In progress, 60% complete
> - `DOCS-ISSUE-895` (Best practices): In progress, 40% complete
> - `DOCS-ISSUE-896` (Data models concept): Starting March 20
>
> On track for March 29 deadline. Screenshots are going smoothly with the stable `UI`.

### Week 2 completion (March 23-29)

On March 26, Jordan Chen posts the completion update:

> **Post-launch documentation completed**
>
> All deferred API Analytics Dashboard documentation is now published:
>
> - `DOCS-ISSUE-892`: How-to: Create custom filters for analytics queries
> - `DOCS-ISSUE-893`: How-to: Build custom metrics and visualizations
> - `DOCS-ISSUE-894`: Concept: Analytics performance optimization
> - `DOCS-ISSUE-895`: Concept: Dashboard best practices
> - `DOCS-ISSUE-896`: Concept: Understanding analytics data models
>
> Timeline met. All topics completed by March 26, three days ahead of the March 29 deadline.
>
> Thanks to @Taylor Kim for quick review turnaround and technical input, which helped accelerate the process.

Jordan Chen closes all five deferred issues and adds a final comment to `DOCS-ISSUE-847`:

> **Post-launch documentation completed**
>
> All deferred documentation completed and published by March 26, ahead of the March 29 deadline. The terminology change from "workspace" to "project" is now consistent across all API Analytics Dashboard documentation.
>
> **Lessons learned:**
>
> - Restricting launch scope allowed quality documentation for core features while meeting the business timeline
> - Early creation of deferred issues (at decision time rather than after launch) helped with planning and tracking
>   - Contact @Jordan Chen for guidance on creating deferred issue structure
> - Engineering support during post-launch period accelerated review cycles
>   - Having dedicated engineering reviewer availability significantly improved turnaround time
>
> Full documentation suite is now available to users.

## Outcome

The API Analytics Dashboard launched on March 15 with complete documentation for core functionality. Users could successfully discover, learn, and use the feature from launch day. Advanced topics were added within two weeks, completing the full documentation suite ahead of the deadline.

The team met both business objectives (on-time launch) and quality standards (accurate, complete documentation) by applying the last-minute changes protocol.
