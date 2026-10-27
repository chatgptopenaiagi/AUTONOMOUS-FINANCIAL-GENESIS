# Recorded capabilities

These are historical results from the original environment on **26–27 October 2026**, not fresh verification on the reader's computer. The [source catalogue](KNOWLEDGE-INDEX.md#evidence-sources) identifies the reports; [verification-summary.json](verification-summary.json) provides a small machine-readable snapshot.

## Financial Control Hub

| Capability | Recorded functional result | Boundary |
|---|---|---|
| Financial accounts | Account classes, status, currencies and synthetic balances | Local simulated accounts; no bank connection. |
| Transaction processing | Durable intent, explicit states, repeated-request checks, recovery and reconciliation | Unknown provider outcomes are retained rather than blindly resent. |
| Double-entry accounting | Per-currency balanced journals; exact integer minor units; compensating reversals | Not a regulatory or financial audit certification. |
| SQLite persistence | Ledger/provider state, migrations, rollback, backup and restart recovery tested | Coordinated recovery must preserve related stores. |
| Financial Control API | 29 distinct HTTP paths; real local requests passed | Local single-owner operation; no production access-control claim. |
| MCP integration | Official SDK exchange; Codex discovered 17 hub tools and invoked a balance read | Discovery/invocation acceptance did not use a model request. |
| Financial dashboard | Actual Edge browser acceptance, including failure behavior | Original local application; no hosted dashboard is distributed here. |
| Simulated trading | Existing controller research/simulation reused with isolated positions and cash settlement | One deterministic instrument and idealized execution. |
| SQL Server snapshot adapter | JSON/hash roundtrip and journal projection checked with temporary tables and rollback | SQLite remains operational; persistent dedicated deployment remains future work. |

The recorded acceptance deposited synthetic **EUR 100.00**, purchased **EUR 25.00** with no fee and ended at **EUR 75.00**. Two journals contained four balanced entries; all four simulated provider balances reconciled. Replaying the transaction identifier caused no duplicate movement. The run passed **74 hub tests** and **305 active workspace regressions**, with zero failures, errors or skips. These test scopes must not be added together as proof of all upstream software.

## Engineering intelligence and tools

| Area | Recorded achievement | Scope |
|---|---|---|
| Capability intelligence | 1,645 inventory records; 1,807 nodes; 496 relationships; 47 workflows; 92 outcomes; 20 causal cases | Evidence/component counts, not unique applications. |
| Routing and learning | Direct/indirect lookup, alternatives, compatible-environment reasoning, composition, history and causal repair memory | Plans return data; they do not execute proposed stacks. |
| Engine acceptance | 131 scoped tests and all ten advanced scenarios passed | Source metadata and environment changes can invalidate proof. |
| Numerical mathematics | GNU Octave 11.3.0 matrix result `[[19,22],[43,50]]`; Python scientific workflows | Specific operations and environment bindings were tested. |
| Symbolic mathematics | Maxima 5.50.0 differentiation result `4*x^3 + 6*x` | Bounded symbolic test. |
| Database tooling | SQLite workloads, local SQL Server 2022 connectivity and a SQL-to-Excel workflow | Does not establish every SQL Server optional feature. |
| Interoperability | Native C++/Python/NumPy; NumPy/SciPy/Matplotlib; Qt/SQLite; SQL/Excel; tiny PyTorch/CUDA calculation | Narrow executed workflows, not general compatibility certification. |
| Research laboratory | Ten scoped functional checks at project level; seven builds; three partial classifications | Optional hosted, AI, data and broker integrations have separate limits. |

The advanced paired routing benchmark used the same frozen graph, Python 3.14.9, three warmups and 50 alternating old/new pairs. Median numerical-query time changed from **10.1314 ms to 0.3299 ms** with semantic parity checks. This is a query-specific historical measurement, not a general application speedup.

## What remains incomplete

The hub has no implemented real bank/payment/broker connector. Persistent SQL Server deployment, production security and operational controls, realistic market execution and a controlled unattended scheduler are further work. A complete local inference/MCP chain was blocked in the advanced run. See [architecture](ARCHITECTURE.md), [system inventory](SYSTEM-INVENTORY.md) and [roadmap](ROADMAP.md).
