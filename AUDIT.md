# Repository Workflow Audit

## Problem 1 – Direct commits to main

**Evidence**

Commit: `abc1234`

Commit message: `fix`

### Meaning

Developers are committing directly to the main branch without code review.

### Risk

Broken code can immediately reach production and bypass team review.

---

## Problem 2 – Poor commit messages

**Evidence**

Commit: `def5678`

Message: `update`

### Meaning

The commit history provides no explanation of what changed.

### Risk

Debugging and reverting changes becomes difficult.

---

## Problem 3 – Poor branch naming

**Evidence**

Branch:
