# ExpenseLedger V2 — Naming Conventions

## .NET
- Projects: `ExpenseLedger.Api`, `ExpenseLedger.Application`, `ExpenseLedger.Domain`.
- Classes: PascalCase.
- Methods/properties: PascalCase.
- Private fields: `_camelCase`.
- Interfaces: `I` + PascalCase.
- Async methods: suffix `Async`.
- Commands: `<Verb><Noun>Command`.
- Queries: `Get<Noun>Query` / `List<Noun>Query`.
- Handlers: matching request + `Handler`.
- Validators: matching request + `Validator`.

## Blazor
- Components: `LedgerXxx.razor`.
- Page route folder: feature name; page file `Index.razor` unless a different route requires otherwise.
- Scoped CSS: same basename with `.razor.css`.
- Event handlers: `HandleXxx`, `OpenXxx`, `CloseXxx`, `SaveXxxAsync`.

## API
- Resource names are plural and lowercase in routes.
- IDs use clear names such as `categoryId`, `productId`, `expenseId`.

## Redis
Keys follow `expensebook:{feature}:{scope}`.

## Database
Tables use consistent plural naming chosen by the EF Core model conventions; constraints and indexes use predictable prefixes.