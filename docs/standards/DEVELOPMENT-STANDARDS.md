# Development Standards

## General
- Prefer small, cohesive and independently testable changes.
- Use supported language/runtime versions and pin dependencies appropriately.
- Keep configuration explicit and validate it at startup.
- Use structured logging; never log secrets or unnecessary sensitive data.
- Provide clear error types and actionable diagnostics.
- Avoid hidden side effects and implicit cloud provisioning.

## Python baseline
Use type hints, focused modules, deterministic tests and a consistent formatter/linter selected by the project. Keep dependency groups clear. Pin production dependencies and maintain a lock/constraints strategy appropriate to the package manager.

## API and CLI design
Validate inputs, use stable schemas, document exit codes and errors, and avoid exposing stack traces to callers. Make destructive operations opt-in and explicit.

## Configuration
Commit safe examples such as `.env.example` with placeholders only. Never commit credentials or production configuration.

## Dependencies
Evaluate maintenance, licensing, security posture, transitive dependencies, release maturity and compatibility. Use automated updates and vulnerability scanning where available.

## Documentation
A project is incomplete if another engineer cannot understand its purpose, configure it safely, test it, deploy it, operate it and clean it up.
