# ExpenseLedger V2 — Folder Rules

## Solution Layout
```text
src/
  ExpenseLedger.Api/
  ExpenseLedger.Application/
  ExpenseLedger.Domain/
  ExpenseLedger.Infrastructure/
  ExpenseLedger.Persistence/
  ExpenseLedger.Contracts/
  ExpenseLedger.SharedKernel/
  ExpenseLedger.Blazor/
  ExpenseLedger.Mobile/
tests/
  ExpenseLedger.Application.Tests/
  ExpenseLedger.Api.Tests/
  ExpenseLedger.Integration.Tests/
```

## Ownership
- Domain: business rules, entities, value objects, domain events.
- Application: CQRS, handlers, validators, abstractions, mappings.
- Persistence: EF Core, DbContext, configurations, migrations, seeds.
- Infrastructure: Redis, logging, external services, storage.
- API: HTTP endpoints, middleware, authentication/authorization, OpenAPI.
- Blazor: presentation only; consume contracts/API.
- Mobile: MAUI presentation and client state.

## Rules
- Respect dependency direction.
- Do not place database access in UI projects.
- Do not reference Infrastructure/Persistence from Domain.
- Keep feature code cohesive and colocated under Application feature folders.
- Shared UI components live in the shared Ledger component area.
- Shared UI styling belongs to component-scoped CSS.
