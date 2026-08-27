# UI — Create Page

Create or update a complete ExpenseLedger Blazor page for `{Feature}`.

Requirements:
- Follow `.github/copilot-instructions.md` and `.github/planner/ui-design-system.md`.
- Inspect existing pages and reuse established Ledger components.
- Use LedgerCard, LedgerButton, LedgerDialog, LedgerTextBox, LedgerSelect, LedgerPageSizeSelect, LedgerPagination, LedgerSearchBox, loading and empty-state components as applicable.
- Keep presentation/orchestration in Blazor; call API clients, never DbContext directly.
- Preserve Light/Dark Notebook theme parity.
- Use scoped CSS only for page-specific composition.
- Do not duplicate reusable component styles.
- Reserve validation space to prevent layout shift.
- Provide complete replacement files with exact paths.
