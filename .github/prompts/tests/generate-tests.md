# Generate Tests Prompt

Generate production-quality tests for ExpenseLedger.

Cover the requested behavior at the appropriate level:
- Domain unit tests for business rules.
- Application handler and validator tests.
- API integration tests.
- Blazor component tests when applicable.
- MAUI view-model tests when applicable.

Use deterministic data, meaningful names, Arrange/Act/Assert structure, cancellation behavior, validation failures, authorization, cache interactions and error paths where relevant.
Do not change production code merely to make tests pass unless the design genuinely requires it.
Return complete test files with exact paths when code is requested.
