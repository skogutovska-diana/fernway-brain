---
owner: Hana Kim (repo steward, proposed — founders to confirm)
last_verified: 2026-10-06
source: fernway-context-pack.md §5; repo setup decisions (founders to confirm)
status: draft
---

# Contributing to the Fernway Brain

These rules apply to everyone: people and AI.

## Rules

1. **Every change goes through a pull request.** Nothing is pushed straight to `main`. AI may draft a PR but never merges.
2. **Every doc starts with front matter:** `owner`, `last_verified`, `source`, `status`. See the template below.
3. **If sources disagree, record both in `open-questions.md`** and name who decides. Do not pick one.
4. **English, plain Markdown, one topic per file.**
5. **Docs not verified for 90 days are treated as `needs-review`**, whatever their `status` field says.

## Never in the repo

- **Secrets or credentials.** Write where to find them in 1Password instead.
- **Customer personal data or contacts** (e.g. a client's phone number).
- **Compensation or other people data.**
- **Undecided commercial matters** (e.g. accounts on legacy pricing).
- **Anything not stated in a source.** Mark it unknown with an owner instead of guessing:
  `UNKNOWN — owner: <name>`

If something from this list lands in a PR, the reviewer must reject it. It has to be removed from the branch history too, not just from the latest commit.

## Front matter template

Put this at the top of every Markdown doc:

```yaml
---
owner: <person responsible for keeping this doc true>
last_verified: YYYY-MM-DD
source: <where the content came from: Slack thread, owner confirmation, etc.>
status: current | needs-review | draft
---
```

| Field | Meaning |
|---|---|
| `owner` | One named person who confirms the content is true. Normally the process owner. |
| `last_verified` | The date the owner last checked the whole doc against reality. |
| `source` | Where the information came from. Be specific enough that someone can trace it. |
| `status` | `current` = verified and in use. `needs-review` = may be out of date. `draft` = not yet confirmed by the owner. |

Exception: `.github/pull_request_template.md` has no front matter, because GitHub would copy it into every PR description. `.github/CODEOWNERS` is not a Markdown doc.

## How a change gets reviewed

1. **Branch.** Create a branch from `main` (e.g. `docs/onboarding-csv-workaround`).
2. **Edit.** Keep one topic per file. Update `last_verified` and `source` on every doc you touch.
3. **Open a PR.** Fill in the checklist in the PR template.
4. **Review.** `CODEOWNERS` requests a review from the owner of the folder. The reviewer checks the content is true and the checklist is honest.
5. **Merge.** A human with review rights merges. AI never merges.

If your change touches a disagreement, add it to `open-questions.md` in the same PR and tag the person who decides.

## How the brain stays current

- **90-day rule.** Any doc whose `last_verified` is older than 90 days counts as `needs-review`. Claude warns about these when it cites them.
- **Re-verifying.** When an owner checks a doc and it is still right, they open a small PR that only bumps `last_verified` (and sets `status: current`).
- **Steward sweep.** The repo steward (proposed: Hana Kim) regularly lists stale docs and asks their owners to verify or update them.
- **Answer twice, write it down.** If you answer the same question twice in Slack, it belongs here. Open a PR.
- **Decisions in Slack.** When a public Slack thread settles something, the doc owner updates the doc and links the thread in `source`.
- **Resolving open questions.** When the named decider decides, move the entry to *Resolved* in `open-questions.md` and update the affected docs in the same PR.
