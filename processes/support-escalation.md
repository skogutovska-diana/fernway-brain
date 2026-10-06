---
owner: Jonas Berg
last_verified: 2026-10-06
source: fernway-context-pack.md §4 (Support escalation), §2 (roles), §6 (ghost shift), §7 (Claude trial)
status: draft
---

# Support escalation

**Owner:** Jonas Berg (support agent, first line).

## Flow

1. A ticket arrives in Intercom.
2. Jonas handles it first.
3. Jonas escalates when needed:
   - **Technical issues** → Ana Silva.
   - **Production incidents** → Noor Haddad (on call for production incidents).
   - **Anything involving customer data** → Ivan Petrenko.

Decision steps: [runbooks/02-escalate-a-support-ticket.md](../runbooks/02-escalate-a-support-ticket.md).

## Hand-offs

| From | To | When |
|---|---|---|
| Lukas Weber (onboarding) | Jonas Berg | After the 7-day check-in call |
| Jonas Berg | Ana Silva | Technical issue |
| Jonas Berg | Noor Haddad | Production incident |
| Jonas Berg | Ivan Petrenko | Anything involving customer data |

How a hand-off is made (Intercom assignment, Slack, Linear ticket): UNKNOWN — owner: Jonas Berg.

## Known problems

- **Ghost shifts** (a published shift nobody claimed) are the single most common support complaint.
- **Ana is only half on support.** Ana splits 50/50 between QA and technical support. Backup when Ana is unavailable: UNKNOWN — owner: Jonas Berg.
- **Claude for draft replies is on trial with no rules** for what may be pasted into it. This conflicts with team rule 3. See [agents/claude-support-drafts.md](../agents/claude-support-drafts.md) and [open-questions.md → Rules for pasting into Claude for support](../open-questions.md#rules-for-pasting-into-claude-for-support).
