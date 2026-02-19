# Personal GitHub Workflow: A Solo Engineering System

This document defines how to use GitHub as a complete development environment — not just for storing code, but for managing thinking, focus, knowledge, and publication.

The goal is simple:

> Remove mental overhead so projects can actually be finished.

Instead of using many disconnected tools, each GitHub feature is assigned **one clear responsibility**.

---

## The Core Idea

Think of your workflow as a pipeline:

```
Idea → Active Work → Code → Understanding → Teaching
```

Each stage maps to a specific GitHub feature.

You are not organizing files.
You are organizing **states of thought**.

---

## Layer 1 — Issues (Thinking & Work Tracking)

**Purpose:** External working memory and project reasoning.

Issues are *not* bug trackers. They are your development journal and planning system.

### What goes in Issues

* new ideas
* feature plans
* design decisions
* progress updates
* blockers
* debugging discoveries
* pivots and reasoning

### What does NOT go in Issues

* polished explanations
* tutorials
* long documentation pages

### How to use them

Treat comments like checkpoints in a game.

Examples of good comments:

* "Starting implementation using Go instead of Rust for libvirt bindings."
* "Blocked: vm IP discovery not working with bridged network."
* "Solution: need to read DHCP lease file from libvirt network."
* "MVP working locally. Next step: remote VM testing."

An issue answers:

> Why does this project exist and what has happened so far?

---

## Layer 2 — Projects (Focus)

**Purpose:** What you are actively doing *this week*.

A Project board is a filter over issues, not storage.

You should maintain:

* 1–3 issues in **Doing**
* several in **Todo**
* everything else left alone

This becomes your daily dashboard.

When you sit down to code, you do not decide what to work on.
You open the board and continue the top item in **Doing**.

The project board answers:

> What should I work on right now?

---

## Layer 3 — Repository (Implementation)

**Purpose:** The software itself and how to run it.

Repositories contain operational information only.

### What belongs in a repo

* README
* build instructions
* run instructions
* configuration
* brief architecture overview

### What does NOT belong

* design debates
* development logs
* idea brainstorming

The repository answers:

> How does this software operate?

Every repository should link to its tracking issue:

```
Tracking issue: https://github.com/<user>/ideas/issues/<id>
```

---

## Layer 4 — Wiki (Knowledge)

**Purpose:** Long‑term understanding and learning.

The wiki is your personal textbook — not a task list and not a journal.

### Put here

* how libvirt networking works
* paging and memory models
* tmux concepts
* Rust ownership mental models
* lessons learned from projects

### Do NOT put

* todos
* daily logs
* unfinished thoughts

The wiki answers:

> What did I learn from building this?

---

## Layer 5 — Zola (Publication)

**Purpose:** Clean teaching material and public explanation.

Zola is the final stage, not the starting stage.

A post should only be written **after**:

1. The project exists
2. The issue contains the journey
3. The wiki contains understanding

Now you distill the knowledge into something others can read.

Zola answers:

> What can I teach another developer?

---

## How the Pieces Work Together

Full workflow:

1. Create an idea → **Issue**
2. Start building → add issue to **Project (Doing)**
3. Write code → **Repository**
4. Learn concepts → document in **Wiki**
5. Clean explanation → publish in **Zola**

```
Issue → Project → Repo → Wiki → Blog
```

You never skip steps and you never reverse them.

---

## Why This Works

The real problem this solves is not organization — it is **cognitive load**.

Without a system, your brain keeps unfinished ideas in memory and repeatedly interrupts you while coding.

By storing each stage externally:

* Issues hold intention
* Projects hold focus
* Repos hold execution
* Wiki holds understanding
* Blog holds communication

Your brain no longer needs to remember everything simultaneously.

You can work on one project without fear of losing the others.

---

## Practical Rules

1. Never start a project without an issue.
2. Never track progress in the README.
3. Never write a blog post before the project works.
4. Never store learning notes in issues.
5. Always link repos ↔ issues.

---

## What This Enables

* Resume projects instantly
* Avoid re‑debugging old decisions
* Reduce context switching
* Finish more software
* Turn finished work into teaching material

This system turns GitHub from a code host into a **personal engineering environment**.
