# Tests — Create Integration Tests

Create integration tests for an ExpenseLedger feature across real application boundaries.

Use the existing test host, configuration and database strategy.

Cover:
- API endpoint to MediatR handler.
- Validation and authorization.
- Persistence behavior.
- Redis behavior where part of the feature contract.
- Standard response and ProblemDetails behavior.
- Important transaction and concurrency paths.

Keep tests isolated and repeatable. Never rely on developer-local state. Return complete files with exact paths.
