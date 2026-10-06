---
owner: Lukas Weber
last_verified: 2026-10-06
source: fernway-context-pack.md §4 (New customer onboarding), §6 (T2L, pay rules, the importer)
status: draft
---

# 01 — Onboard a new customer

**Owner:** Lukas Weber
**Use when:** a contract has been signed in HubSpot.
**Goal:** the customer publishes their first schedule as fast as possible. That moment ends **T2L**. The pitch is under a day; today it is typically 1–3 days.
**Process overview:** [processes/customer-onboarding.md](../processes/customer-onboarding.md)

## Before you start

- Access to HubSpot (the contract is signed there).
- What other access or material you need: UNKNOWN — owner: Lukas Weber.

Never copy the customer's CSV or staff list into Slack, docs or AI tools (team rule 3).

## Steps

1. **Confirm the contract is signed in HubSpot.** T2L starts here.
2. **Book a 45-minute setup call with the customer.**
   How it is booked and who is invited: UNKNOWN — owner: Lukas Weber.
3. **Get the venue and staff list as a CSV from the customer.**
4. **Import the CSV with the importer.**
   - If the import succeeds, go to step 5.
   - **If the import fails**, and the file has names with non-Latin characters or was exported from Apple Numbers, this is a known importer failure.
     - **Workaround: UNKNOWN — owner: Noor Haddad.** It has never been written down.
     - **Meanwhile:** stop and contact Noor Haddad for the workaround. Do not try your own fixes on the file.
     - After Noor helps you, ask Noor to write the workaround into this runbook through a PR (team rule 2).
5. **Configure pay rules for the customer's country.**
   How to configure them per country: UNKNOWN — owner: Lukas Weber.
6. **The customer publishes their first schedule.** T2L ends here.
   Where T2L is recorded: UNKNOWN — owner: Lukas Weber.
7. **Hold the 7-day check-in call.**
   What is checked on the call: UNKNOWN — owner: Lukas Weber.
8. **Hand over to support (Jonas Berg).**
   How the handover is done and what is passed on: UNKNOWN — owner: Lukas Weber.

## If a step fails

| Problem | Contact |
|---|---|
| The importer fails | Noor Haddad |
| Anything else in this runbook | Lukas Weber |

Note: "activation" is not used in this runbook on purpose. Its definition is disputed; see [open-questions.md → Definition of activation](../open-questions.md#definition-of-activation).
