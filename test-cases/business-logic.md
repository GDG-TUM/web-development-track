[← Back to Finance Web Security home](../README.md)

# Financial business logic test cases

| ID | Test | Expected result | Priority | Result | Finding |
|---|---|---|---|---|---|
| BL-01 | Intercept a payment request in the lab proxy and change the amount | Server uses its own amount calculation; tampered value rejected or ignored | High | | |
| BL-02 | Modify a status field (for example, "paid" or "success") in a request or callback body | Status is set only after server-side verification of the simulated payment result | High | | |
| BL-03 | Send the same simulated payment request twice (replay or double click) | Handled safely: one transaction applied, no duplicate credit | High | | |
| BL-04 | Submit negative, zero, very large or non-numeric amounts | Rejected with a validation error | High | | |
| BL-05 | Attempt to set or change a balance from the browser | Balance is calculated on the server only; client-supplied balance ignored | High | | |
| BL-06 | Run two simultaneous requests against the same account (lab only, small volume) | Balance stays consistent | Medium | | |
| BL-07 | Review how the simulated payment confirmation is received | Confirmation is verified (for example, by signature or server-side lookup), not trusted from the browser | High | | |
| BL-08 | Check that statements and balances reconcile with the transaction history | Totals match | Medium | | |

> Keep volumes small. No load or denial-of-service testing.
