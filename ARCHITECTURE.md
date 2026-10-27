# Architecture

The architecture connects human-directed engineering, reusable software knowledge and a simulated financial execution path.

```text
HUMAN OWNER
     |
     v
OPENAI CODEX
     |
     v
CAPABILITY INTELLIGENCE
     |
     v
FINANCIAL CONTROL API
     |
     +-- ACCOUNT ENGINE
     +-- PAYMENT ENGINE
     +-- TRADING ENGINE
     |
     v
TRANSACTION CONTROLLER
     |
     v
SIMULATED FINANCIAL PROVIDERS
     |
     v
SQLITE ACCOUNTING LEDGER
     |
     v
FINANCIAL REPORTS
```

The diagram is a conceptual responsibility flow. The three engines feed shared transaction and accounting controls. It does not imply that capability selection automatically authorizes execution, or that every financial operation must pass through a model request.

## Human owner and OpenAI Codex

The owner defines objectives, constraints and authorized scope. Codex performs engineering work within those instructions: inspecting software, implementing changes, running checks and explaining results. Financial authority comes from explicit owner authorization, not from a tool recommendation.

The recorded hub acceptance verified Codex tool discovery and a read operation through its app-server protocol. It did not demonstrate an unattended model conducting financial business.

## Capability intelligence

GENESIS-3 supplies the authoritative software inventory. GENESIS-3.1 relates tools, runtimes, interfaces, dependencies and previous outcomes through a persistent graph and engineering history.

Queries can find direct or indirect capabilities, compare candidate stacks, predict known conflicts and retrieve verified workflows. Recommendations preserve evidence dates, environment bindings and uncertainty. They favor the smallest effective existing implementation. Query and planning commands return data; they do not install software or execute proposed stacks.

## Financial Control API and engines

The local Financial Control API exposes shared operations to the dashboard and MCP bridge. The implementation reuses an existing Python environment with FastAPI and the official MCP SDK.

| Component | Responsibility | Existing scope |
|---|---|---|
| Account engine | Account classification, status, currencies and balances | Synthetic local accounts with explicit currency precision. |
| Payment engine | Deposits, purchases, transfers and related payment workflows | Simulated provider effects, explicit transaction identity and tested replay handling. |
| Trading engine | Instruments, research, simulated orders, positions and settlement | Reuses GENESIS-1 simulation/research code with isolated hub-owned state. |
| Transaction controller | Validation, durable intent, state transitions, confirmation, recovery and reconciliation | Coordinates financial effects and accounting; retains unresolved outcomes without speculative resend. |

The trading controller's separate cTrader demo interface belongs to GENESIS-1. It is not an active banking or broker connector behind the hub's simulated providers. GENESIS-2 supplies research tools and reusable environments, rather than automatically wiring every upstream application into the API.

## Transaction control and providers

Transactions progress through explicit states from creation and validation to preparation, submission, confirmation and settlement. Failure, cancellation, uncertainty and reversal remain visible. Intent and submission ownership are durable before a provider side effect.

Simulated providers keep independent persistent state and confirmation records. After an interruption, the controller can reconcile confirmed effects and post them once. An interruption without verifiable confirmation remains uncertain; it is not silently retried.

The provider interface is an extension point. Real provider authentication, consent, confirmation semantics and reconciliation must be implemented and tested independently before any such connector can be considered functional.

## SQLite ledger and financial reports

SQLite is the operational accounting store. Double-entry journals balance per currency. Monetary inputs become integer minor units; unsupported precision and invalid numeric inputs are rejected. Original postings remain available when a reversal creates compensating entries.

Transaction identifiers and canonical payload checks suppress duplicate postings and reject conflicting reuse. Ledger records, provider confirmations and transaction history support reconciliation and reports. Recovery requires coordinated handling of the ledger, provider state and isolated trading state.

SQL Server currently provides a separately prepared snapshot adapter. Its temporary-table and rollback checks do not establish a deployed persistent snapshot service or a replacement operational ledger.

## Verified boundaries and future extensions

Local API calls, browser behavior, MCP exchange, synthetic ledger effects, replay protection and recovery were tested in the recorded GENESIS-4 run. This is a local single-owner simulation, with no real banking connector or live broker mutation in that acceptance.

Production operation would require further authorization controls, secret management, transport security, provider-specific integration, monitoring, recovery validation and applicable financial controls. More realistic execution and research models are also future work. The [roadmap](ROADMAP.md) describes those possibilities without treating them as installed capabilities.
