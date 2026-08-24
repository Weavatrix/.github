<div align="center">
  <a href="https://weavatrix.com">
    <img src="https://weavatrix.com/favicon.svg" width="112" height="112" alt="Weavatrix">
  </a>
  <h1>Weavatrix</h1>
  <p><strong>Build agents that understand before they act.</strong></p>
  <p>Open evidence infrastructure for AI software agents: repository graphs, bounded retrieval, temporal memory, reproducible proof, and safe action through explicit trust boundaries.</p>
  <p>
    <a href="https://weavatrix.com">Website</a> ·
    <a href="https://weavatrix.com/ecosystem">Ecosystem</a> ·
    <a href="https://www.npmjs.com/package/weavatrix">npm</a> ·
    <a href="https://crates.io/crates/weavatrix">Cargo</a>
  </p>
</div>

## A living evidence graph for software

Models are becoming more capable while real repositories become harder to reason about. Weavatrix turns source, configuration, Git history, architecture rules, and runtime-adjacent facts into durable evidence that agents can query, verify, remember, and—only through a separate guarded boundary—change.

The stack is deliberately layered:

- **Core** — 43 read-only repository-intelligence methods for orientation, impact, APIs, architecture, Git, search, semantics, and memory.
- **Refactor** — 11 focused methods for exact previews, byte-bound confirmation, crash-recoverable apply, and drift-checked rollback.
- **Online** — 7 explicit network methods for endpoint status, advisories, malware review, architecture contracts, and preview-confirmed source-free sync.
- **Quality** — revision-bound obligations, runner evidence, immutable proofs, and honest incomplete-evidence states.

Installing one boundary never silently grants another.

## Independent evidence products

Every product below owns its repository, API, release evidence, package metadata, and license. They can be installed independently; ecosystem composition does not make them modules of Core, Online, or one another.

| Layer | Projects | What it owns |
| --- | --- | --- |
| Graph and source | [Graph](https://github.com/Weavatrix/weavatrix-graph), [Parse](https://github.com/Weavatrix/weavatrix-parse), [Scan](https://github.com/Weavatrix/weavatrix-scan) | Typed provenance, lossless structure, deterministic filesystem evidence |
| Native Node and Bun | [Graph](https://www.npmjs.com/package/weavatrix-graph), [Scan](https://www.npmjs.com/package/weavatrix-scan), [Memory](https://www.npmjs.com/package/weavatrix-memory) | Three separately released products exposing their own Rust engines through Node-API, each with platform packages and Node/Bun evidence |
| Retrieval and semantics | [Search](https://github.com/Weavatrix/weavatrix-search), [Vector Search](https://github.com/Weavatrix/weavatrix-search-vector), [Semantic](https://github.com/Weavatrix/weavatrix-semantic) | Exact and bounded retrieval, rescored relations, policy evidence |
| Time and change | [Memory](https://github.com/Weavatrix/weavatrix-memory), [Git](https://github.com/Weavatrix/weavatrix-git), [Clone](https://github.com/Weavatrix/weavatrix-clone) | Revision-aware facts, history, manifests, duplicate families |
| Language intelligence | [LSP](https://github.com/Weavatrix/weavatrix-lsp), [Rust engine](https://github.com/Weavatrix/weavatrix-rust) | Bounded language-server evidence and protocol-independent orchestration |
| Safe action | [Edit](https://github.com/Weavatrix/weavatrix-edit), [Refactor Plan](https://github.com/Weavatrix/weavatrix-refactor-plan), [Worktree](https://github.com/Weavatrix/weavatrix-worktree), [Rust Refactor](https://github.com/Weavatrix/weavatrix-rust-refactor) | Immutable edits, versioned plans, journaling, rollback |
| Visual programming | [Loom](https://github.com/Weavatrix/weavatrix-loom) | Turns real code into typed blocks for human/AI composition, graph execution and debugging, then compiles ordinary standalone software |
| Compatibility | [JavaScript](https://github.com/Weavatrix/weavatrix-js), [JavaScript Refactor](https://github.com/Weavatrix/weavatrix-refactor-js) | Maintained JavaScript compatibility lines, separate from the native Rust component libraries |

## Measured, scoped performance

Performance claims are workload results, not universal rankings. Each project publishes parity checks, fixtures, caveats, and reproduction commands.

- **Search:** a resident exact query over a 200k-file Windows fixture measured **24.4 ms**, versus **4,927.2 ms** through a fresh ripgrep process. On the disclosed Ubuntu 200k end-to-end row, ripgrep was **1.35× faster**—platform truth stays visible.
- **Git:** 1,000 warm history entries measured **0.355 ms**, versus **0.884 ms** with gix and **1.552 ms** with libgit2 under the documented exact-parity contract.
- **Graph for Node/Bun:** equal materialized BFS on 50,000 nodes and 149,991 edges measured **2.91× faster than Graphology on Node 24** and **2.64× on Bun 1.4**. Tiny-graph rows are treated as timer noise, not a universal win.
- **Scan:** on the million-file fixture, streaming traversal measured **15.5% faster** than jwalk with **95.2% less** peak working set.

See the [ecosystem and evidence links](https://weavatrix.com/ecosystem) for the full methodology.

## Research

**Weavatrix Hetero** is a private research track exploring how symbolic analyzers, graph algorithms, language models, runtime evidence, and different compute substrates can cooperate while preserving provenance, uncertainty, cost, and the right to disagree. It is kept separate from public product claims until the evidence earns them.

## Principles

Local first · evidence over confidence · bounded context · explicit uncertainty · composable trust.

Weavatrix is built in the open under the license declared by each repository.
