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

## How the ecosystem works

<p align="center">
  <img src="https://raw.githubusercontent.com/Allura-Ecosystem/.github/main/assets/allura-ecosystem-map-v1.png" alt="Allura Ecosystem Map: how memory, teams, and plugins work together around the Allura Memory/Brain core." width="960">
</p>

Allura is the sovereign memory layer for AI. It gives teams and agents a trusted memory, connected context, and the tools to turn work into intelligent outcomes. The memory engine sits at the center; Team RAM, Team Durham, Allura Plugins, and Curator & Governance feed it evidence and draw governed context from it, and everything converges on the apps, agents, and outputs the system produces.

### Team RAM — AI engineering workforce

<p align="center">
  <img src="https://raw.githubusercontent.com/Allura-Ecosystem/.github/main/assets/allura-team-ram-v1.png" alt="Team RAM: AI Engineering Workforce. Task intake, Brooks orchestration, specialist functions (architecture, coding, review, testing, governance, routing), verification, merge and delivery, and lessons and memory." width="960">
</p>

Team RAM is the engineering workforce inside Allura: architecture, coding, testing, governance, routing, and self-improving workflows. You define the goal; the team builds it, verifies it, and makes it better.

### Team Durham — AI design & brand workforce

<p align="center">
  <img src="https://raw.githubusercontent.com/Allura-Ecosystem/.github/main/assets/allura-team-durham-v1.png" alt="Team Durham: AI Design and Brand Workforce. Discovery, strategy, messaging, UX, UI, accessibility, visual QA, and analytics loop." width="960">
</p>

Team Durham is the design, brand, and experience workforce inside the Allura ecosystem: strategy, UX, content, visual design, accessibility, and presentation quality — turning ideas into experiences that are clear, beautiful, inclusive, and on-brand.

### Team RAM vs Team Durham

<p align="center">
  <img src="https://raw.githubusercontent.com/Allura-Ecosystem/.github/main/assets/allura-team-ram-vs-durham-v1.png" alt="Team RAM vs Team Durham: RAM builds the system, Durham shapes the experience, and where they meet on product direction, human-centered AI, quality, and the final experience." width="960">
</p>

One builds the engine. One shapes the ride. When RAM and Durham work together, Allura delivers production-ready AI products that are powerful, human-centered, and built to last.

### One task across the Allura workforce

<p align="center">
  <img src="https://raw.githubusercontent.com/Allura-Ecosystem/.github/main/assets/allura-one-task-workforce-v1.png" alt="One task across the Allura workforce: a user request enters, Allura Memory/Brain understands and recalls, Team RAM builds the logic, Team Durham shapes the UX and message, plugins supply tools, Curator and Governance verifies, the final product is delivered, and feedback returns to memory." width="960">
</p>

Every task flows through the same governed loop: memory understands intent and retrieves context, the workforces build and shape, governance verifies, and feedback strengthens memory for the next task.

<p align="center"><sub>Ecosystem infographics. Allura’s published capabilities and implementation boundary are documented below.</sub></p>

---

## Agentic AI framework & harness

Allura is built as a **reusable agent framework and harness for enterprise software delivery** — the same capabilities that let engineering teams design, compose, test, and operationalize agentic workflows with correctness, composability, governance, and testability at scale.

| Capability | What Allura provides |
| --- | --- |
| **Agent orchestration & execution** | DAG-based process engine with step lifecycle events, checkpoint continuation, and event-sourced replay for deterministic runs. |
| **Memory patterns** | Append-only episodic ledger plus a curator-gated semantic layer over one PostgreSQL engine, with branchable working memory and tenant-scoped retrieval. |
| **Policy hooks & tool calling** | Control plane with 12 syscalls; every mutation requires proof-of-intent then policy evaluation before dispatch, through an authenticated MCP gateway with fail-closed tool calling. |
| **Simulator harness & evaluation** | Deterministic scenario runner with tool simulators, byte-for-byte receipt replay for determinism proof, and eval suites over scenario runs. |
| **SDK, API & CLI design** | Typed SDK (ESM + CJS), `allura run` / `allura replay` CLI, and a canonical HTTP gateway — one developer surface over the governed contracts. |
| **Framework scale & governance** | 59 forward-only migrations with forced RLS, immutable SHA-bound receipts, and CI evidence lanes that aggregate unit, build, live-PostgreSQL, benchmark, and evaluation artifacts. |

Every capability above is code, not copy — each maps to named source paths in [`FRAMEWORK.md`](https://github.com/Allura-Ecosystem/Allura_Memory/blob/main/FRAMEWORK.md), and the engineering narrative is in the [principal engineer case study](https://github.com/Allura-Ecosystem/Allura_Memory/blob/main/docs/portfolio/principal-engineer-case-study.md).

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
