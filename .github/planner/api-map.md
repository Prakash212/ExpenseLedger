# ExpenseLedger V2 — API Map

## API Principles
- ASP.NET Core 10.
- Thin endpoints; business orchestration lives in Application.
- MediatR dispatches commands and queries.
- Use ProblemDetails for failures.
- Scalar is the primary interactive API UI; Swagger/OpenAPI remains available for tooling compatibility.
- Include correlation/trace information in responses and logs.

## Feature Groups
- `/api/categories`
- `/api/product-groups`
- `/api/products`
- `/api/expenses`
- `/api/dashboard`
- `/api/reports`
- `/api/budgets`
- `/api/notifications`

## CRUD Convention
- GET collection
- GET by identifier
- POST create
- PUT/PATCH update according to feature semantics
- DELETE remove

## Response Envelope
```json
{
  "success": true,
  "message": "",
  "data": {},
  "errors": [],
  "traceId": ""
}
```

## API Rules
- Validate at the application boundary.
- Map domain/application errors into stable HTTP responses.
- Never expose EF Core entities directly.
- Use Contracts DTOs between API and clients.
- Support CancellationToken.
- Document security requirements in OpenAPI.
