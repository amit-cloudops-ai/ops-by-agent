# Ops by Agent

**Building AI agents for real-world operations engineering.**

Ops by Agent is an open-source engineering programme exploring how AI agents can help engineers investigate, understand and improve complex infrastructure operations.

The focus is practical engineering: real cloud environments, operational workflows, controlled tool access, measurable evaluation and production-minded implementation.

This is not a collection of LLM wrappers or prompt-only demonstrations. Each release is designed around a concrete engineering problem and evaluated against the operational task it is intended to support.

## What we're building toward

AI agents that work with real infrastructure and engineering tools to help with infrastructure discovery, troubleshooting, security and reliability analysis, deployment workflows, observability, incident response and cloud platform operations.

The repository evolves through independently documented and tested releases. New capabilities appear here as they are built and validated.

## Engineering principles

- **Real infrastructure:** AWS is the deployment and validation target, not merely an optional final demo.
- **Human control:** Infrastructure-changing operations require explicit authorization and appropriate approval.
- **Security by design:** Least-privilege IAM, scoped permissions, secure configuration and auditable actions.
- **Evidence before conclusions:** Findings are grounded in tool outputs and observable state; uncertainty is explicit.
- **Testable engineering:** Unit tests, integration tests, failure scenarios and agent evaluations are part of the process.
- **Cost accountability:** AWS cost is estimated before deployment, monitored during use and verified during teardown.
- **Useful documentation:** Every release should help another engineer understand, reproduce, evaluate and learn from it.

## Technology

The programme evaluates technologies across Amazon Web Services, Kubernetes and Amazon EKS, Amazon Bedrock, Python, infrastructure automation, Model Context Protocol (MCP), agent orchestration, observability, security and deployment tooling.

Technology choices are documented with alternatives and trade-offs. The presence of a technology here does not imply every project uses it.

## How development works

Each project follows an independently testable build cycle:

1. Define the operational problem and research existing solutions.
2. Document architecture, security boundaries and AWS cost.
3. Implement the agent and controlled tool integrations.
4. Deploy and validate it in AWS.
5. Evaluate behavior, document limitations and verify teardown.
6. Publish implementation details and learning resources.

A local test, an AWS deployment and production readiness are different levels of validation. We report each honestly.

## Explore the repository

- `docs/` — engineering standards, architecture, research and programme documentation
- `agents/` — released agent implementations
- `infrastructure/` — infrastructure-as-code and cloud resources
- `deployment/` — deployment configurations and policies
- `tests/` — automated tests and evaluation scenarios
- `scripts/` — development, deployment, verification and teardown utilities

Directories and capabilities are introduced as they become useful; there are no empty placeholders for unfinished work.

## Current status

**Programme approved. Repository foundation being established. No agent release has been declared complete yet.**

Individual project releases will appear here only after implementation and validation milestones have been demonstrated.

## Learn and contribute

This repository is intended to be useful to engineers learning about AI agents, cloud infrastructure, Kubernetes, DevOps and SRE practices. Start with the documentation, inspect the implementation, reproduce the tests and review the design decisions.

See [CONTRIBUTING.md](CONTRIBUTING.md) for contribution guidelines and [SECURITY.md](SECURITY.md) for responsible security reporting.

## License

Licensed under the [Apache License 2.0](LICENSE).
