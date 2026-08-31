# Input Validation Rules

- Treat all external input as untrusted (HTTP, queues, files, webhooks).
- Validate at system boundaries using schema-based validators.
- Enforce types, ranges, length, format, and required fields explicitly.
- Reject unknown fields for sensitive endpoints (fail closed).
- Normalize canonical forms before validation when relevant (Unicode, case, whitespace).
- Separate validation from business logic to ensure consistent enforcement.
- Apply contextual output encoding (HTML, URL, SQL, shell) at sink points.
- Use allowlists for enum-like fields and identifiers.
- Return structured validation errors without exposing internals.
- Add negative tests for malformed, oversized, and malicious payloads.
