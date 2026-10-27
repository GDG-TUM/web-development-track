[← Back to Finance Web Security home](../README.md)

# Input and output handling test cases

| ID | Test | Expected result | Priority | Result | Finding |
|---|---|---|---|---|---|
| IO-01 | Submit unexpected types, lengths and characters in every form field and API parameter | Server-side validation rejects invalid input with a safe error | High | | |
| IO-02 | Review database access code for string-built queries | Parameterised queries or a safe ORM are used everywhere | High | | |
| IO-03 | In the test lab, try standard injection test strings in search and filter fields | No database errors, altered results or unexpected behaviour | High | | |
| IO-04 | Enter markup or script test strings in any user-controlled field that is later displayed (names, notes, references) | Content is encoded on output and displayed as text, not executed | High | | |
| IO-05 | Remove or bypass client-side validation (for example, with Developer Tools or a proxy) and resubmit | Server still enforces the same rules | High | | |
| IO-06 | Trigger errors with malformed requests | Error pages do not expose stack traces, queries or paths | Medium | | |
| IO-07 | Upload a file, if uploads exist | Type, size and content are validated; files are not served as executable content | Medium | | |
