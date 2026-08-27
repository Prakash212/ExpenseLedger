# ExpenseLedger V2 — CQRS Feature Map

## Purpose
This document defines the standard feature organization for ExpenseLedger.

## Feature Structure
```text
Features/
  Categories/
    Commands/
      CreateCategory/
      UpdateCategory/
      DeleteCategory/
    Queries/
      GetCategories/
      GetCategoryById/
    DTOs/
    Validators/
    Mappings/
  Products/
  ProductGroups/
  Expenses/
  Dashboard/
  Budgets/
  Reports/
```

## Request Flow
```text
UI -> API -> MediatR -> Pipeline Behaviors -> Handler -> Persistence/Infrastructure -> Result
```

## Commands
Commands change state and return the smallest useful result. Every command must have a handler and validator when validation is required.

## Queries
Queries are read-only and must not mutate application state. Query handlers should use projections where practical.

## Pipeline Behaviors
1. Validation
2. Logging / correlation
3. Performance measurement
4. Caching where applicable
5. Exception normalization

## Feature Rules
- Keep domain rules in Domain.
- Keep orchestration in Application handlers.
- Do not place EF Core access in UI or API endpoints.
- API endpoints should dispatch requests through MediatR.
- Mutations that affect cached data must invalidate related Redis keys.

## Naming
- `CreateExpenseCommand`
- `CreateExpenseCommandHandler`
- `CreateExpenseCommandValidator`
- `GetExpensesQuery`
- `GetExpensesQueryHandler`
