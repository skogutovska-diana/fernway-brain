---
owner: Ivan Petrenko
last_verified: 2026-10-06
source: fernway-context-pack.md §4 (Releases), §5 (rule 5), §6 (Friday freeze), §7 (staging reset)
status: draft
---

# Releases

**Owner:** Ivan Petrenko (CTO).

## Flow

1. A Linear ticket.
2. A pull request.
3. Ana Silva tests it on staging.
4. Deploy on **Tuesdays and Thursdays**.

**Never on Fridays.** This is the **Friday freeze**, team rule 5; see [company/team-rules.md](../company/team-rules.md).

## Hand-offs

| From | To | When |
|---|---|---|
| Engineer | Ana Silva (QA) | PR ready for staging test |
| Ana Silva | Deployer: UNKNOWN — owner: Ivan Petrenko | Test passed |
| Production incident after deploy | Noor Haddad (on call) | See [support-escalation.md](support-escalation.md) |

Who reviews PRs, who deploys, and how to roll back: UNKNOWN — owner: Ivan Petrenko.

## Known problems

- **Only Ana knows how the staging environment is reset.** When Ana is unavailable, nobody else can do it. See [open-questions.md → Single points of knowledge](../open-questions.md#single-points-of-knowledge).
- **Staging testing depends on Ana**, who is also half on technical support. Backup tester: UNKNOWN — owner: Ivan Petrenko.
