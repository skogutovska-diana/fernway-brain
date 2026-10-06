---
owner: Ivan Petrenko
last_verified: 2026-10-06
source: fernway-context-pack.md §3 (n8n, 1Password), §2 (Ivan Petrenko), §5 (rule 4)
status: draft
---

# n8n workflows

**Owner:** Ivan Petrenko
**Status:** in use, **undocumented**

## What it is

- Fernway's internal automations run in **Ivan's own n8n instance**.
- Ivan built all of them, alone.
- There are **six or seven workflows**. Nobody else can explain them.

## Register

| # | Workflow | What it does | What it touches | Credentials stored where | Status |
|---|---|---|---|---|---|
| 1 | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | Undocumented |
| 2 | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | Undocumented |
| 3 | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | Undocumented |
| 4 | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | Undocumented |
| 5 | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | Undocumented |
| 6 | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | Undocumented |
| 7 | UNKNOWN — owner: Ivan Petrenko (may not exist: the source says "six or seven") | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | UNKNOWN — owner: Ivan Petrenko | Undocumented |

## Risks

- **API keys are pasted directly into nodes** in a couple of workflows. This breaks team rule 4 (secrets live in 1Password). Anyone with access to the instance or an export of it can read the keys. Which workflows and which keys: UNKNOWN — owner: Ivan Petrenko.
- **One person knows it.** If Ivan is unavailable, nobody can explain, fix or switch off a workflow.
- **It runs in Ivan's own instance,** not a company-administered one. Who else has access and where it is hosted: UNKNOWN — owner: Ivan Petrenko.
- **Unknown blast radius.** Without an inventory, nobody knows which systems or customer data these workflows read or write.

## Fix

1. **Move every key out of the nodes and into 1Password.** Reference the 1Password item from n8n's credential store, not the raw value. Owner: Ivan Petrenko. Mechanism: UNKNOWN — owner: Ivan Petrenko.
2. **Rotate the keys that were pasted into nodes** *(proposed)*, since they have been readable in plain text. Owner: Ivan Petrenko.
3. **Inventory each workflow** in the register above: what it does, what it touches, where its credentials live, what breaks if it stops. Owner: Ivan Petrenko.

Never paste keys, credentials or workflow exports that contain them into this file. Name the 1Password item instead.
