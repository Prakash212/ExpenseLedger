# Create Notification Prompt

Implement a user notification in ExpenseLedger using the existing notification service/component system.

Requirements:
- Inspect current NotificationService and Ledger notification components before coding.
- Reuse the shared toast/notification surface; do not create a page-specific alert system.
- Support success, info, warning and error semantics.
- Keep Light/Dark Notebook styling consistent.
- Use accessible roles, readable contrast and non-blocking interaction.
- Ensure async operations report success only after the underlying operation completes.
- Do not leak sensitive exception details to users.
- Add tests for notification triggering where practical.
- Return complete files with exact paths when code is requested.
