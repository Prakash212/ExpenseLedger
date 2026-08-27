# UI — Create Modal

Create or update an ExpenseLedger modal using the existing LedgerDialog component.

Requirements:
- Use LedgerDialog, LedgerTextBox, LedgerSelect, LedgerButton and LedgerButtonGroup where appropriate.
- Separate add and edit state cleanly.
- Validation must reserve space and never move controls when messages appear.
- Footer actions remain predictable and keyboard accessible.
- Support loading/processing state and prevent duplicate submissions.
- Preserve Light/Dark Notebook theme parity.
- No page-specific replacement for shared dialog styling.

Verify close, cancel, save, validation, API failure and success notification flows.
Return complete files with exact paths.
