# Contributing

Thank you for helping make Ops by Agent useful, reproducible, secure and technically accurate.

## Before starting
- Read the README and relevant standards in `docs/standards/`.
- Open an issue before significant features or architectural changes.
- Do not begin a new agent or expand project scope without maintainer approval.
- Evaluate existing tools first; prefer integration over unnecessary reinvention.

## Workflow
1. Open or select an issue describing the problem and acceptance criteria.
2. Discuss scope and design for non-trivial changes.
3. Create a focused branch from `main`.
4. Implement the smallest complete, testable change.
5. Add or update tests and documentation.
6. Run relevant checks and record exact commands/results.
7. Open a pull request with rationale, evidence, security impact and operational impact.

## Pull request expectations
Include the problem, implementation, design decisions, tests actually run, AWS services/resources affected, security and data-handling implications, cost estimate and teardown plan (if infrastructure is involved), limitations and follow-up work.

Keep changes focused. Do not commit secrets, credentials, personal data, customer information or unexplained binaries.

## Engineering expectations
Use least privilege, validate inputs and tool outputs, make side effects explicit, default to read-only, require approval for mutations, add regression coverage and document safe operation and cleanup.

## Tests and evidence
Separate local, mocked and AWS integration tests. Tests requiring AWS must not silently create billable resources.

## Licensing
By submitting a contribution, you agree it may be distributed under Apache License 2.0. Ensure you have the right to contribute it and properly attribute third-party material.
