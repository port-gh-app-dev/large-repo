# Security Logging Rules

- Log security-relevant events: auth attempts, privilege changes, access denials, token events, sensitive data access.
- Use structured logs with timestamp, actor, action, resource, result, and correlation/request ID.
- Never log secrets, passwords, tokens, private keys, or full PII payloads.
- Redact sensitive fields consistently before writing logs.
- Protect log pipelines against tampering with append-only or integrity controls.
- Ensure synchronized clocks (NTP) for accurate event sequencing.
- Define retention and deletion policies based on compliance and incident response needs.
- Configure alerts for suspicious patterns (brute force, privilege escalation, anomaly spikes).
- Restrict log access with least privilege and audit log access itself.
- Periodically test logging coverage during incident simulations.
