# govctl-org

**Bringing determinism to AI coding.**

---

## The Problem

AI coding assistants are powerful — but they lack discipline:

- **No structure** — changes happen anywhere, anytime, in any order
- **No traceability** — "why was this changed?" gets lost in conversation history
- **No gates** — nothing stops half-baked code from reaching production
- **No coordination** — multiple agents step on each other's work

The result? Fast but fragile. Productive but unpredictable.

## Our Mission

We build tools that enforce **structure**, **traceability**, and **phase discipline** on AI-assisted development workflows.

Every change flows through a governed lifecycle:

```
┌──────────┐     ┌──────────┐     ┌──────────┐     ┌──────────┐
│   SPEC   │ ──▶ │   IMPL   │ ──▶ │   TEST   │ ──▶ │  STABLE  │
│ Document │     │  Build   │     │  Verify  │     │  Ship    │
└──────────┘     └──────────┘     └──────────┘     └──────────┘
```

No shortcuts. No chaos. Just determinism.

---

## Products

### 🔧 [govctl](https://github.com/govctl-org/govctl) — Governance CLI

![Live](https://img.shields.io/badge/status-live-22c55e)

Opinionated CLI for RFC-driven development. Enforces phase gates, tracks decisions, and keeps AI agents in line.

```bash
govctl rfc new "Add user authentication"   # Create RFC
govctl work start RFC-001                  # Begin implementation
govctl gate check                          # Validate before advancing
govctl phase advance                       # Move to next phase
```

### ⚡ [skillc](https://github.com/govctl-org/skillc) — Skill Compiler

![Live](https://img.shields.io/badge/status-live-22c55e)

Development kit for [Agent Skills](https://agentskills.io/). Scaffold, lint, compile, and analyze skills for AI coding assistants.

```bash
skc init my-skill          # Scaffold new skill
skc lint                   # Validate structure
skc build                  # Compile for distribution
skc stats                  # Analyze usage patterns
```

### 🔀 jjgov — Multi-Agent Collaboration

![Coming Soon](https://img.shields.io/badge/status-coming%20soon-a1a1aa)

jj-based workflow for coordinating multiple AI agents working on the same codebase. Parallel branches, clean merges, no conflicts.

### 🧬 everevolve — Living Project Rules

![Coming Soon](https://img.shields.io/badge/status-coming%20soon-a1a1aa)

Automatically generate and evolve project rules from commit history. Your codebase teaches the AI how to contribute.

---

## Philosophy

> _"Good programmers worry about data structures and their relationships."_

We believe:

- **Constraints enable creativity** — structure doesn't slow you down, chaos does
- **Decisions should be traceable** — every "why" deserves a documented answer
- **AI needs guardrails** — powerful tools require disciplined processes
- **Phase gates work** — they've worked in engineering for decades

---

## Links

| Resource       | URL                                                                 |
| -------------- | ------------------------------------------------------------------- |
| 🌐 Website     | [govctl.org](https://govctl.org)                                    |
| 📖 govctl Docs | [govctl-org.github.io/govctl](https://govctl-org.github.io/govctl/) |
| 📖 skillc Docs | [govctl-org.github.io/skillc](https://govctl-org.github.io/skillc/) |
| 📝 Blog        | [govctl.org/blog](https://govctl.org/blog)                          |

---

<p align="center">
  <sub>Built with phase discipline. Governed by govctl.</sub>
</p>

