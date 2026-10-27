[← Back to Finance Web Security home](../README.md)

# Audit log test cases

| ID | Test | Expected result | Priority | Result | Finding |
|---|---|---|---|---|---|
| AL-01 | Make a financial adjustment as a staff user | Audit entry records who acted, what changed and when | High | | |
| AL-02 | Review the log content after login and password-reset attempts | Passwords, tokens and session identifiers are not written to logs | High | | |
| AL-03 | Check whether a user can edit or delete audit entries | No; entries are append-only for ordinary roles | Medium | | |
| AL-04 | Make a failed or denied privileged action | Attempt is recorded where appropriate | Medium | | |
| AL-05 | Compare the audit trail with a series of known test actions | Every important change appears, in order | Medium | | |
