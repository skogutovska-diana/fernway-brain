---
owner: Hana Kim (repo steward, proposed — founders to confirm)
last_verified: 2026-10-06
source: fernway-context-pack.md §3; repo setup decisions (founders to confirm)
status: draft
---

# agents/

The register of Fernway's automations and AI agents. Proposed owner of the register: Ivan Petrenko.

## What belongs here

One file per automation, covering:

- **What it does:** trigger, steps, output.
- **What it touches:** every system it reads from or writes to.
- **Owner:** who maintains it and who to call when it breaks.
- **Risks:** what happens if it fails, what data it can see, where its credentials are stored.

Anything that is not known yet is written as `UNKNOWN — owner: <name>`.

## What does not belong here

- API keys, tokens or exported workflow configs that contain them. Reference the 1Password item instead.
- Customer data seen in workflow runs.
