# Create Cache Handler Prompt

Implement caching for the requested ExpenseLedger query or feature using the existing Redis abstraction.

Requirements:
- Inspect existing cache interfaces, serializers, key conventions and expiration policies first.
- Keep caching concerns outside the Domain layer.
- Use cancellation-aware async operations.
- Define a deterministic cache key and document ownership of the key.
- Invalidate affected keys after successful mutations.
- Prevent stale data from becoming authoritative after writes.
- Handle Redis unavailability gracefully according to existing application policy.
- Add tests for cache hit, miss, invalidation and fallback behavior where applicable.
- Do not introduce a second cache abstraction when one already exists.
- Return complete files with exact paths when code is requested.
