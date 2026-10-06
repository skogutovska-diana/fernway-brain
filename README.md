---
owner: Hana Kim (repo steward, proposed — founders to confirm)
last_verified: 2026-10-06
source: fernway-context-pack.md §1, §2, §3, §4, §7; repo setup decisions (founders to confirm)
status: draft
---

# Fernway Brain — start here

This repo is Fernway's shared memory: how the company works, written down in one place.

Fernway builds **Fernway Shifts**, a shift-planning and labour-cost forecasting tool for independent café and restaurant groups. We sell on speed: a venue goes live in under a day.

## What to read first

1. **This file.** It is the map.
2. **[`glossary.md`](glossary.md).** How we talk. Learn *account vs venue* before anything else.
3. **[`company/`](company/).** What Fernway is ([overview](company/overview.md)), how [pricing](company/pricing.md) works, [who owns what](company/team-and-owners.md), our [tools](company/tools.md) and [team rules](company/team-rules.md).
4. **[`processes/`](processes/).** Read the process for your role, then skim the others.
5. **[`open-questions.md`](open-questions.md).** Topics the team has not settled yet. Don't treat any one answer as the rule.

## Where to find what

| You want to know… | Look in | Owned by (proposed) |
|---|---|---|
| What Fernway is | [`company/overview.md`](company/overview.md) | Hana Kim |
| Team, who owns what, who to ask | [`company/team-and-owners.md`](company/team-and-owners.md) | Hana Kim |
| Which tools we use and who administers them | [`company/tools.md`](company/tools.md) | Hana Kim |
| Team rules | [`company/team-rules.md`](company/team-rules.md) | Hana Kim |
| Pricing rules | [`company/pricing.md`](company/pricing.md) | Mara Voss |
| How customer onboarding works | [`processes/customer-onboarding.md`](processes/customer-onboarding.md) | Lukas Weber |
| How inbound leads are handled | [`processes/inbound-leads.md`](processes/inbound-leads.md) | Priya Raman |
| How support escalates | [`processes/support-escalation.md`](processes/support-escalation.md) | Jonas Berg |
| How billing works | [`processes/billing.md`](processes/billing.md) | Hana Kim |
| How releases work | [`processes/releases.md`](processes/releases.md) | Ivan Petrenko |
| Onboard a new customer, step by step | [`runbooks/01-onboard-a-new-customer.md`](runbooks/01-onboard-a-new-customer.md) | Lukas Weber |
| Escalate a support ticket, step by step | [`runbooks/02-escalate-a-support-ticket.md`](runbooks/02-escalate-a-support-ticket.md) | Jonas Berg |
| What the n8n automations do | [`agents/n8n-workflows.md`](agents/n8n-workflows.md) | Ivan Petrenko |
| Claude for support draft replies (trial) | [`agents/claude-support-drafts.md`](agents/claude-support-drafts.md) | UNKNOWN — proposed: Jonas Berg |
| What a word means | [`glossary.md`](glossary.md) | Hana Kim |
| What is still undecided | [`open-questions.md`](open-questions.md) | Hana Kim |

Every doc says at the top who owns it, when it was last checked (`last_verified`) and whether it is `current`. Docs not checked in the last 90 days count as needing review. Check with the owner before you rely on one.

## Asking @claude

You can ask Claude about anything in this repo in plain English, e.g. *"@claude how do we hand a new customer over to support?"*

- Claude answers **only from this repo** and gives the file path it used.
- If it says **"not documented"**, ask the owner it names. Then write the answer down through a pull request. Our rule: if the same question gets answered twice, it gets written down.
- If it points you to `open-questions.md`, the team has not decided yet. Claude won't pick a side, and you shouldn't either.
- If it warns that a doc **needs review**, confirm with the doc owner before acting on it.

**Never paste these into Claude or into this repo:** passwords or API keys (they live in 1Password), customer personal data or contacts, or salary/people data.

## Want to change something?

Read `CONTRIBUTING.md`. Every change goes through a pull request.
