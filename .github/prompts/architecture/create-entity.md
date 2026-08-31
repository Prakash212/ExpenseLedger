# Create Entity Prompt

Design or add a Domain entity for ExpenseLedger.

Requirements:
- Inspect existing Domain entities, base types, value objects and conventions first.
- Model invariants and business behavior in Domain, not in API or UI.
- Use strong types/value objects when they improve correctness.
- Consider ownership, lifecycle, concurrency and audit requirements.
- Define relationships without leaking EF Core concerns into Domain.
- Add EF Core configuration separately in Persistence.
- Add unit tests for business rules and invariants.
- Return complete files with exact paths when code is requested.
