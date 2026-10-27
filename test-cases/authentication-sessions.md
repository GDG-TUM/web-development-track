[← Back to Finance Web Security home](../README.md)

# Authentication and session test cases

| ID | Test | Expected result | Priority | Result | Finding |
|---|---|---|---|---|---|
| AU-01 | Inspect how passwords are stored in the test database (fictional accounts) | Passwords are hashed with an established library, never plain text | High | | |
| AU-02 | Inspect session cookie attributes in browser Developer Tools | `HttpOnly`, `Secure` (when on HTTPS) and a suitable `SameSite` value are set | High | | |
| AU-03 | Log out, then press Back or replay a previous authenticated request | Session is invalidated server-side; access is denied | High | | |
| AU-04 | Repeated failed logins on a test account | Rate limiting or lockout behaviour is applied | Medium | | |
| AU-05 | Review login error messages | Messages do not reveal whether the username exists | Medium | | |
| AU-06 | Walk through the password-reset flow (if in scope) | Reset tokens are single-use, expire, and are not guessable; the process does not leak whether an account exists | High | | |
| AU-07 | Check whether the session identifier changes after login | A new session identifier is issued on login | Medium | | |
| AU-08 | Check session expiry after inactivity | Session expires after a reasonable idle time | Low | | |
| AU-09 | Review privileged (staff/admin) accounts | Stronger controls applied where in scope; no default or shared credentials | High | | |
