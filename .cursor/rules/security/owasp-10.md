# OWASP Top 10 Mapping Rules

These rules map implementation checks to OWASP Top 10 categories (2021):

1. **A01: Broken Access Control**
   - Enforce server-side authorization on every protected action.
   - Deny by default and verify ownership/tenant boundaries.

2. **A02: Cryptographic Failures**
   - Use approved algorithms and key sizes.
   - Enforce TLS and secure key management/rotation.

3. **A03: Injection**
   - Use parameterized queries and safe command/process APIs.
   - Sanitize and encode according to context.

4. **A04: Insecure Design**
   - Perform threat modeling for new features.
   - Add abuse-case tests for critical flows.

5. **A05: Security Misconfiguration**
   - Harden defaults, disable debug in production, and set secure headers.
   - Maintain environment-specific secure baselines.

6. **A06: Vulnerable and Outdated Components**
   - Continuously scan dependencies and patch critical/high findings quickly.
   - Pin versions and avoid unmaintained libraries.

7. **A07: Identification and Authentication Failures**
   - Implement strong credential policies and session management.
   - Protect against brute force and credential stuffing.

8. **A08: Software and Data Integrity Failures**
   - Verify artifact integrity and signatures in CI/CD.
   - Restrict unsafe deserialization patterns.

9. **A09: Security Logging and Monitoring Failures**
   - Log security events with traceability and alerting.
   - Protect log integrity and retention.

10. **A10: Server-Side Request Forgery (SSRF)**
    - Restrict outbound network access and use allowlisted destinations.
    - Validate and canonicalize URLs/IPs; block internal metadata endpoints.
