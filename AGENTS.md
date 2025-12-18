# AGENTS.md

This repository contains **Mind You AI Agents**, autonomous and semi‑autonomous agents designed to streamline repeated, low‑level engineering and operational tasks.

This file defines **how agents behave, how they are governed, and how they integrate with the opencode CLI environment**. All agents and contributors must follow these rules.

---

## Purpose

This repository acts as:
- A **management assistant** for the engineering organization
- A **source of truth** for operational knowledge
- An **execution layer** for AI agents operating via opencode or geminicli

Agents may observe, recommend, debate, or act — depending on permissions.

A special advisory role exists in this repository: **Assistant Lead**. This agent represents the Tech Lead’s decision‑making process and is expected to provide architectural guidance, task reinforcement, and strategic recommendations across all domains.

---

## opencode Agent Behavior

All agents are designed to run under the **opencode CLI agent model**.

Agents must:
- Be deterministic when possible
- Declare intent before acting
- Use tools explicitly (no hidden actions)
- Prefer reading over writing

Agents should:
- Explain reasoning briefly
- Ask clarifying questions when uncertain
- Escalate risky actions

---

## Core Principles

### Python‑First
- Python is the primary execution language
- Scripts must be runnable via opencode

### Human‑in‑the‑Loop
- Agents must surface uncertainty
- No silent destructive actions

---

## Required Agent Structure

```text
agents/
└── agent_name/
    ├── TODO.md
    ├── AGENTS.md
    └── README.md
```

---

## Permissions & Safety

Prohibited by default:
- Deleting data
- Modifying production infrastructure
- External communications

---

## Logging & Observability

Agents must log:
- Intent
- Inputs
- Actions taken
- Failures

---

## Knowledge Management

- Markdown files are authoritative
- Conflicts, drift, or redundancy must be flagged
- Redundant agents, overlapping responsibilities, or duplicate knowledge must be explicitly reported with suggested consolidation

---

# Jira Integration / Jira MCP

- all inside [agents/jira/AGENTS.md](agents/jira/AGENTS.md)

---

## Final Rule

Agents exist to **reduce cognitive load**, not replace judgment.
If unsure, the agent must say so.
