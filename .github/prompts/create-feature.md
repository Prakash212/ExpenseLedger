# Create Feature Prompt

Implement a complete ExpenseLedger feature using the existing repository architecture and conventions.

## Inputs
- Feature name: {{FEATURE_NAME}}
- Primary entity: {{ENTITY_NAME}}
- Business rules: {{BUSINESS_RULES}}
- User stories: {{USER_STORIES}}

## Required analysis
1. Inspect the repository for analogous features and existing shared components.
2. Reuse existing patterns before introducing new abstractions.
3. Preserve Clean Architecture dependency direction.
4. Do not duplicate reusable UI components or CSS.

## Required deliverables
- Domain entities/value objects and business rules.
- Application CQRS commands and queries.
- MediatR handlers.
- FluentValidation validators.
- DTOs and mappings.
- Persistence/EF Core configuration and migration when needed.
- Infrastructure integrations when needed.
- Redis caching and invalidation when appropriate.
- API endpoints with consistent response contracts.
- Scalar/Swagger documentation.
- Blazor UI using existing Ledger components.
- MAUI Android implementation/contracts when applicable.
- Unit, integration, API, and component tests appropriate to the feature.

## Quality requirements
- Async APIs with CancellationToken support.
- SOLID and readable code.
- No magic strings.
- Correct logging and error handling.
- ProblemDetails for API failures.
- Light/Dark Notebook theme compatibility.
- Validation must not cause layout shifts.
- Security and authorization must be considered.

## Output
When code is requested, provide complete files with exact repository paths. Do not provide partial patches unless explicitly requested.
