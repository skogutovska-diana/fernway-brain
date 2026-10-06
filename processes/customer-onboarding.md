---
owner: Lukas Weber
last_verified: 2026-10-06
source: fernway-context-pack.md §4 (New customer onboarding), §1 (positioning), §6 (T2L, pay rules, the importer, activation)
status: draft
---

# Customer onboarding

**Owner:** Lukas Weber (Customer Success), end to end.

**Why it matters:** onboarding speed is Fernway's whole positioning. The pitch is that a venue is live in under a day. The team measures this as **T2L** (time to live): contract signed → first schedule published.

## Flow

1. Contract signed in HubSpot.
2. Lukas books a 45-minute setup call.
3. Lukas imports the venue and staff list from the customer's CSV using **the importer**.
4. Lukas configures **pay rules** for the country.
5. The customer publishes their first schedule. **T2L stops here.**
6. 7-day check-in call.
7. Handover to support.

**Typical T2L today: 1–3 days.** The pitch is "under a day".

Step-by-step: [runbooks/01-onboard-a-new-customer.md](../runbooks/01-onboard-a-new-customer.md).

## Hand-offs

| From | To | When |
|---|---|---|
| Sales (contract signed in HubSpot) | Lukas Weber | Contract signed |
| Lukas Weber | Noor Haddad | The importer fails (see below) |
| Lukas Weber | Support: Jonas Berg | After the 7-day check-in call |

What exactly is handed over to support, and how: UNKNOWN — owner: Lukas Weber.

## Known problems

- **The importer fails** on names with non-Latin characters and on files exported from Apple Numbers.
  - Noor Haddad knows the workaround. It has never been written down, so Lukas messages him every time.
  - Workaround: UNKNOWN — owner: Noor Haddad.
  - This is a single point of knowledge; see [open-questions.md → Single points of knowledge](../open-questions.md#single-points-of-knowledge).
- **"Activation" means different things to different people.** Sales means first published schedule. Lukas means a full week scheduled. The Metabase dashboard measures something else. See [open-questions.md → Definition of activation](../open-questions.md#definition-of-activation).
