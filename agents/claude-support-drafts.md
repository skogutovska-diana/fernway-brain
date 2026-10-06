---
owner: UNKNOWN — proposed: Jonas Berg (support process owner)
last_verified: 2026-10-06
source: fernway-context-pack.md §7 (Claude trial), §5 (rules 3 and 4), §4 (Support escalation)
status: draft
---

# Claude for support draft replies

**Owner:** UNKNOWN — proposed: Jonas Berg (support process owner)
**Status:** trial. **No rules exist yet** for what may be pasted into it.

## What it does

The team is trying out Claude to draft replies to support tickets.

Who uses it, how often, and how drafts get back into Intercom: UNKNOWN — owner: Jonas Berg (proposed).

## What it touches

- **Intercom ticket text**, pasted into Claude.
- Ticket text can contain customer personal data. That data is meant to stay in its own system.
- Which Claude account or plan is used and its data settings: UNKNOWN — owner: Hana Kim (tooling admin).

## Risks

- **Conflict with team rule 3:** "Customer data stays in the systems it lives in … No exports into docs, spreadsheets, or AI tools." Pasting raw ticket text into Claude can break this rule.
- **No rules yet.** Each person decides on their own what to paste.
- Possible secrets in tickets (rule 4) if a customer or agent pastes credentials into a conversation.

## Interim rules — **PROPOSED, DECISION NEEDED**

> These are not agreed rules. They are a proposal until the decider in [open-questions.md → Rules for pasting into Claude for support](../open-questions.md#rules-for-pasting-into-claude-for-support) decides.

1. **No secrets.** Never paste passwords, API keys or login details (rule 4).
2. **Strip customer personal data before pasting.** Remove names, emails, phone numbers and anything that identifies a person or customer. Describe the problem instead.
3. **Nothing from Stripe or the production database.** No payment or account data (rule 3).
4. **A human reviews every draft before it is sent.** Claude never replies to a customer directly.
5. **Tickets involving customer data are escalated, not drafted.** They go to Ivan Petrenko per [runbooks/02-escalate-a-support-ticket.md](../runbooks/02-escalate-a-support-ticket.md).

Status of these rules: **proposed, decision needed.**
