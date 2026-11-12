# Shared Agent Architecture

## Design goal
Reuse only proven foundations. Each agent should remain independently understandable, testable and deployable. Shared code should reduce duplicated security and operational work without coupling unrelated releases.

## Candidate shared capabilities
- Identity and request context.
- Tool registry and typed tool adapters.
- Policy evaluation and approval records.
- Model invocation abstraction and usage accounting.
- Task state and persistence where required.
- Structured evidence and provenance.
- Audit events and correlation identifiers.
- Evaluation harness and scenario fixtures.
- Telemetry, health checks and structured errors.

These are candidates, not a requirement to build a shared platform before the first agent.

## Agent execution lifecycle
1. Authenticate caller and establish principal context.
2. Authorize the requested operation.
3. Create a task record and correlation identifier.
4. Gather only required context.
5. Ask the model to reason over bounded, typed context.
6. Validate proposed tool calls against schemas and policy.
7. Execute read-only tools or request approval for side effects.
8. Preserve raw evidence and source metadata.
9. Validate response structure and cite evidence in the result.
10. Record outcome, evaluation signals, token usage and errors.

## Tool adapter contract
Adapters should declare tool name/version, purpose, supported resource types, input/output schemas, required IAM and Kubernetes permissions, side-effect classification, timeout/retry behavior, audit fields and error taxonomy.

## Isolation and failure handling
Treat model output, external resource data, logs and repository content as untrusted. Defend against prompt injection in retrieved content. Prevent authorization or context from leaking across tasks. Bound recursion, tool calls, payload sizes and execution time.

## Human approval
An approval decision is bound to the exact proposed action, target, parameters and expiry. A changed action requires new approval. Approval is not inferred from prior conversation or model confidence.
