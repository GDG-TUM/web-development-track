[← Back to Finance Web Security home](../README.md)

# Secrets, dependencies and configuration test cases

| ID | Test | Expected result | Priority | Result | Finding |
|---|---|---|---|---|---|
| SC-01 | Search the repository and Git history for passwords, API keys, tokens and `.env` files | None found | High | | |
| SC-02 | Confirm `.gitignore` covers environment and secret files | Covered | High | | |
| SC-03 | Review where secrets live at runtime | Held in environment variables or a suitable secret store | High | | |
| SC-04 | Run a dependency audit (for example, `npm audit` or the stack's equivalent) | Known-vulnerable packages reviewed; plan to update recorded | Medium | | |
| SC-05 | Check configuration for debug mode or verbose errors | Debug disabled outside local development | High | | |
| SC-06 | If deployed: check HTTPS, redirect from HTTP, and security headers | HTTPS enforced; sensible headers set | Medium | | |
| SC-07 | If deployed: check file and directory permissions, and error handling | Least privilege; no sensitive error output | Medium | | |
| SC-08 | If deployed: confirm backup and recovery steps exist | Documented and, where feasible, tried on fictional data | Low | | |
