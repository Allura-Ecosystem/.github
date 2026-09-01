# allura

<p align="center">
  <img src="https://raw.githubusercontent.com/Allura-Ecosystem/.github/main/assets/allura-wordmark.png" alt="allura" width="360">
</p>

**MEMORY THAT SHOWS ITS WORK**

allura is a self-hosted, governed memory engine for AI systems. It preserves
raw evidence, places review between capture and reusable knowledge, and keeps
provenance attached when memory is retrieved.

## Canonical Project

[`Allura_Memory`](https://github.com/Allura-Ecosystem/Allura_Memory) is the
authoritative public product repository.

Its code and documentation define the engine boundary, memory lifecycle,
governance rules, supported interfaces, and current implementation status.

## What allura Does

1. Captures agent activity as append-only episodic evidence in PostgreSQL.
2. Scores candidate memory and routes governed knowledge through review.
3. Promotes approved knowledge into versioned PostgreSQL canonical graph tables.
4. Retrieves scoped memory through controlled MCP and API interfaces.
5. Preserves source, actor, decision, and audit context through the lifecycle.

## Product Surfaces

| Surface | Role |
| --- | --- |
| **Allura Memory Engine** | Canonical memory data plane and source of truth |
| **MCP and API** | Primary integration path for agents and applications |
| **Memory Command Center** | Optional, launch-gated operator view over the same governed contracts |
| **Curator and RuVix governance** | Human review, policy disposition, and evidence receipts |

The Memory Command Center is not a second memory system. It may inspect and
request governed actions, but it cannot bypass the engine or own canonical
state.

## Repository Scope

GitHub may display other public repositories owned by this organization. Some
are supporting experiments, delivery harnesses, or reserved namespaces. Their
visibility does not make them equal parts of the allura product.

## Governance Principles

- Evidence before completion claims
- Human approval before governed promotion
- Provenance before reuse
- Tenant boundaries before retrieval
- Explicit degraded or unknown states
- Reproducible verification for public claims

## Start Here

Read the
[`Allura_Memory` documentation](https://github.com/Allura-Ecosystem/Allura_Memory#readme)
for architecture, installation, integration paths, and current evidence.

For a framework-level overview mapping the codebase to agentic AI concepts
(orchestration, memory patterns, policy hooks, harness/eval, SDK design), see
[`FRAMEWORK.md`](https://github.com/Allura-Ecosystem/Allura_Memory/blob/main/FRAMEWORK.md).

## Ecosystem Repositories

| Repository | Role |
| --- | --- |
| [`Allura_Memory`](https://github.com/Allura-Ecosystem/Allura_Memory) | Canonical governed memory engine, MCP server, SDK, policy hooks, and evidence authority |
| [`allura-team-ram`](https://github.com/Allura-Ecosystem/allura-team-ram) | Canonical governed multi-agent software-delivery harness for OpenCode, Claude Code, and Codex |
| [`team-durham`](https://github.com/Allura-Ecosystem/team-durham) | Canonical governed multi-agent brand-production harness for strategy, design, accessibility, evidence, and QA |
| [`mortagate`](https://github.com/Allura-Ecosystem/mortagate) | Canonical Microsoft Copilot Cowork mortgage evidence-review product |
| [`allura-plugins`](https://github.com/Allura-Ecosystem/allura-plugins) | Installation catalog and pinned generated exports from the standalone canonical repositories |
| [`Allura-ecosystem`](https://github.com/Allura-Ecosystem/Allura-ecosystem) | Ecosystem map, governance policies, enforcement plugin, and architecture index |

allura is memory that shows its work. Its public claims should do the same.
