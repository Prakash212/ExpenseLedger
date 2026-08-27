# Create Blazor Form Prompt

Create or modify a Blazor form in ExpenseLedger using the existing Ledger component library.

Requirements:
- Inspect existing form pages and control APIs before coding.
- Reuse LedgerTextBox, LedgerSelect, LedgerButton, LedgerDialog and other shared controls.
- Keep API calls behind existing client/service abstractions.
- Use EditForm and validation consistently with repository conventions.
- Ensure validation messages do not move surrounding controls.
- Support processing, success, cancellation and API-error states.
- Support Light/Dark Notebook themes and responsive layouts.
- Avoid inline styles and duplicated page-level control CSS.
- Return complete files with exact paths when code is requested.
