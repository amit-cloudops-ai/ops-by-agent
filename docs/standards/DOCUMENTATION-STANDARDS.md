# Documentation Standards

## Reader-first requirement
Every public document should answer a real reader question. Avoid empty stubs, vague aspirations, unexplained acronyms and unverified claims.

## Project documentation baseline
Each approved project should maintain, as applicable:
- `README.md`: purpose, supported workflows, prerequisites, quick start and links.
- `PROJECT-PLAN.md`: scope, non-goals, acceptance criteria and milestones.
- `ARCHITECTURE.md`: components, data flows, trust boundaries and decisions.
- `ALTERNATIVES.md`: existing tools, comparison and differentiation.
- `SECURITY.md`: threat model, permissions, data handling and controls.
- `TESTING.md`: exact test commands, scenarios and evidence.
- `EVALUATION.md`: task-level agent evaluation and results.
- `DEPLOYMENT.md`: AWS deployment, configuration and validation.
- `COST-ESTIMATE.md`: assumptions, estimates, actual usage and alerting.
- `OPERATIONS.md`: monitoring, incidents, rollback and maintenance.
- `IMPLEMENTATION-STATUS.md`: evidenced status and limitations.
- `HANDOFF.md`: self-contained continuation instructions for a new chat.
- `NEXT-STEPS.md`: one prioritized next action and remaining work.

Files may be combined for small projects, but their information must remain discoverable.

## Evidence and accuracy
Label diagrams, screenshots and benchmarks with implementation version and capture date. Distinguish planned architecture from deployed architecture. Link sources. Avoid fabricated badges and unmeasured performance claims.

## Cross-chat continuity
The repository is the source of truth. Keep status, decisions, exact commands, resource state and blockers current so a new conversation can continue without hidden chat history.
