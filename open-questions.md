---
owner: Hana Kim (repo steward, proposed — founders to confirm)
last_verified: 2026-10-06
source: fernway-context-pack.md §2, §3, §4, §6, §7
status: draft
---

# Open questions

Topics the team has not settled. **No answer below is the rule** until the decider decides. Claude and docs present every position and do not pick a side.

When a question is decided, move it to *Resolved* and update the affected docs in the same PR ([CONTRIBUTING.md](CONTRIBUTING.md)).

## Entry format

- **Question:** what needs deciding.
- **Positions:** each position and who holds it.
- **Impact:** what goes wrong while it is open.
- **Who decides:** the named decider, or "proposed decider" if the source names nobody.
- **Status:** open / resolved.

## Open

### Lead qualification time

- **Question:** must inbound leads be qualified within 24 hours or 48 hours?
- **Positions:**
  - **24 hours.** Held by Sofia Marchetti (Head of Sales), who tells the team this is the rule.
  - **48 hours in busy weeks.** What Priya Raman (SDR) works to in practice, and the team has quietly accepted it.
- **Impact:** nobody knows which SLA to measure or hold people to. New SDRs get two different answers.
- **Who decides:** not stated in source. **Proposed decider: Mara Voss** (CEO), since Sofia holds one of the positions.
- **Status:** open
- **Affects:** [processes/inbound-leads.md](processes/inbound-leads.md)

### Definition of activation

- **Question:** what does "activation" mean?
- **Positions:**
  - **First published schedule.** Sales.
  - **A full week scheduled.** Lukas Weber (Customer Success).
  - **Something else.** What the Metabase dashboard measures. Exactly what: UNKNOWN — owner: Ivan Petrenko (proposed).
- **Impact:** the same word gives different numbers in sales, onboarding and dashboards. Reports can't be compared.
- **Who decides:** not stated in source. **Proposed decider: Mara Voss** (CEO), since the term spans sales, customer success and data.
- **Status:** open
- **Affects:** [glossary.md](glossary.md), [processes/customer-onboarding.md](processes/customer-onboarding.md)

### Rules for pasting into Claude for support

- **Question:** what may support paste into Claude when drafting replies?
- **Positions:**
  - **No rules yet.** The current trial: people decide for themselves.
  - **Team rule 3:** customer data stays in its systems, with no exports into AI tools. Followed literally, this limits pasting raw ticket text.
  - **Interim rules proposed** in [agents/claude-support-drafts.md](agents/claude-support-drafts.md). This is a proposal for the decider, not an agreed position.
- **Impact:** customer data may leave Intercom without anyone deciding that is acceptable.
- **Who decides:** not stated in source. **Proposed decider: Ivan Petrenko** (CTO; anything involving customer data escalates to him).
- **Status:** open
- **Affects:** [agents/claude-support-drafts.md](agents/claude-support-drafts.md), [processes/support-escalation.md](processes/support-escalation.md)

### Who owns documentation

- **Question:** who owns documentation, including this repo?
- **Positions:**
  - **Nobody owns it today.** When a new person joins, whoever has time that week walks them through things. *(Source: context pack §2.)*
  - **Hana Kim as repo steward.** Proposed in [CONTRIBUTING.md](CONTRIBUTING.md), not yet confirmed by the founders.
- **Impact:** docs go stale (Notion is "where documents go to die"). Rule 2, "answer twice, write it down", has nobody enforcing it.
- **Who decides:** not stated in source. **Proposed deciders: Mara Voss and Ivan Petrenko** (founders).
- **Status:** open
- **Affects:** [company/team-and-owners.md](company/team-and-owners.md), [CONTRIBUTING.md](CONTRIBUTING.md)

### New-hire account access

- **Question:** does a new hire get all tool accounts on day one, or later?
- **Positions:**
  - **Day one.** The Notion onboarding checklist. Who wrote it: UNKNOWN — owner: Hana Kim.
  - **Week two.** What happens in practice for most people.
- **Impact:** new hires can't work in their first week, and the written checklist is not true.
- **Who decides:** not stated in source. **Proposed decider: Mara Voss** (runs hiring), with Hana Kim (tooling admin).
- **Status:** open
- **Affects:** [company/tools.md](company/tools.md), [company/team-and-owners.md](company/team-and-owners.md)

### Single points of knowledge

- **Question:** how should knowledge that only one person has be written down and shared, and who makes sure it happens?
- **Known cases:**
  - **Staging environment reset.** Only Ana Silva knows how.
  - **CSV importer workaround** (non-Latin names, Apple Numbers exports). Only Noor Haddad knows. Lukas messages Noor every time.
  - Related: the **n8n workflows**, which only Ivan Petrenko can explain ([agents/n8n-workflows.md](agents/n8n-workflows.md)).
- **Positions:** no positions recorded in the source. The open points are priority, deadline and who writes each runbook.
- **Impact:** releases stall when Ana is unavailable. Onboarding stalls when Noor is unavailable, which hurts T2L.
- **Who decides:** not stated in source. **Proposed decider: Ivan Petrenko** (CTO; all cases are in engineering).
- **Status:** open
- **Affects:** [processes/releases.md](processes/releases.md), [runbooks/01-onboard-a-new-customer.md](runbooks/01-onboard-a-new-customer.md)

## Resolved

None yet.
