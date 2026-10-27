[← Back to Finance Web Security home](../README.md)

# Threat list

Prepared in Weeks 5–6 with the Web lead.

| ID | Asset | Threat | Who could cause it | Likelihood | Impact | Planned control | Related requirement |
|---|---|---|---|---|---|---|---|
| T-01 | Student fee balance | A student views another student's records | Authenticated student | | | Server-side ownership checks | Access control |
| T-02 | Payment status | Browser-supplied status or amount is trusted | Any user | | | Server-side verification | Financial business logic |
| T-03 | Staff adjustments | Unauthorised financial adjustment | Student or low-privilege staff | | | Role-based access control, audit trail | Access control, Audit logs |
| T-04 | Accounts and sessions | Weak login, session or password-reset flow | Any user | | | Established hashing library, secure session settings | Authentication and sessions |

> The rows above are starting prompts drawn from the project's protection goals. Edit them to match the features actually built, and add rows as the design evolves.
