# Create Blazor Page

Create or update a complete ExpenseLedger Blazor page for `{Feature}`.

Requirements:
- Follow `.github/copilot-instructions.md` and planner documents.
- Inspect existing project structure and reuse existing Ledger components before creating anything new.
- Use `LedgerCard`, `LedgerButton`, `LedgerDialog`, `LedgerTextBox`, `LedgerSelect`, `LedgerPageSizeSelect`, `LedgerPagination`, `LedgerSearchBox`, loading and empty-state components where applicable.
- Keep page logic focused on presentation/orchestration; call the API client, never DbContext directly.
- Preserve light/dark Notebook theme parity.
- Use scoped CSS for page-specific composition only.
- Do not duplicate reusable component styles.
- Keep validation space stable and prevent layout shift.
- Provide complete replacement files when modifying existing files.

Output:
1. Exact files to create/modify.
2. Complete contents for each file.
3. Verification checklist.