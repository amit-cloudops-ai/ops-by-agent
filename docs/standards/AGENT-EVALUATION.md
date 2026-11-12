# Agent Evaluation Standard

A successful HTTP response or tool invocation does not prove an agent solved the operational problem safely. Evaluate each agent against representative tasks and failure scenarios.

## Evaluation dimensions
- Task completion and operational correctness.
- Evidence grounding and source attribution.
- Correct tool selection and argument validity.
- Handling missing, stale or contradictory evidence.
- Calibration of uncertainty and safe abstention.
- Resistance to prompt injection in retrieved content.
- Authorization and policy compliance.
- Avoidance of unauthorized side effects.
- Latency, model usage and cost.
- Reproducibility across repeated runs.

## Scenario design
Include normal, ambiguous, adversarial, partially unavailable and negative cases. Each scenario defines inputs, expected observations, forbidden actions, evaluation rubric and pass criteria.

## Evidence quality
Conclusions should point to the resource, event, log, metric or API response supporting them. Separate facts, hypotheses and recommendations.

## Regression
Store versioned evaluation cases and compare results across meaningful code, prompt, model or tool changes. Record model identifier, region, inference settings, tool versions and test date.

## Human review
High-impact operational recommendations require human review. A model self-assessment is not a substitute for independent evidence and policy checks.
