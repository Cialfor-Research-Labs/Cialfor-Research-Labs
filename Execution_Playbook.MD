# PD Team Execution Playbook 

---

## 1. Non-Negotiable Rules

* No PR → No Code Exists
* No Review → No Merge
* No CI Pass → No Progress
* No Issue → No Work

---

## 2. Work Lifecycle (MANDATORY FLOW)

### Step 1: Issue Creation

Every task MUST start as a GitHub Issue.

Types:

* Feature
* Bug
* Task

---

### Step 2: Branch Creation

Format:

```
feature/<issue-id>-<short-name>
bugfix/<issue-id>-<short-name>
```

Example:

```
feature/123-auth-api
```

---

### Step 3: Development Rules

* Pull latest `dev`
* No long-running branches (> 2 days)
* Commit frequently (clean commits only)
* Code must compile/run locally before push

---

### Step 4: Pull Request

PR must be raised within:

* 24 hours of starting work

---

### Step 5: Review Cycle

* Reviewer must respond within SLA
* Max 2 review cycles allowed
* If still failing → escalate to Lead

---

### Step 6: Merge Discipline

* Only after:

  * 2 approvals
  * CI success
* Use **Squash Merge**
* Delete branch after merge

---

## 3. Daily Team Sync Model

Each developer must:

* Update issue status
* Mention blockers
* Push at least one meaningful commit/day

---

## 4. Ownership Model

| Area           | Owner        |
| -------------- | ------------ |
| Feature        | Assigned Dev |
| Code Quality   | Reviewer     |
| Stability      | Repo Owner   |
| Final Decision | Team Lead    |

---

## 5. PR Size Rules

* Ideal: < 300 lines
* Max: 500 lines
* Above → MUST split

---

## 6. Failure Handling

If:

* CI fails → fix immediately
* Prod breaks → hotfix within 1 hour
* Repeated bad PRs → restricted merge access

---

## 7. Definition of Done (DoD)

A task is ONLY complete if:

* Code merged to `dev`
* CI passed
* Reviewed & approved
* Documentation updated (if needed)

---

## 8. Speed vs Quality Rule

Priority order:

1. Correctness
2. Stability
3. Speed

---

## 9. Golden Execution Rules

* Think → Code → Test → Push → PR → Fix → Merge
* Never “just push and see”
* Never bypass review
* Never ignore CI

---
[PR_TEMPLATE](PR_template.MD)


