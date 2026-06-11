# Allura

<p align="center">
  <img src="https://raw.githubusercontent.com/Allura-Ecosystem/.github/main/assets/allura-wordmark.png" alt="Allura" width="420">
</p>

**MEMORY THAT SHOWS ITS WORK**

Allura is an open-source ecosystem for governed AI memory. It helps agent
systems preserve context, show where knowledge came from, and place human
approval between raw evidence and long-term knowledge.

<p align="center">
  <img src="https://raw.githubusercontent.com/Allura-Ecosystem/.github/main/assets/allura-ecosystem-map.svg" alt="Map of the public Allura ecosystem connecting Allura Memory, Allura Desktop, Team RAM, protocols, and the reserved allura repository." width="100%">
</p>

## Start Here

Begin with
[`Allura_Memory`](https://github.com/Allura-Ecosystem/Allura_Memory).
Its documentation explains the memory model, architecture, installation path,
governance rules, and supported agent integrations.

## Public Repositories

| Repository | Public role |
| --- | --- |
| [`Allura_Memory`](https://github.com/Allura-Ecosystem/Allura_Memory) | Self-hosted memory and governance engine for AI agents |
| [`Allura_Desktop`](https://github.com/Allura-Ecosystem/Allura_Desktop) | Tauri-based desktop command-center project for the Allura ecosystem |
| [`allura-team-ram`](https://github.com/Allura-Ecosystem/allura-team-ram) | Agent harness with surgical-team orchestration for the Allura ecosystem |
| [`allura`](https://github.com/Allura-Ecosystem/allura) | Reserved public ecosystem repository; no public documentation is available yet |

Descriptions above are deliberately narrow. Each repository's code and
documentation remain authoritative for its implemented and planned behavior.

## How Allura Treats Memory

Allura separates raw evidence from approved knowledge:

1. Agent activity is captured as traceable, append-only evidence.
2. Candidate knowledge is scored and placed behind a review boundary.
3. Approved knowledge is promoted with provenance and audit history intact.
4. Retrieval preserves tenant boundaries and source context.

The system is designed around inspectability, governance, self-hosting, and
human agency over stored knowledge.

<p align="center">
  <img src="https://raw.githubusercontent.com/Allura-Ecosystem/.github/main/assets/governed-memory-flow.svg" alt="Five-stage governed memory flow: capture evidence, evaluate candidates, human review, promote approved knowledge, and retrieve with provenance." width="100%">
</p>

## Governance Principles

- Evidence before completion claims
- Human approval before governed promotion
- Provenance before reuse
- Tenant boundaries before retrieval
- Explicit degraded or unknown states
- Reproducible verification for public claims

## Public Scope

This page describes only repositories and capabilities visible in the public
organization. Private work, internal infrastructure, client implementations,
and unverified runtime status are intentionally excluded.

## Participate

- Read [CONTRIBUTING.md](https://github.com/Allura-Ecosystem/.github/blob/main/CONTRIBUTING.md) before proposing changes.
- Report security concerns using [SECURITY.md](https://github.com/Allura-Ecosystem/.github/blob/main/SECURITY.md).
- Follow the [Code of Conduct](https://github.com/Allura-Ecosystem/.github/blob/main/CODE_OF_CONDUCT.md).

Allura is memory that shows its work. Its public claims should do the same.
