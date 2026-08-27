# API — Create Command or Query

Create a complete CQRS request for ExpenseLedger.

For commands:
- Validate business input.
- Use MediatR IRequest/IRequestHandler.
- Apply domain rules.
- Persist through Application abstractions.
- Invalidate relevant Redis cache entries after successful mutation.
- Return a typed result/response.

For queries:
- Use read-focused DTOs.
- Avoid loading unnecessary entity graphs.
- Support filtering, sorting and pagination where appropriate.
- Use Redis when the query is cacheable.

Always include validator, handler, DTO/result and tests as appropriate.
Follow existing feature folder conventions and return complete files with exact paths.
