# Create Report Prompt

Create a reporting or analytics feature for ExpenseLedger.

Requirements:
- Define the report as a read-focused application use case.
- Use CQRS queries and MediatR handlers.
- Keep aggregation logic out of controllers and Blazor components.
- Apply Redis caching only where the report is safe and worthwhile to cache, with explicit invalidation rules.
- Return stable DTOs designed for reporting rather than exposing entities.
- Provide API endpoints documented through Scalar/Swagger.
- Build Blazor views with existing Ledger cards, charts, tables and filters.
- Support Light/Dark Notebook themes, responsive layouts and loading/empty/error states.
- Ensure monetary values, date ranges and timezone behavior are explicit and correct.
- Add tests for filters, aggregates, edge cases and authorization.
- Return complete files with exact paths when code is requested.
