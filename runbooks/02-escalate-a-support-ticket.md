---
owner: Jonas Berg
last_verified: 2026-10-06
source: fernway-context-pack.md §4 (Support escalation), §2 (roles), §5 (rule 3)
status: draft
---

# 02 — Escalate a support ticket

**Owner:** Jonas Berg
**Use when:** a ticket arrives in Intercom.
**Process overview:** [processes/support-escalation.md](../processes/support-escalation.md)

The pack gives the escalation targets (technical → Ana, production incident → Noor, customer data → Ivan). It does not give an order for checking them. The order below checks customer data first because that has the strictest owner. **This order is proposed and must be confirmed by Jonas Berg.**

## Steps

1. **Read the ticket in Intercom.** Jonas is first line for every ticket.
2. **Does it involve customer data?** → Escalate to **Ivan Petrenko**. Stop here.
   Do not copy the data out of Intercom into Slack, docs or AI tools (team rule 3).
3. **Is it a production incident?** → Escalate to **Noor Haddad** (on call for production incidents). Stop here.
   What counts as a production incident: UNKNOWN — owner: Noor Haddad.
4. **Is it a technical issue?** → Escalate to **Ana Silva** (technical support). Stop here.
5. **Otherwise** → Jonas handles it in Intercom.

## Open points

- How to escalate (Intercom assignment, Slack channel, Linear ticket): UNKNOWN — owner: Jonas Berg.
- A ticket that fits more than one category: UNKNOWN — owner: Jonas Berg.
- Who to escalate to when Ana, Noor or Ivan is unavailable: UNKNOWN — owner: Jonas Berg.
- Expected response times: UNKNOWN — owner: Jonas Berg.
- Using Claude to draft the reply: rules are not decided. See [agents/claude-support-drafts.md](../agents/claude-support-drafts.md).
