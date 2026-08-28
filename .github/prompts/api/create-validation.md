# Create Validation Prompt

Implement validation for the requested ExpenseLedger command, query or input model.

Requirements:
- Inspect existing FluentValidation conventions first.
- Keep domain invariants in Domain and request validation in Application.
- Validate required, range, length, format, uniqueness and cross-field rules where applicable.
- Produce user-friendly validation messages without leaking implementation details.
- Ensure Blazor validation integrates cleanly with the existing Ledger controls.
- Reserve validation space in UI layouts so controls do not shift when messages appear.
- Cover valid, invalid and boundary cases with tests.
- Return complete files with exact paths when code is requested.
