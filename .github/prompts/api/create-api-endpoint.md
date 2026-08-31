# Create API Endpoint

Create a .NET 10 ExpenseLedger API endpoint for `{Feature}` / `{Operation}`.

Requirements:
- Follow Clean Architecture and CQRS.
- Keep endpoint/controller thin.
- Dispatch a MediatR command or query.
- Use Contracts DTOs; never expose EF/domain entities directly.
- Add FluentValidation where applicable.
- Support CancellationToken.
- Return the project's standard result/error model and ProblemDetails on failures.
- Document endpoint metadata for Scalar/OpenAPI/Swagger.
- Apply authorization requirements appropriate to the feature.
- Update Redis cache/invalidation strategy for mutations where needed.
- Add or update tests for happy path, validation, authorization, not-found, and failure paths.

Output exact paths and complete files.