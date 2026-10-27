[← Back to Finance Web Security home](../README.md)

# Access control test cases

| ID | Test | Expected result | Priority | Result | Finding |
|---|---|---|---|---|---|
| AC-01 | Log in as Student A and request Student B's statement or balance by changing the record identifier in the URL or request | Request is denied; no data from Student B returned | High | | |
| AC-02 | Log in as a student and call a finance-staff endpoint directly (for example, a balance adjustment) | Request is denied with an authorisation error | High | | |
| AC-03 | Access a finance-staff page by typing its URL while logged in as a student | Access denied; no staff data rendered | High | | |
| AC-04 | Access protected pages and API routes while logged out | Redirect to login or an authentication error | High | | |
| AC-05 | Modify a role or user-id field in a request body or token | Server ignores or rejects the change; role comes from the server session | High | | |
| AC-06 | List or search endpoints as a student | Only the student's own records are returned | Medium | | |
| AC-07 | Staff user attempts actions beyond their role (for example, admin-only functions) | Denied | Medium | | |
