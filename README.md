# AUTONOMOUS FINANCIAL GENESIS

Human-directed engineering with OpenAI Codex, persistent software knowledge and a simulated financial platform.

This repository documents the ideas, development process and verified achievements of five GENESIS stages. The human owner defines the goals; Codex performs authorized engineering work using existing software tools. The platform source code, execution environments, account data and private engineering evidence remain outside this repository.

**Status:** an existing local engineering platform with tested research, capability intelligence and simulated financial operations. Real financial-provider integrations and production deployment remain future work.

## Explore the project

| Read | What it explains |
|---|---|
| [Project history](PROJECT-HISTORY.md) | How the five GENESIS stages evolved. |
| [Engineering philosophy](ENGINEERING-PHILOSOPHY.md) | Human direction, AI execution and reusable verified knowledge. |
| [Architecture](ARCHITECTURE.md) | Components, accounting flow and integration boundaries. |
| [Capabilities](CAPABILITIES.md) | Recorded functional results and their limits. |
| [Roadmap](ROADMAP.md) | Future concepts and the checks they would require. |
| [Contributing](CONTRIBUTING.md) · [Changelog](CHANGELOG.md) | How to propose improvements and what changed. |

## Vision and motivation

The aim is to make financial software development cumulative. Each engineering task should reuse installed tools, successful workflows and known repairs instead of starting again. Financial decisions and effects should remain explicit, traceable and subject to the human owner's authority.

The platform began with a practical question: can a human owner direct Codex to discover available software, build useful financial tools, test their behavior, repair actual failures and retain the resulting knowledge for the next task?

GENESIS developed through that process. Its long-term vision is an increasingly capable engineering assistant and financial research environment. The current implementation demonstrates bounded technical capabilities; it does not establish profitable trading or autonomous control of real funds.

## How the human owner and Codex worked together

The owner set objectives, selected priorities, authorized scope and defined acceptance criteria. Codex inspected the existing environment, chose available tools, implemented changes and ran representative checks. When a method failed, it investigated the evidence, applied a scoped repair and verified the result.

The recurring process was:

**DISCOVER → BUILD → TEST → REPAIR → VERIFY → RECORD → REUSE.**

Inventory records, test results, workflow history and failure explanations became persistent engineering memory. Installed software, historical success, current functional proof and unverified compatibility remain separate states. A newer failure can block a recommendation until a repair is verified.

Recorded repairs included choosing a compatible existing runtime after a dependency conflict, releasing SQLite handles before file cleanup, and correcting payment recovery and failed-payment dashboard behavior. Each repair was followed by a scoped check; the original failure evidence was retained.

## Five stages of development

| Stage | Purpose | Existing engineering result |
|---|---|---|
| GENESIS-1 | Trading controller | A deterministic Python interface for research, simulation, public market data, journaling, reporting and separately authorized cTrader demo operations. Inputs and broker identity are checked before allowed mutations. |
| GENESIS-2 | Open-source trading research laboratory | Ten independently maintained upstream projects with isolated environments, provenance and representative local functional checks. Optional features remain separately classified. |
| GENESIS-3 | Windows software capability registry | An evidence-based inventory of installed tools, exact executables, versions, environments and verification status, retained for future Codex sessions. |
| GENESIS-3.1 | Capability intelligence engine | Graph queries, dependency prediction, alternative selection, multi-tool composition, workflow reuse and causal error memory over the existing registry. |
| GENESIS-4 | Financial Control Hub | A local API, dashboard and MCP interface around simulated accounts, payments, trading, transaction recovery, accounting and reports. |

GENESIS-2 includes NautilusTrader, Freqtrade, Jesse, VeighNa, LEAN, TradingGym, TradingGoose-Studio, ta4j, OpenStock and Qbot. These remain separate upstream projects. Their local checks do not certify every integration or establish broker readiness.

## Financial platform architecture

The human owner directs Codex. Capability intelligence helps select suitable installed tools. The Financial Control API exposes account, payment, trading and reporting operations. A transaction controller records intent, validates transitions and coordinates simulated providers. A SQLite ledger preserves accounting entries for reconciliation and reports.

This is a conceptual view of the existing components and their intended cooperation. Capability planning does not automatically execute a stack or authorize a financial operation. The hub currently reuses the controller's simulation and research interfaces; its simulated provider path is separate from the controller's broker-demo path.

See [ARCHITECTURE.md](ARCHITECTURE.md) for component relationships and current boundaries.

## Verified capabilities

The following results are snapshots from local engineering reports dated **26–27 October 2026**. They summarize recorded tests; publishing this repository did not repeat those tests or execute transactions.

| Area | Recorded result | Scope |
|---|---|---|
| Trading laboratory | 10 acquired projects with representative functional checks; 7 recorded builds and 3 partial classifications | Public or synthetic data; optional services and account-dependent features have limits. |
| Capability intelligence | 1,645 inventory records; 1,807 graph nodes; 496 relationships; 47 workflows; 92 engineering outcomes; 20 causal cases | Component/evidence counts, not unique applications or financial customers. |
| Advanced engine verification | 131 scoped automated tests and all 10 acceptance scenarios passed | Includes selection, dependency conflicts, compilation, workflow reuse and failure prevention. |
| Mathematics | GNU Octave 11.3.0 returned `[[19, 22], [43, 50]]` for a 2×2 matrix product; Maxima 5.50.0 returned `4*x^3 + 6*x` for the requested derivative | Bounded numerical and symbolic execution checks. |
| Cross-tool engineering | Native C++ library called from Python, scientific plotting, Qt with SQLite, SQL-to-Excel calculation and a small PyTorch GPU calculation passed | Specific tested combinations and environments; broader compatibility is not assumed. |
| Financial Control Hub | 74 hub tests and 305 active workspace regressions passed in its recorded run | Separate test scopes; counts are not additive proof of every upstream project. |
| Financial interfaces | Local HTTP API, browser dashboard, official MCP exchange and Codex discovery of 17 hub tools passed | Local simulated operation; no live banking connector or model request was used in that acceptance. |

Persistent JSON, TOML and SQLite representations preserve inventory and capability evidence. Routing can explain selected tools, dependencies, alternatives, compatibility uncertainty and previous failures.

## Simulated banking and trading

The recorded hub acceptance started with a **synthetic EUR 100.00 deposit**, made a **synthetic EUR 25.00 purchase** and ended at **EUR 75.00** with no fee. Two journals produced four balanced entries. Repeating the same transaction identifier produced no duplicate journal or balance movement. Provider and ledger balances reconciled.

Money uses integer minor units with explicit currency precision. The hub records durable intent before provider effects, checks payload identity for repeated requests and retains uncertain outcomes for reconciliation instead of automatically resending them. Reversals preserve original entries through compensating postings.

Hub trading uses a deterministic fixture, idealized simulated execution and existing research code. Its positions and settlement state are isolated from the original controller's journals. Historical backtests, synthetic simulation and broker-confirmed demo tests are distinct evidence categories. None establishes real-money performance.

## Current limitations

- Real bank, payment and broker connectors are not implemented or enabled in the hub. Its providers and funds are simulated.
- SQLite is the operational ledger. SQL Server snapshot roundtrips were tested with temporary tables and rollback; persistent deployment and an operational SQL Server backend remain separate work.
- Hub trading covers one synthetic instrument with idealized fills. It does not model margin, financing, slippage or production market feeds.
- Production authorization, consent, secure deployment, audit retention, operational monitoring and recovery requirements need further design and independent validation.
- Some software capabilities are installed or historically verified only. Environment changes require scoped rechecks. A complete local inference/MCP chain was blocked in the recorded advanced run.
- Backtests and successful engineering tests do not demonstrate investment returns. Unattended real-money operation is outside the verified scope.

## Future development

Potential next steps include better dependency reasoning, richer financial analysis, more realistic research models, explainable reports and explicitly authorized provider integrations. These are proposals, not delivered capabilities. See [ROADMAP.md](ROADMAP.md).

## For Future AI Engineering Agents

This repository preserves engineering knowledge to help future Codex instances understand prior work and continue from available implementation sources. It is primarily documentation, not a complete distribution of the platform. Cloning it does not supply the original Windows workspace, installed tools or private evidence.

- Read [AGENTS.md](AGENTS.md) for persistent repository instructions.
- Follow the [continuation guide](CONTINUATION-GUIDE.md) before proposing implementation work.
- Use the [system inventory](SYSTEM-INVENTORY.md) to locate original components when those sources are available.
- Review [engineering knowledge](ENGINEERING-KNOWLEDGE.md) for tested combinations, failures and repairs.
- Consult the [knowledge index](KNOWLEDGE-INDEX.md) for all documents and the original evidence sources.

Historical results guide a new investigation; they do not prove that another machine has the same capabilities. Continuing from existing source and reconstructing a system from descriptions are different projects.

## Evidence and publication scope

This narrative was prepared from the existing GENESIS-1 controller documentation, GENESIS-2 final engineering report, GENESIS-3 registry report, GENESIS-3.1 capability and advanced intelligence reports, and GENESIS-4 Financial Control report. Those working documents contain machine-specific evidence and are retained privately rather than copied here.

This repository is a documentation foundation for future development. It contains no platform implementation, credentials, private account identifiers, local configuration or financial execution commands.
