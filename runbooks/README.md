---
owner: Hana Kim (repo steward, proposed — founders to confirm)
last_verified: 2026-10-06
source: repo setup decisions (founders to confirm)
status: draft
---

# runbooks/

Numbered, step-by-step procedures someone can follow without asking anyone.

## What belongs here

- One procedure per file, named `NN-short-topic.md` (e.g. `01-...md`).
- Each runbook states: owner, when to use it, what you need before you start, numbered steps, and who to call if a step fails.
- Knowledge that only one person has today should become a runbook.

## What does not belong here

- Credentials. Give the 1Password item name, never the secret itself.
- Customer data, even as an example. Use made-up sample values.
- The overall flow of a process. That goes in `processes/`.
