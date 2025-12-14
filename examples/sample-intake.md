# Sample intake: Health monitoring feature

This example shows a completed documentation intake for a fictional feature. Use it as a reference when completing your own documentation requests.

---

## Feature summary

Health monitoring lets administrators see which services are online, how much traffic they're handling, and whether they're configured correctly. Administrators access this information through the dashboard and the API.

## Terminology

This section defines the standard terms and usage conventions for health monitoring documentation.

| Term | Usage notes |
|------|-------------|
| health, `health` | Lowercase unless at the beginning of a sentence. Use to refer to the overall condition of a service. Don't use "status" or "state." Format in code if referring to the API endpoint. |
| service ID, `service_id` | Lowercase, two words. Unique identifier for a service. Always use code formatting if referring to the API parameter or response field (`service_id`) |
| Health check | Lowercase unless at the beginning of a sentence. Two words, not hyphenated. Don't call it "status check" or "ping." |
| Healthy | Lowercase unless at the beginning of a sentence. Use to describe a service that passes all health checks. Don't use "up" or "online." |
| Unhealthy | Lowercase unless at the beginning of a sentence. Use to describe a service that fails one or more health checks. Don't use "down" or "offline." |
| Health Monitoring | Always capitalize both words when referring to the feature name. On first reference, clarify this is the product's specific feature, not the general concept of monitoring health. |
| Dashboard | Always capitalize when referring to the product's specific dashboard interface. |
| `check_interval` | Lowercase, one word with underscore. Configuration option for how often health checks run. Don't hyphenate or use camelCase. Always use code formatting. |
| `alert_threshold` | Lowercase, one word with underscore. Configuration option for the number of failed checks before triggering an alert. Don't hyphenate or use camelCase. Always use code formatting. |
| `retention_days` | Lowercase, one word with underscore. Configuration option for how long to keep historical health data. Don't hyphenate or use camelCase. Always use code formatting. |

## Documentation scope

This section outlines the information that needs to be documented for the health monitoring feature, including user-facing concepts, requirements, limitations, and procedures.

### What users need to know

- Core concepts: what health monitoring is and how it works.
- Why users would use this: proactive identification of service issues.

### Requirements

- Permissions: Admin role required to view health data.
- Plan: Available on Business and Enterprise plans.
- Prerequisites: At least one service must be configured.

### Limitations

- Health checks run every 60 seconds; more frequent checks not supported.
- Historical data retained for 30 days.
- Known issue: health check failures during maintenance windows may trigger false alerts.
  - Configure maintenance windows to suppress alerts during scheduled downtime.

### Instructions needed

- How to enable health monitoring for a service.
- How to configure alert thresholds.
- How to view health status in the dashboard.
- How to query health data using API.

### Reference documentation

- API endpoints: `GET /api/v1/health`, `GET /api/v1/health/{service_id}`.
- Configuration options: `check_interval`, `alert_threshold`, `retention_days`.

### Troubleshooting

- What to do when health checks fail unexpectedly.
- How to debug connectivity issues affecting health checks.

## New topics needed

- Health monitoring overview (conceptual).
- Enable health monitoring (how-to).
- Health monitoring API reference.

## Existing topics to update

- Dashboard overview: add section on health status panel.
- API reference index: add links to new health endpoints.

## Complexity estimate

**Level:** Medium

**Reasoning:** Introduces new terminology (health check, healthy, unhealthy) but uses familiar interfaces (dashboard, API). Requires new topics but builds on existing concepts. Two interfaces involved (dashboard and API) but interactions follow established patterns.
