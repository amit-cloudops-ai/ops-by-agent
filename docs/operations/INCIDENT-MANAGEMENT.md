# Incident Management

## Purpose
Consistent response for incidents affecting agent services, AWS deployments, security, data or operational workflows.

## First response
1. Protect people, data and infrastructure.
2. Stop unsafe automation and revoke compromised credentials.
3. Establish scope, impact and current evidence.
4. Notify responsible maintainers and affected stakeholders.
5. Preserve relevant logs and audit evidence with sensitive data protected.

## Agent-specific containment
Disable or restrict affected tools, revoke workload permissions if necessary, pause queued actions and invalidate outstanding approvals where safe. Do not allow an impaired agent to continue changing infrastructure.

## Recovery
Restore from trusted artifacts/configuration, rotate secrets, validate permissions, test critical paths and monitor for recurrence. Document residual risk.

## Review
Write a blameless incident record with impact, timeline, contributing factors, detection, response, recovery and follow-up actions. Do not expose credentials or private data in public postmortems.
