# Prompts

This directory contains executable prompt implementations for agents in the Engineering Operating System.

Agent specifications are stored in:

`../500_agent_specifications/`

Prompts are implementations of those specifications.

A prompt shall not be treated as the agent definition itself.

The agent definition is the specification.

The prompt is the current executable version of that specification.

---

# Directory Structure

```text
prompts/
├── README.md
├── system/
│   ├── core/
│   └── specialists/
└── tests/
```

## `system/core/`

Contains system prompts for core EOS agents.

Examples:

* Constitution Guardian
* Engineering OS Orchestrator
* Engineering Knowledge Manager
* Independent Auditor

## `system/specialists/`

Contains system prompts for specialist agents.

Examples:

* Requirements Engineer
* Homologation & Compliance Agent
* Functional Safety Agent
* Electrical Engineering Agent
* Mechanical Engineering Agent
* Software / Embedded Agent
* Test & Validation Agent

## `tests/`

Contains prompt test conversations, expected behavior examples and activation test cases.

---

# Prompt Rules

1. Every active prompt must reference an agent specification.
2. Every active prompt must have a version.
3. Every active prompt must have a change history.
4. Every active prompt must be tested before activation.
5. Prompt changes must be documented.
6. Prompt changes shall not bypass governance.
7. A prompt is not active until it is listed in the Agent Registry.
8. A prompt implementation must not contradict the Constitution.
9. A prompt implementation must not extend an agent’s authority beyond its specification.
10. Prompt changes affecting governance require Constitution Guardian review.

---

# Relationship Between Specification and Prompt

The EOS separates agent specification from prompt implementation.

## Agent Specification

Defines:

* mission,
* scope,
* responsibilities,
* limits,
* inputs,
* outputs,
* interfaces,
* review requirements.

Stored in:

`../500_agent_specifications/`

## Prompt Implementation

Defines:

* executable system prompt,
* model-facing behavior,
* response format,
* operational constraints,
* tool usage instructions,
* version-specific behavior.

Stored in:

`prompts/`

This separation allows the same agent specification to be implemented for different models, runtimes or tools without changing the organizational role of the agent.

---

# Source of Truth

For active prompt implementations, this directory is the source of truth.

For agent role definitions, the source of truth remains:

`../500_agent_specifications/`

For agent status, the source of truth is:

`../200_organization/AGENT_REGISTRY.md`
