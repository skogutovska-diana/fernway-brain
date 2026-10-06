---
owner: Hana Kim
last_verified: 2026-10-06
source: fernway-context-pack.md §4 (Billing), §1 (Pricing), §2 (external bookkeeping firm)
status: draft
---

# Billing

**Owner:** Hana Kim (Ops lead). Billing, invoices and vendor accounts.

## Flow

1. Billing runs in **Stripe**.
2. Customers are **invoiced monthly per venue** (not per account; see *account vs venue* in the [glossary](../glossary.md)).
3. Hana checks Stripe for failed payments **every Monday**.
4. Failed payments are **chased by hand**.

Prices and discounts: [company/pricing.md](../company/pricing.md).

## Hand-offs

| From | To | When |
|---|---|---|
| Sales (contract signed) | Hana Kim | Billing set-up for a new account: UNKNOWN — owner: Hana Kim |
| Hana Kim | Berlin bookkeeping firm (external) | What is handed over and when: UNKNOWN — owner: Hana Kim |

## Known problems

- **Failed payments are chased by hand** and depend on one person checking Stripe once a week.
- How a failed payment is chased (steps, timing, when to involve the account owner): UNKNOWN — owner: Hana Kim.
- Who covers the Monday check when Hana is unavailable: UNKNOWN — owner: Hana Kim.
