<!--
Ops by Agent — public project homepage.
Only add an agent to the Releases section after its implementation and validation evidence is published.
-->

<div align="center">

# ⚙️ OPS BY AGENT

### BUILDING AI AGENTS FOR REAL-WORLD OPERATIONS ENGINEERING

**From infrastructure signals to evidence-backed operational insight.**

[![AWS](https://img.shields.io/badge/Cloud-AWS-232F3E?logo=amazonaws&logoColor=white)](https://aws.amazon.com/)
[![Kubernetes](https://img.shields.io/badge/Domain-Kubernetes-326CE5?logo=kubernetes&logoColor=white)](https://kubernetes.io/)
[![Amazon Bedrock](https://img.shields.io/badge/AI-Amazon%20Bedrock-693CC5?logo=amazonaws&logoColor=white)](https://aws.amazon.com/bedrock/)
[![Python](https://img.shields.io/badge/Language-Python-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)

[**Follow the build on LinkedIn**](https://www.linkedin.com/in/amit-cloudops-ai/) · [**Explore the engineering standards**](docs/standards/PRODUCTION-READINESS.md) · [**Read the contribution guide**](CONTRIBUTING.md)

</div>

---

## The idea

Cloud operations generate more signals than engineers can reasonably correlate by hand: cluster state, events, logs, deployments, metrics, policies and infrastructure configuration.

**Ops by Agent explores how purpose-built AI agents can help engineers investigate those systems—with evidence, bounded tools and human control.**

The product is the agent. Kubernetes is the first operational domain. AWS is the target environment for cloud deployment and validation.

This is an engineering programme, not a gallery of prompt wrappers. Each release is built around a specific operational job and must demonstrate what it can and cannot do.

## How we approach operations

<table>
<tr>
<td width="50%" valign="top">

### 🔎 Observe before reasoning

Agents gather authorized infrastructure evidence before forming conclusions. Findings should reference the underlying resources, events or telemetry.

</td>
<td width="50%" valign="top">

### 🧠 Reason with boundaries

Models help interpret context and plan investigation. Deterministic application code enforces identity, schemas and permissions.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🛡️ Keep operators in control

Read-only access is the default. Any infrastructure-changing action must be scoped, authorized and explicitly approved.

</td>
<td width="50%" valign="top">

### 📊 Evaluate the actual outcome

We test task success, evidence quality, tool selection, failure handling, safety, latency and inference cost—not just whether the model responds.

</td>
</tr>
</table>

## Engineering principles

| Principle | What it means in practice |
|---|---|
| **AWS-first validation** | AWS-dependent behavior is deployed and tested in AWS; local tests are not presented as cloud integration tests. |
| **Least privilege** | Dedicated IAM roles, narrow Kubernetes RBAC and short-lived credentials. |
| **Human authorization** | The model cannot grant itself permissions; side effects require explicit approval. |
| **Evidence over confidence** | Facts, hypotheses, recommendations and unknowns are clearly separated. |
| **Operational resilience** | Timeouts, bounded retries, structured errors, telemetry and recovery paths are designed deliberately. |
| **Cost accountability** | Estimate before provisioning, monitor during use and verify teardown. |
| **Honest reporting** | Implemented, tested, AWS-deployed, validated and production-ready are separate claims. |

## Releases

> New agent implementations will be introduced here one release at a time. This section intentionally shows only work that has reached a documented, evidence-backed release.

**No agent release is being claimed yet.** The repository foundation and engineering standards are in place; the first implementation is the next milestone.

## The engineering lifecycle

```text
Operational problem
       ↓
Alternatives research
       ↓
Architecture + threat boundaries + cost estimate
       ↓
Agent implementation + automated tests
       ↓
AWS deployment + integration validation
       ↓
Evaluation + documentation + verified teardown
       ↓
Evidence-backed release
```

Each project is developed as an independently testable build, targeting a 48–72-hour cycle when scope allows. Quality gates take precedence over the calendar.

## Technology landscape

<div align="center">

[![Amazon EKS](https://img.shields.io/badge/Amazon%20EKS-FF9900?logo=amazoneks&logoColor=white)](https://docs.aws.amazon.com/eks/)
[![Amazon Bedrock](https://img.shields.io/badge/Amazon%20Bedrock-232F3E?logo=amazonaws&logoColor=white)](https://docs.aws.amazon.com/bedrock/)
[![Terraform](https://img.shields.io/badge/Terraform-7B42BC?logo=terraform&logoColor=white)](https://developer.hashicorp.com/terraform/docs)
[![MCP](https://img.shields.io/badge/Model%20Context%20Protocol-222222)](https://modelcontextprotocol.io/)
[![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)](https://docs.python.org/3/)

</div>

The exact stack is selected per project. LangGraph, Bedrock AgentCore, Kubernetes APIs, MCP interfaces and other integrations are evaluated against security, reliability, maintainability, maturity and cost. A technology badge is not a claim that every component is already implemented.

## Learn from the repository

This project is intended to be useful to engineers who want to understand how agentic systems interact with real infrastructure—not just see a finished demo.

| Start here | What you will learn |
|---|---|
| [System architecture](docs/architecture/SYSTEM-ARCHITECTURE.md) | Agent, model, policy and tool boundaries |
| [AI safety and tool use](docs/standards/AI-SAFETY.md) | How to constrain agent tool access and side effects |
| [IAM and Kubernetes RBAC](docs/standards/IAM-RBAC-STANDARDS.md) | Least-privilege access patterns |
| [Agent evaluation](docs/standards/AGENT-EVALUATION.md) | How we assess agent behavior beyond response quality |
| [Testing standards](docs/standards/TESTING-STANDARDS.md) | Unit, contract, integration and failure testing |
| [AWS cost management](docs/operations/COST-MANAGEMENT.md) | Estimation, monitoring and teardown discipline |
| [Production-readiness criteria](docs/standards/PRODUCTION-READINESS.md) | Evidence required before making operational claims |

For the programme's complete planning register and technical decisions, see [programme documentation](docs/programme/PROGRAMME-OVERVIEW.md). It is planning context, not a list of announced releases.

## Contributing

Technical feedback, reproducible issues, documentation improvements and thoughtful contributions are welcome.

- Read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a pull request.
- Report vulnerabilities privately using the process in [SECURITY.md](SECURITY.md).
- Follow the [Code of Conduct](CODE_OF_CONDUCT.md).

## About the builder

**Amit Madakatti** — Cloud & DevOps engineering, AI agents and infrastructure automation.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/amit-cloudops-ai/)

Follow the build-in-public series: **Ops by Agent**.

---

<div align="center">

**Built in public. Grounded in evidence. Designed for real operations.**

Licensed under [Apache License 2.0](LICENSE).

</div>
