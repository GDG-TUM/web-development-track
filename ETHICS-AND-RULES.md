[← Back to Finance Web Security home](README.md)

# ⚖️ Ethics and rules of engagement

Read this before you touch anything. It takes five minutes.

> [!IMPORTANT]
> **We attack only systems built for the purpose.** Our target is the team's own prototype, with fictional data. Never test the live TUM finance system, or any campus, personal or third-party system, without **explicit written permission**. Unauthorised access is illegal, including under Kenya's Computer Misuse and Cybercrimes Act.

## The four rules

1. Use **fictional student data** and **simulated payments**.
2. Test only the **team's own prototype** or **explicitly authorised training environments**.
3. Do **not** probe the live TUM finance system without explicit written permission.
4. **Never** commit secrets, use real payment credentials, or run disruptive tests against a live service.

## Do and don't

| ✅ Do | ❌ Don't |
|-------|---------|
| Test our own prototype in a lab or local build | Scan, probe or log in to the live TUM finance system |
| Use made-up students, balances and payments | Use real student records, real names or real payment details |
| Record permission and the testing window first | Start testing "just to see" |
| Keep request volumes small | Run load, flooding or denial-of-service tests |
| Redact tokens, cookies and personal data in evidence | Paste secrets or real data into issues, chats or screenshots |
| Report a finding with steps, impact and a fix | Share working exploits in public channels |
| Disclose unresolved issues honestly | Hide a finding because it is awkward before the demo |

## Authorisation record

Record written permission for every testing window **before** testing starts.

| Date | Target environment | Scope (features, roles) | Authorised by | Testing window |
|------|--------------------|-------------------------|---------------|----------------|
| *[TO CONFIRM]* | *e.g. local dev build or team staging URL* | | *Web lead / chairperson* | *start to end* |

## If something goes wrong

- **You reach something that is not our prototype** (a real system, real data): stop immediately, do not continue, and tell the Cybersecurity track lead.
- **You find real personal or financial data**: do not copy or share it. Tell a maintainer and delete any local copy.
- **You committed a secret**: tell a maintainer straight away so it can be rotated and removed from history. See the [security policy](https://github.com/GDG-TUM/.github/blob/main/SECURITY.md).

## Behaviour

We follow the [Code of Conduct](https://github.com/GDG-TUM/.github/blob/main/CODE_OF_CONDUCT.md). Review the code and the design, not the person.
