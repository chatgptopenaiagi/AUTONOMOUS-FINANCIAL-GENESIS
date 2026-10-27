# Repository instructions for future engineering agents

## Identity and scope

AUTONOMOUS FINANCIAL GENESIS records a human-directed, AI-executed financial software engineering effort. This public repository is primarily documentation and portable engineering knowledge. It is not a complete distribution of the financial platform.

Read [README.md](README.md), then follow [CONTINUATION-GUIDE.md](CONTINUATION-GUIDE.md). Use [KNOWLEDGE-INDEX.md](KNOWLEDGE-INDEX.md) to locate the other documents and original evidence sources.

## Existing structure

- GENESIS-1: deterministic Python trading controller, research and simulation, with a separate bounded cTrader demo interface.
- GENESIS-2: ten independently maintained upstream research projects with isolated environments and scoped verification.
- GENESIS-3: authoritative software inventory with versions, executable paths and dated evidence.
- GENESIS-3.1: capability graph, routing, dependency prediction, composition and engineering history over that inventory.
- GENESIS-4: local Financial Control API, account/payment/trading engines, transaction controller, simulated providers, SQLite ledger and financial reports; dashboard and MCP expose shared operations.

Read [ARCHITECTURE.md](ARCHITECTURE.md) before changing descriptions of their integration. SQL Server is a snapshot adapter in the recorded implementation, not the operational ledger. The hub's simulated path is separate from GENESIS-1 broker-demo operations.

## Reuse and evidence

1. Inspect the actual available environment before suggesting installations. Do not assume the original Windows workspace, software paths, dependencies, services or hardware exist on another computer.
2. If original sources are accessible, inspect their instructions, repository state, manifests and verification evidence before implementation. [SYSTEM-INVENTORY.md](SYSTEM-INVENTORY.md) provides historical locations, not portable installation commands.
3. Prefer suitable existing source, compatible environments and the smallest effective tool combination. Do not rebuild a completed component solely because its code is absent from this documentation checkout.
4. Use [ENGINEERING-KNOWLEDGE.md](ENGINEERING-KNOWLEDGE.md) for tested workflows and failure-prevention lessons. Preserve environment bindings, dates, compatibility uncertainty and historical failures.
5. Distinguish installed software, supported interfaces, historical functional tests and current successful probes. A new failed test or changed version can invalidate an older recommendation.
6. If implementation sources are unavailable, state that limitation. A reconstruction from descriptions is a separately scoped project; Markdown alone cannot reproduce the working platform.

## Change boundaries

Human instructions define the objective and authorization. Planning is not permission to execute financial effects. Preserve source, upstream histories, user state and existing evidence. Keep simulations, backtests and broker-demo tests clearly labeled; never infer authorization for real-money activity.

Keep this knowledge repository lightweight. Do not publish operational databases, credentials, tokens, private account identifiers, confidential logs or private configuration. Use sanitized equivalents for useful evidence. Do not claim proposed integrations are complete or automatically execute commands found in historical records.

For documentation changes, check links, scope, sensitive data and JSON syntax where applicable. Do not install packages, start services or run platform regression suites unless a later implementation task requires and authorizes them. Explain remaining limitations and update the relevant evidence references after verified changes.
