# Create Background Job Prompt

Create a reliable background job for ExpenseLedger.

Requirements:
- Use the existing hosted/background-service or worker abstraction if present.
- Keep business operations in Application handlers/services, not in the worker itself.
- Support cancellation and graceful shutdown.
- Prevent duplicate execution where the operation is not idempotent.
- Use structured logging and correlation information.
- Use Redis/queues only through existing abstractions.
- Define retry, failure and observability behavior explicitly.
- Add tests for scheduling/orchestration and the underlying business operation.
- Return complete files with exact paths when code is requested.
