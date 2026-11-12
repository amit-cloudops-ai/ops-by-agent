# Observability Standards

## Signals
Instrument services with structured logs, metrics and traces as appropriate. Use correlation IDs to connect user requests, agent tasks, model calls, tool calls and infrastructure outcomes.

## Minimum signals
- Request and task counts, outcomes and duration.
- Tool invocation counts, latency, failures and throttling.
- Model identifier, token usage, latency and inference cost where available.
- Approval requested, granted, denied and expired counts.
- Retry counts and timeout rates.
- Application health and dependency availability.

## Logging
Logs must be structured, access-controlled and useful for investigation. Redact credentials and minimize personal or operationally sensitive data. Define retention and deletion requirements.

## Alerting
Alerts should be actionable, severity-aware and linked to runbooks. Avoid exposing secret values or unnecessarily duplicating sensitive payloads.

## Operational review
Document dashboards, health checks, service objectives, alert thresholds and failure response for each deployed agent.
