[← Back to Finance Web Security home](../README.md)

# 3. Security requirements

- **Access control:** A student can only access their own records; finance functions are restricted to authorised roles.
- **Authentication and sessions:** Where accounts exist, use established password-hashing libraries, secure session settings, safe logout and appropriate password-reset controls.
- **Input and output handling:** Validate inputs on the server, use parameterised database queries, and safely encode user-controlled content before displaying it.
- **Financial business logic:** Calculate balances on the server; verify transaction status server-side; handle duplicate requests safely; do not trust amounts or statuses sent by the browser.
- **Secrets and configuration:** Keep passwords, API keys and tokens out of source code and Git history. Use suitable secret storage and non-debug settings.
- **Dependencies:** Track third-party libraries and review/update known-vulnerable dependencies.
- **Audit logs:** Record important financial changes with user, timestamp and action, without logging passwords or tokens.
- **Deployment and recovery:** If deployed, check HTTPS, permissions, security headers, backups and error handling where relevant.

A trackable version is in [checklists/requirements-checklist.md](../checklists/requirements-checklist.md).
