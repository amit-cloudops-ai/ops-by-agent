# Programme Overview

## Purpose
Ops by Agent is a long-running open-source engineering programme to build practical AI agents for DevOps, Cloud, Site Reliability Engineering and Platform Engineering.

The central product is the AI agent. Kubernetes is the first operational domain used to develop and validate those agents. The programme will subsequently explore other DevOps and cloud domains.

## Intended audience
- DevOps and platform engineers.
- Cloud and SRE practitioners.
- Engineers learning agentic AI in operational environments.
- Open-source contributors interested in infrastructure and reliability.

## Outcomes
Each project should deliver an independently testable agent; a clear operational problem statement; documented architecture and threat model; implementation and test evidence; deployment and operational instructions; AWS cost visibility; and verified cleanup procedures.

## Principles
1. Solve an identifiable operational problem.
2. Research existing tools and integrate them where appropriate.
3. Ground conclusions in evidence from authorized tools.
4. Keep permissions narrow and default to read-only operations.
5. Put human approval in front of material side effects.
6. Evaluate agent behavior, not only API success.
7. Document limitations and failure modes.
8. Use AWS as the deployment and validation target.
9. Estimate, monitor and clean up every billable resource.
10. Publish project details only when ready to be shown.

## Project approval
The overall programme direction and portfolio are approved. Individual projects still require explicit approval before implementation. Approval confirms scope, acceptance criteria, integrations, AWS architecture, estimated cost and teardown plan.

## Build cadence
Target one useful, independently testable release every 48–72 hours where scope permits. This is a target, not a reason to skip security, validation or documentation. Split large work into meaningful releases.

## Status vocabulary
- **Proposed:** under research; not approved for implementation.
- **Approved:** scope accepted; implementation may begin.
- **Building:** implementation in progress.
- **Implemented:** code exists; validation may remain.
- **Locally tested:** specified local tests passed.
- **AWS deployed:** deployed to the documented AWS environment.
- **AWS validated:** deployment and operational scenarios tested with evidence.
- **Released:** documentation and release criteria are complete.
- **Production-ready:** all production-readiness criteria met for a defined operating context.

These states are not interchangeable.
