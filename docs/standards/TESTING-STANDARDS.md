# Testing Standards

## Test layers
1. **Unit tests:** deterministic logic, schemas, policy decisions and adapters with controlled fixtures.
2. **Contract tests:** tool/service request and response schemas, including errors and version assumptions.
3. **Integration tests:** real service behavior in an explicitly approved environment.
4. **Security tests:** authentication, authorization, injection, secret handling and forbidden side effects.
5. **Failure tests:** timeouts, throttling, partial failures, stale data, malformed output and dependency outages.
6. **Agent evaluations:** task success, evidence grounding, tool selection, safety, uncertainty and cost.
7. **Operational validation:** deployment, health, rollback, backup/restore where relevant, and teardown.

## Evidence
Document exact commands, environment assumptions, test counts and outcomes. Distinguish tests skipped, mocked, locally executed and run against AWS. Do not present mocked tests as integration tests.

## Test data
Use synthetic or sanitized data. Keep fixtures deterministic and avoid real customer information or secrets.

## Acceptance
Define acceptance criteria before implementation. Passing a test suite is necessary but is not, by itself, proof of production readiness.
