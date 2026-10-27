[← Back to Finance Web Security home](../README.md)

# Test cases

Starting points for the Cybersecurity track. They are written to be **tied to the actual finance-portal features** once the Web lead confirms them (Weeks 5–6) and **prioritised in Weeks 8–9**. Adapt, delete or add cases to match what was really built.

Run them only against the team's own prototype or an authorised training lab, with fictional data. See [Rules and boundaries](../ETHICS-AND-RULES.md).

| File | Area | OWASP link |
|---|---|---|
| [access-control.md](access-control.md) | Students see only their own records; role restrictions | Broken access control |
| [authentication-sessions.md](authentication-sessions.md) | Login, sessions, logout, password reset | Authentication failures |
| [input-output.md](input-output.md) | Server-side validation, injection, output encoding | Injection |
| [business-logic.md](business-logic.md) | Server-side balances, payment verification, duplicates | Insecure design |
| [secrets-dependencies-config.md](secrets-dependencies-config.md) | Secrets, dependencies, configuration, deployment | Security misconfiguration |
| [audit-logs.md](audit-logs.md) | Audit trail for financial changes | Logging failures |

## Result codes
Pass · Fail (raise a finding) · N/A (feature not built) · Blocked
