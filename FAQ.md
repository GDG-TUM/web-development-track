[← Back to Finance Web Security home](README.md)

# ❓ FAQ

### Do I need security experience to join?
No. Start with [Learning priorities](plan/04-learning-priorities.md) and the free labs in [Starter resources](plan/05-starter-resources.md). Mixed skill levels are normal.

### Can I test the real TUM finance portal?
**No.** Not without explicit written authorisation. This project builds and tests our **own prototype** with fictional data. See the [rules](ETHICS-AND-RULES.md).

### What data do we use?
Fictional student records and simulated transactions only. No real student data and no real payment credentials.

### Which tools do I need?
Browser Developer Tools are enough to start. OWASP ZAP and Burp Suite Community are used in an authorised lab from Week 10. See [Getting started](GETTING-STARTED.md).

### Who builds the app and who secures it?
The **Web track** owns the application structure and features. The **Cybersecurity track** defines security requirements, assesses risks, coordinates authorised testing, and documents fixes and limitations. Both meet weekly.

### How do I report a finding?
Open a *Security finding* issue and fill in the [finding report](templates/finding-report.md): reproduction steps, affected feature, impact, evidence, severity, recommended fix, owner and retest status. Then add a row to the [vulnerability register](templates/vulnerability-register.md).

### Who fixes a finding?
The developer who owns the affected feature, with the Cybersecurity track's help. The Cybersecurity track then **retests** and updates the [retest log](templates/retest-log.md).

### What if I find a vulnerability in a real system by accident?
Stop, do not go further, do not copy any data, and tell the Cybersecurity track lead.

### What if I commit a secret?
Tell a maintainer immediately so it can be rotated and removed from history. See the [security policy](https://github.com/GDG-TUM/.github/blob/main/SECURITY.md).

### How are severities decided?
Using the scale in the [vulnerability register](templates/vulnerability-register.md): Critical, High, Medium, Low, Info. The exact criteria are an [open item](OPEN-ITEMS.md).

### What happens at Week 13?
We demonstrate the prototype, safely show a finding and its fix, and explain remaining limitations. See [Before the showcase](checklists/pre-showcase.md).

### I missed a check-in. What now?
Read the [roadmap](roadmap/week-by-week.md) for that week, check open issues, and ask in the project channel.
