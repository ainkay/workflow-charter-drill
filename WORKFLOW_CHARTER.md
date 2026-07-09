## Validation Gates

### 1. Build Validation

Checks whether the application builds successfully.

Failure:
The PR cannot be merged.

Workflow:
.github/workflows/ci.yml

---

### 2. Unit Tests

Runs all automated tests.

Failure:
The PR is blocked until tests pass.

Workflow:
.github/workflows/ci.yml

---

### 3. Linting

Checks formatting and coding standards.

Failure:
Merge is blocked.

Workflow:
.github/workflows/ci.yml

---

### 4. Security / Dependency Checks

Scans dependencies for known vulnerabilities.

Failure:
The PR cannot be merged until vulnerabilities are addressed.

Workflow:
.github/workflows/ci.yml

---

### Non-Negotiable Rule

No validation gate may be bypassed, even under deadline pressure. Every pull request must pass all required checks before merging into `main`.