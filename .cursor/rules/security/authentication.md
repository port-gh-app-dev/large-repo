# Authentication Rules

- Require authentication for every non-public endpoint by default.
- Use centralized middleware/guards rather than per-handler checks.
- Never store plaintext passwords; hash with Argon2id (preferred) or bcrypt with a strong cost factor.
- Enforce MFA for privileged/admin access.
- Use short-lived access tokens and rotate refresh tokens on use.
- Validate token issuer, audience, signature, expiration, and not-before claims.
- Revoke sessions/tokens on password reset, account compromise, or role downgrade.
- Implement account lockout or progressive delays for repeated failed login attempts.
- Avoid user enumeration in auth errors (return generic credential failure messages).
- Require re-authentication for high-risk actions (email/password changes, payout actions).
