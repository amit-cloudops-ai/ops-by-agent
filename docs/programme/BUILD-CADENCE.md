# Build Cadence

## Target rhythm
Target one useful, independently testable agent build or release every 48–72 hours where scope permits. This is a delivery rhythm, not a deadline that overrides safety or quality.

## Typical cycle
1. **Define and research:** confirm project approval, user/problem, alternatives, scope, non-goals and acceptance criteria.
2. **Design:** document architecture, trust boundaries, integrations, IAM/RBAC, approval, AWS/model cost, tests and teardown.
3. **Implement:** build a real operational workflow with narrow, typed, validated tools and tests.
4. **Deploy and validate:** deploy to approved AWS environment; test normal, failure and authorization scenarios; capture evidence; monitor cost.
5. **Document and close:** update status, limitations and next steps; publish only demonstrated capabilities; terminate temporary resources and verify cleanup; prepare a new-chat handoff.

## When scope is too large
Split work into independently useful releases with their own acceptance criteria. Do not count unfinished subcomponents as a completed agent or skip tests/deployment evidence to preserve cadence.

## New-chat handoff
Each project must leave enough repository context for a fresh conversation to continue without chat history: approved scope, current state, exact commands, tested behavior, outstanding defects, decisions, AWS resource state and next concrete task.
