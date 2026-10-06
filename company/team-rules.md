---
owner: Hana Kim (proposed — founders to confirm)
last_verified: 2026-10-06
source: fernway-context-pack.md §5; CONTRIBUTING.md (how the repo applies the rules)
status: draft
---

# Team rules

1. **No decisions in DMs.** Anything affecting more than one person goes in a public Slack channel.
2. **Answer the same question twice and it gets written down.** In practice nobody does this. It is the rule the team breaks most often.
3. **Customer data stays in the systems it lives in:** HubSpot, Stripe, the production database. No exports into docs, spreadsheets or AI tools.
4. **Secrets live in 1Password.** Never in Slack, never in a document, never in a repo.
5. **No deploys on Friday.** This is the *Friday freeze*; see [processes/releases.md](../processes/releases.md).
6. **English is the working language**, including in country channels.

## How this repo applies rules 2, 3 and 4

### Rule 2: answer twice, write it down

- This repo is where "written down" goes.
- If you answer the same question twice in Slack, open a pull request that adds the answer to the right doc ([CONTRIBUTING.md](../CONTRIBUTING.md)).
- If @claude says **"not documented"**, that is a signal the answer belongs here. Ask the named owner, then open a PR.
- This is the rule most often broken. The repo only works if it is followed.

### Rule 3: customer data stays where it lives

- No customer personal data or contacts in any doc. That includes names, phone numbers and emails.
- No customer names, exports or screenshots of customer records, even as examples. Runbooks use made-up sample values.
- Docs say *where* data lives (HubSpot, Stripe, production database), never *what* it is.
- The same rule covers pasting into AI tools. Rules for the Claude support-drafts trial are still open; see [open-questions.md → Rules for pasting into Claude for support](../open-questions.md#rules-for-pasting-into-claude-for-support).

### Rule 4: secrets live in 1Password

- Docs name the 1Password item, never the value.
- A PR containing a secret must be rejected. The secret must be removed from branch history too, not just from the latest commit ([CONTRIBUTING.md](../CONTRIBUTING.md)).
- Known breach of this rule outside the repo: API keys pasted into n8n nodes. See [agents/n8n-workflows.md](../agents/n8n-workflows.md).
