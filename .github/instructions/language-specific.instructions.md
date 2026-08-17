# Language-Specific Instructions

## JavaScript / TypeScript
- Enable strict compiler/lint settings and keep `any` usage minimal.
- Use runtime schema validation for external input.
- Avoid blocking operations in request paths.

## Python
- Use type hints for public interfaces.
- Prefer context managers for resources (files, sockets, DB sessions).
- Avoid dynamic `exec`/`eval` on untrusted input.

## Go
- Always check returned errors.
- Use contexts for cancellation/timeouts in I/O boundaries.
- Guard concurrent map/state access.

## Java / Kotlin
- Prefer immutable objects for shared data flows.
- Use bean validation for request DTOs.
- Close resources via try-with-resources/use blocks.

## SQL
- Parameterize queries and enforce least-privilege DB roles.
- Bound result sets with pagination and sensible defaults.
- Version schema changes with repeatable migration tooling.
