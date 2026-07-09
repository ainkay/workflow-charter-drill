# Branching Strategy

## Branch Naming Convention

| Prefix | Purpose | Example |
|---------|----------|---------|
| feature/ | New features | feature/user-login |
| bugfix/ | Bug fixes | bugfix/navbar-crash |
| hotfix/ | Emergency production fixes | hotfix/payment-error |
| release/ | Release preparation | release/v1.3.0 |
| chore/ | Maintenance work | chore/update-eslint |

---

# Protected Branches

## main

Protection:

- No direct pushes
- Pull Requests required
- At least 2 approvals
- Passing CI required
- Branch must be up to date before merge

Reason:

Keeps production stable.

---

## develop (if used)

Protection:

- PR required
- Passing CI

Reason:

Ensures integration branch remains stable.

---

# Branch Lifecycle

1. Create branch from main.
2. Implement changes.
3. Sync regularly with main.
4. Open Pull Request.
5. Complete reviews.
6. Pass all CI checks.
7. Merge.
8. Delete branch.

Maximum feature branch lifetime:

**7 days**

---

# Sync Policy

Developers must sync with main:

- Daily
- Before opening a PR
- Before merging

Command:

```bash
git fetch origin
git rebase origin/main