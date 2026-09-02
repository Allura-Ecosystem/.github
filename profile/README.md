# allura

<p align="center">
  <img src="https://raw.githubusercontent.com/Allura-Ecosystem/.github/main/assets/allura-wordmark.png" alt="Allura wordmark" width="360">
</p>

<p align="center"><strong>Memory that shows its work.</strong></p>

<p align="center">
  Allura gives agentic systems a governed way to retain evidence, review what becomes reusable knowledge, and preserve the context behind every retrieval.
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/Allura-Ecosystem/.github/main/assets/allura-governance-flow-diagram-v1.png" alt="Governance is part of the flow: a proposed action passes through policy, human approval, and evidence retention around the Allura agent workflow." width="960">
</p>

<p align="center"><sub>Product-support diagram. Allura’s published capabilities and implementation boundary are documented below.</sub></p>

---

## Start with the source of truth

[`Allura_Memory`](https://github.com/Allura-Ecosystem/Allura_Memory) is the authoritative public product repository. Its code and documentation define the engine boundary, memory lifecycle, governance rules, supported interfaces, and current implementation status.

For a framework-level view of orchestration, memory patterns, policy hooks, harnesses and evaluation, and SDK design, read [`FRAMEWORK.md`](https://github.com/Allura-Ecosystem/Allura_Memory/blob/main/FRAMEWORK.md).

## How Allura handles memory

| Stage | What happens | Why it matters |
| --- | --- | --- |
| **Capture** | Agent activity is retained as append-only episodic evidence in PostgreSQL. | The original context remains available for inspection. |
| **Review** | Candidate memory is scored and governed knowledge is routed through review. | Reuse is a considered decision, not an automatic side effect. |
| **Promote** | Approved knowledge is promoted into versioned PostgreSQL canonical graph tables. | The reusable record has a clear state and lineage. |
| **Retrieve** | Scoped memory is accessed through controlled MCP and API interfaces. | Retrieval respects the system’s boundaries. |
| **Account for it** | Source, actor, decision, and audit context remain attached through the lifecycle. | A memory-backed response can show where it came from. |

## Product surfaces

| Surface | Role |
| --- | --- |
| **Allura Memory Engine** | Canonical memory data plane and source of truth. |
| **MCP and API** | Primary integration path for agents and applications. |
| **Memory Command Center** | Optional, launch-gated operator view over the same governed contracts. |
| **Curator and RuVix governance** | Human review, policy disposition, and evidence receipts. |

The Memory Command Center is not a second memory system. It may inspect and request governed actions, but it cannot bypass the engine or own canonical state.

## Principles we build around

- Evidence before completion claims.
- Human approval before governed promotion.
- Provenance before reuse.
- Tenant boundaries before retrieval.
- Explicit degraded or unknown states.
- Reproducible verification for public claims.

## The ecosystem

GitHub may display other public repositories owned by this organization. Some are supporting experiments, delivery harnesses, or reserved namespaces; visibility does not make them equal parts of the Allura product.

| Repository | Role |
| --- | --- |
| [`Allura_Memory`](https://github.com/Allura-Ecosystem/Allura_Memory) | Canonical governed memory engine, MCP server, SDK, policy hooks, and evidence authority |
| [`allura-team-ram`](https://github.com/Allura-Ecosystem/allura-team-ram) | Canonical governed multi-agent software-delivery harness for OpenCode, Claude Code, and Codex |
| [`team-durham`](https://github.com/Allura-Ecosystem/team-durham) | Canonical governed multi-agent brand-production harness for strategy, design, accessibility, evidence, and QA |
| [`mortagate`](https://github.com/Allura-Ecosystem/mortagate) | Canonical Microsoft Copilot Cowork mortgage evidence-review product |
| [`allura-plugins`](https://github.com/Allura-Ecosystem/allura-plugins) | Installation catalog and pinned generated exports from the standalone canonical repositories |
| [`Allura-ecosystem`](https://github.com/Allura-Ecosystem/Allura-ecosystem) | Ecosystem map, governance policies, enforcement plugin, and architecture index |

---

Allura is memory that shows its work. Its public claims should do the same.
