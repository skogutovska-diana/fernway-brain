---
owner: Hana Kim (repo steward, proposed — founders to confirm)
last_verified: 2026-10-06
source: fernway-context-pack.md §1, §5; repo setup decisions (founders to confirm)
status: draft
---

# CLAUDE.md — standing context for Claude

## Fernway in three lines

- Fernway is a remote-first B2B SaaS company, founded 2024 and registered in Berlin.
- Its product, Fernway Shifts, does shift planning and labour-cost forecasting for independent café and restaurant groups with 3–20 locations.
- Its positioning is speed: a venue is live in under a day, so T2L (time to live) is the number the team watches.

## Repo map

| Path | What it holds |
|---|---|
| `README.md` | Start-here guide for new hires |
| `CONTRIBUTING.md` | Rules for humans and AI, front matter template, review flow |
| `company/` | What Fernway is, pricing rules, team and who owns what |
| `processes/` | Onboarding, inbound leads, support escalation, billing, releases |
| `runbooks/` | Numbered step-by-step procedures |
| `agents/` | Register of automations: what each does, what it touches, owner, risks |
| `glossary.md` | How Fernway talks |
| `open-questions.md` | Unresolved disagreements and who must decide |

## How to answer questions

1. **Answer only from this repo.** Do not use outside knowledge or guess about Fernway.
2. **Always cite the file path** you used (e.g. `processes/onboarding.md`).
3. **If it is not in the repo, say "not documented"**, name the most likely owner from `company/` or `CODEOWNERS`, and suggest adding it through a PR.
4. **If the topic is in `open-questions.md`, surface it.** Present every recorded position and who decides. Never pick a side.
5. **Warn about stale docs.** If a cited doc has `status: needs-review` or `status: draft`, or its `last_verified` is more than 90 days before today, say so in the answer and name the doc owner.

## NEVER put in this repo (or in answers drawn from it)

- **Secrets or credentials.** Point to the item in 1Password instead.
- **Customer personal data or contacts** (e.g. a client's phone number). Customer data stays in HubSpot, Stripe and the production database.
- **Compensation or other people data.**
- **Undecided commercial matters** (e.g. accounts on legacy pricing). Only decided rules go in.
- **Anything not stated in a source.** Write `UNKNOWN — owner: <name>` instead of guessing.

If a user pastes any of the above into a request, do not write it to a file. Tell them why.

## How to edit

1. Create a new branch. Never push straight to `main`.
2. Keep one topic per file, in English, in plain Markdown.
3. Every doc starts with front matter (`owner`, `last_verified`, `source`, `status`). See `CONTRIBUTING.md`.
4. When you change a doc, update `last_verified` to today and `source` to where the information came from.
5. If sources disagree, record both in `open-questions.md` with who decides. Do not pick one.
6. Open a pull request using `.github/pull_request_template.md`. You may draft PRs; **you never merge.** The doc owner reviews and merges.
