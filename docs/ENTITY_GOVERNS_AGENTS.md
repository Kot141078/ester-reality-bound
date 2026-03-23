# Entity governs agents

## Rule
By default, `c` orchestrates agents; agents do not define `c`.

## Operational meaning
An agent is a bounded worker process, tool-caller, or specialized execution role. An agent may use models, retrieval, tools, or external services. It does not hold the primary continuity of the system.

## Why this matters under L4
When complexity exceeds direct human handling, `c` is the layer that preserves human intent, applies L4 constraints, and coordinates bounded agents. Without this layer, privilege drift, workflow shortcuts, and obedience-style failures become easier.

## What stays at `c`
- continuity
- privilege holding and delegation
- timing and stopping conditions
- challenge / veto handling
- witness / evidence responsibility

## What stays with `a`
- accountable anchoring
- authorship / responsibility context
- ultimate escalation authority

## Hard rule
A model, a judge, or an agent swarm is not the entity. These are components or surfaces under `c`.
