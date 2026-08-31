# Create Docker Service Prompt

Add or modify a containerized ExpenseLedger service.

Requirements:
- Inspect the existing Docker and solution structure first.
- Use supported .NET container patterns for the repository's target framework.
- Keep configuration environment-driven; never hard-code secrets.
- Define health checks and service dependencies appropriately.
- Preserve local development and production parity as far as practical.
- Update docker-compose configuration, Dockerfiles, ignore files and documentation when required.
- Integrate SQL Server, Redis, observability and application services without coupling Domain/Application to containers.
- Verify startup ordering, persistence volumes, ports and environment variables.
- Return complete files with exact paths when code is requested.
