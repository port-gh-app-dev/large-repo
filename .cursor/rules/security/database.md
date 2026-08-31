# Database Security Rules

- Use parameterized queries/prepared statements for all SQL operations.
- Prohibit dynamic query construction from raw user input.
- Apply least-privilege DB accounts per service and environment.
- Use separate read-only and read-write credentials where possible.
- Enable TLS for DB connections in all non-local environments.
- Encrypt sensitive columns at rest (or tokenized/hashed where appropriate).
- Validate pagination/sort/filter fields against allowlists before query usage.
- Add query timeouts and safe limits to prevent expensive full scans.
- Protect against mass assignment in ORM models via explicit allowed fields.
- Back up databases regularly and validate restore procedures.
