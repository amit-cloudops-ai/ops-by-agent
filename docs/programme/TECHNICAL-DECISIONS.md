# Programme Technical Decisions

This register records programme-level decisions accepted in the master blueprint. Project-level choices still require validation and ADRs.

| Area | Programme direction | Qualification |
|---|---|---|
| Product | AI agents are the product | Each agent addresses a concrete operational task |
| First domain | Kubernetes | Later domains: DevOps, Cloud, SRE and Platform Engineering |
| Cloud target | AWS | Local work does not replace AWS validation |
| Kubernetes target | Amazon EKS | Verify project scope and account/region availability |
| Model inference | Amazon Bedrock | Validate model, region, data policy, quota and cost |
| Language | Python initial candidate | Select version/libraries per project |
| Agent framework | Evaluate LangGraph, Bedrock AgentCore and direct orchestration | No blanket commitment |
| Kubernetes integration | Kubernetes API/client, AWS EKS APIs and MCP where appropriate | Recheck EKS MCP maturity |
| Infrastructure as code | Terraform candidate | Use where it improves repeatability and review |
| Source control | Public GitHub repository | No secrets or sensitive operational data |
| Licensing | Apache License 2.0 | Third-party model, data and dependency licenses remain separate |
| Build cadence | Target useful release every 48–72 hours | Quality gates override cadence |
| Approval | Programme approved; each agent individually approved | No project implementation before approval |
| AWS governance | Cost review and teardown plan before provisioning | Budgets are alerts, not hard caps |
| Public reveal | Add agent to root README after release criteria | Full planning register is separate documentation |

Material changes must be recorded in an ADR and reflected in standards and handoff documents.
