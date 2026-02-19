# Personal GitHub Workflow (Succinct)

**Goal:** finish projects by giving each GitHub feature one job.

---

## The Pipeline

**Idea → Active Work → Code → Understanding → Teaching**

Mapped to:  
**Issue → Project → Pull Request → Repo → Wiki → Blog (Zola)**

---
# flow 
branch protection on main
	- PR template + issue templates
	- Actions CI (even simple: format/lint/test/build)
	- 	squash-merge enabled
## 1) Issues — thinking & progress

Use for: ideas, plans, decisions, blockers, updates.  
Do not put polished docs.

**Rule:** if you’re working on it, it has an issue.  
Add short comments as checkpoints.

---

## 2) Projects — focus

A filtered view of issues.  
Keep only **1–3** in **Doing**.

**Question it answers:** *What do I work on today?*

---

## 3) Pull Requests — change history (the answer)

Every meaningful change goes through a PR, even solo.

A PR records:
- what changed
- why it changed
- what problem it solved

Always link the related issue.

Write a short explanation:

Problem:
Cause:
Solution:

**Question it answers:** *Why does the code look like this?*

---

## 4) Repository — implementation

Contains only how to run the software:

- README (build/run)
- minimal architecture

Link the tracking issue and relevant PR in the README.

**Question it answers:** *How does it operate?*

---

## 5) Wiki — durable knowledge

Concepts and lessons learned:

- systems explanations
- mental models
- post-project notes

No todos or daily logs.

**Question it answers:** *What did I learn?*

---

## 6) Zola — publication

Write after the project works and the wiki exists.  
Clean explanation for others.

**Question it answers:** *What can I teach?*

---

## Rules

1. No project without an issue.
2. Progress goes in issues, not README.
3. Changes go through pull requests.
4. Learning goes in wiki, not issues.
5. Blog only after completion.
6. Always cross-link **repo ↔ issue ↔ PR**.

---

**Outcome:** low cognitive load and resumable projects.