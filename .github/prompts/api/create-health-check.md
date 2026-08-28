# Create Health Check Prompt

Implement health checks for the requested ExpenseLedger dependency or service.

- Inspect existing health-check registration and naming conventions.
- Use ASP.NET Core HealthChecks APIs and existing infrastructure abstractions.
- Include meaningful checks for SQL Server, Redis and dependent services where relevant.
- Keep health endpoints unauthenticated only when consistent with deployment/security policy.
- Distinguish readiness and liveness when the application's operational model needs both.
- Avoid expensive checks on high-frequency probes.
- Add tests for registration/configuration where practical.
- Return complete files with exact paths when code is requested.
