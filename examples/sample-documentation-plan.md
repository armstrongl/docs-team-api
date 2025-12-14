# Sample documentation plan

This sample demonstrates how to complete a documentation plan section for a parent initiative. Use it as a reference when filling out your own documentation plans.

**Note:** This is a generic example. Adapt the format, fields, and level of detail to match your organization's needs and processes.

## Feature summary

Analytics reporting lets administrators track system usage patterns, identify optimization opportunities, and demonstrate value to stakeholders. Administrators access pre-built reports through the dashboard or create custom reports using the API.

## Terminology

| Term | Usage notes |
|------|-------------|
| analytics report | Lowercase. Two words, not hyphenated. Don't call it "usage report" or "metrics report." |
| Report Builder | Capitalize both words. This is the specific UI component name, distinct from the general concept of building reports. |
| data retention period | Lowercase. Three words, not hyphenated. Always specify the duration when documenting. |
| time-series metric | Lowercase except when sentence-initial. Hyphenate "time-series" when used as an adjective. Plural is "time-series metrics." |

## Documentation scope

The documentation must cover:

- **Core concepts:** What analytics reports are, how they differ from real-time monitoring, and common use cases.
- **Requirements:** Administrator permissions required, minimum plan tier, prerequisites for accessing historical data.
- **Report types:** Pre-built reports (usage summary, performance trends, security events) and custom reports.
- **Instructions:** How to view a pre-built report, how to customize date ranges and filters, how to export data.
- **Limitations:** Data retention limits (30 days standard, 90 days enterprise), reports cannot combine data from multiple organizations, refresh intervals.
- **API reference:** New endpoints `GET /analytics/reports`, `POST /analytics/reports/custom`, and `GET /analytics/metrics`.
- **Troubleshooting:** Common issues like missing data (permissions or retention), slow report generation (data volume), and export failures (file size limits).

## New and existing topics

### New topics

The following new documentation pages are needed:

- A page explaining analytics reporting concepts, report types, and when to use each type.
- A guide for creating and managing custom reports through the Report Builder interface.
- API reference documentation for the new analytics endpoints.

### Existing topics

The following existing pages require updates:

- **Administrator permissions reference:** Add new analytics-related permissions (view reports, create custom reports, export data).
- **Plan comparison table:** Add analytics features row showing data retention differences (30 vs. 90 days).
- **Getting started guide:** Add mention of analytics reporting in the "Monitor your system" section with link to new analytics page.
- **API overview:** Add analytics endpoints to the API capabilities summary.

## Complexity estimate

**Complexity level:** Medium

**Reasoning:** This feature introduces several new concepts (report types, custom queries, data retention) that require conceptual explanation beyond simple instructions. The documentation requires three new pages plus updates to four existing pages. However, the feature follows established patterns for dashboard-based features, and the API endpoints follow standard REST conventions. There are no unusual edge cases or complex integration scenarios to document.
