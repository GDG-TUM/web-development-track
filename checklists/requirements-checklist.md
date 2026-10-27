[← Back to Finance Web Security home](../README.md)

# Security requirements checklist

Tick when the requirement is implemented **and** verified in the prototype.

## Access control
- [ ] A student can only access their own records
- [ ] Finance functions are restricted to authorised roles

## Authentication and sessions (where accounts exist)
- [ ] Established password-hashing library in use
- [ ] Secure session settings
- [ ] Safe logout
- [ ] Appropriate password-reset controls

## Input and output handling
- [ ] Inputs validated on the server
- [ ] Parameterised database queries
- [ ] User-controlled content safely encoded before display

## Financial business logic
- [ ] Balances calculated on the server
- [ ] Transaction status verified server-side
- [ ] Duplicate requests handled safely
- [ ] Amounts and statuses sent by the browser are not trusted

## Secrets and configuration
- [ ] No passwords, API keys or tokens in source code or Git history
- [ ] Suitable secret storage
- [ ] Non-debug settings

## Dependencies
- [ ] Third-party libraries tracked
- [ ] Known-vulnerable dependencies reviewed and updated

## Audit logs
- [ ] Important financial changes record user, timestamp and action
- [ ] Passwords and tokens are never logged

## Deployment and recovery (if deployed)
- [ ] HTTPS
- [ ] Permissions
- [ ] Security headers
- [ ] Backups
- [ ] Error handling
