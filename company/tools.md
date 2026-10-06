---
owner: Hana Kim
last_verified: 2026-10-06
source: fernway-context-pack.md §3; §2 (Hana Kim: tooling admin; Ivan Petrenko: n8n); §4 (Billing: Stripe); §7 (Claude trial)
status: draft
---

# Tools

Credentials are **never** written here or anywhere in this repo. If a tool has a shared login, it is in 1Password.

Hana Kim is the tooling admin (pack §2). The pack does not say who administers each tool individually. Where that is unconfirmed, it is marked.

| Tool | What it's for | Administered by | Notes |
|---|---|---|---|
| Slack | Main channel for everything | Hana Kim (tooling admin) — per-tool admin UNKNOWN — owner: Hana Kim | Most decisions happen in threads and are never recorded anywhere else. Team rule 1: no decisions in DMs. |
| Notion | Older internal docs (around 60 pages) | Hana Kim (tooling admin) — per-tool admin UNKNOWN — owner: Hana Kim | Most pages were written in the first six months and never touched again. Treat as possibly out of date. |
| HubSpot | CRM and sales pipeline | Hana Kim (tooling admin) — per-tool admin UNKNOWN — owner: Hana Kim | Customer data lives here and stays here (team rule 3). |
| Linear | Engineering tickets | Hana Kim (tooling admin) — per-tool admin UNKNOWN — owner: Ivan Petrenko | Start of the release flow. |
| Intercom | Customer support inbox | Hana Kim (tooling admin) — per-tool admin UNKNOWN — owner: Hana Kim | Start of support escalation. Ticket text is used in the Claude drafts trial; see [agents/claude-support-drafts.md](../agents/claude-support-drafts.md). |
| Stripe | Billing and invoices | Hana Kim | Customer data lives here and stays here (team rule 3). |
| Google Workspace | Docs, shared drive, calendars | Hana Kim (tooling admin) — per-tool admin UNKNOWN — owner: Hana Kim | |
| Metabase | Dashboards over the production database | Hana Kim (tooling admin) — per-tool admin UNKNOWN — owner: Ivan Petrenko | The team shares **one read-only login**. Credentials are in 1Password. |
| n8n | Internal automations | Ivan Petrenko (his own instance) | Six or seven workflows nobody else can explain; some have API keys pasted into nodes. See [agents/n8n-workflows.md](../agents/n8n-workflows.md). |
| 1Password | Where secrets live | Hana Kim (tooling admin) — per-tool admin UNKNOWN — owner: Hana Kim | Team rule 4: secrets live here, never in Slack, documents or repos. |
| Claude | Trial: drafting support replies | UNKNOWN — owner: Jonas Berg (proposed) | No rules yet for what may be pasted in. See [agents/claude-support-drafts.md](../agents/claude-support-drafts.md). |

## Getting access

When a new hire gets accounts is disputed: day one according to the Notion checklist, week two in practice. See [open-questions.md → New-hire account access](../open-questions.md#new-hire-account-access).

How to request access to a tool: UNKNOWN — owner: Hana Kim.
