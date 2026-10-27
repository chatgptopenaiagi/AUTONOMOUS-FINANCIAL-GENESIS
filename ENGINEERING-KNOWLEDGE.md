# Reusable engineering knowledge

These lessons summarize local engineering evidence from 26–27 October 2026. They are historical results, not a verification of the computer reading this repository. Original source reports are identified below and catalogued in [KNOWLEDGE-INDEX.md](KNOWLEDGE-INDEX.md).

## Approaches that worked

- Inspect installed tools, executable paths, runtime versions and existing evidence before proposing dependencies. Reuse the smallest complete working tool combination.
- Keep acquired source, installed dependencies, builds, launches and functional checks as separate states. GENESIS-2 retained ten independent upstream repositories and project environments; three projects still had partial optional functionality after successful local checks.
- Test a narrow integration before describing a larger architecture as functional. Working individual tools do not establish a working end-to-end application.
- Retain commands, artifact identity, environment bindings, results and limitations. Newer failures affect current selection; successful repairs restore only the scope actually reverified.
- Record financial intent before provider effects. Preserve transaction identity, distinguish payload conflicts from retries and reconcile unknown outcomes without automatic resend.

## Verified interoperability discoveries

| Combination | Recorded result | Boundary for reuse |
|---|---|---|
| MSVC + CMake/Ninja + Python/NumPy | A synthetic native DLL built, loaded through `ctypes` and returned 42 plus the expected matrix result. | Match compiler, architecture, DLL artifact and interpreter; this was not a complete application build. |
| Python + NumPy + SciPy + Matplotlib | Numerical assertions and a noninteractive PNG passed. | Recheck numerical imports and the plotting backend in the actual environment. |
| Python + PyQt6 + SQLite | Offscreen model/UI and synthetic database interaction passed. | Qt stays bound to its verified Anaconda runtime. |
| Python + SQL Server + Excel | A read-only constant query returned 42; an owned Excel COM workbook calculated 84 and saved XLSX. | Windows authentication, SQL service availability and Excel COM were specific prerequisites. |
| Python + PyTorch + bundled CUDA | A small GPU matrix multiplication passed. | cuDNN was unavailable; training, convolution, inference and WSL were not established. |
| TradingGym + NumPy + GNU Octave | Synthetic research calculations matched an independent numerical comparison. | No broker operation or profitability claim. |
| Existing Jesse Python environment + Financial Control Hub | FastAPI, MCP and real loopback requests passed without changing packages. | Reuse requires the original source and a compatible environment; the environment is not distributed here. |

The advanced report records six newly executed cross-tool combinations. Android build evidence was reused historically. A separate local inference/MCP chain remained blocked because its Ollama endpoint was unavailable; the successfully tested financial-hub MCP interface is a different integration.

## Historical failures, repairs and prevention

These are reported diagnoses and checks, not new investigations performed for this documentation.

| Failure | Reported cause or condition | Repair and verification | Future prevention |
|---|---|---|---|
| Windows SQLite file cleanup/ownership failure | Confirmed: an owned SQLite handle remained open. | Explicit connection closure; advanced Scenario I exercised close, rename and delete on an owned temporary database. The hub also repaired backup/export connection ownership. | Close owned handles before cleanup; avoid assuming a connection context releases the handle. |
| Maxima batch invocation failure | Confirmed cmd.exe quoting defect in the adapter. | Reused the verified batch adapter with bounded, validated paths; differentiation succeeded. | Preserve validated argument handling; do not substitute untested shell interpolation. |
| ta4j validation with JDK 27 | The acquisition report records toolchain incompatibility; it does not establish that all newer JDKs fail. | Selected compatible JDK 25; the recorded full validation passed, including 11,290 test cases. | Match the project's supported build toolchain rather than defaulting to the newest installed runtime. |
| Native-build acceptance Scenario D initially failed | A source/artifact-path defect in the test harness, not a compiler defect. | Corrected the harness and reused successful prior probes on the acceptance retry. | Check evidence and artifact identity before blaming or replacing the installed compiler. |

GENESIS-4 also reports fixes for overflow protection, reserved ledger identities, replay/recovery transitions, underfunded closes, child-process cleanup and failed-payment controls. Its initial combined run had one failure and two teardown errors; the final 74-test hub run passed. The report does not supply a detailed causal diagnosis for every item, so this summary does not invent one.

## Dependency compatibility lessons

An explicit `>=3.12,<3.14` requirement excludes Python 3.14. Finding Python 3.12 does not prove that a package installed elsewhere is available there. Compare interpreter, package versions, native libraries, architecture and interfaces together. Unsupported requirement syntax and missing evidence remain unknown.

A framework's bundled CUDA runtime is distinct from the standalone CUDA compiler. A library file's presence does not prove ABI or loader compatibility. Windows and WSL evidence stays separate. Recorded database service status is dated evidence, not a current connection check.

## Regression and verification strategy

The original workspace separates scoped unit/orchestration tests from local integration checks, synthetic acceptance, historical backtests and broker-confirmed demo evidence. Active tests exclude retired components. GENESIS-2 checks preserve each upstream project's scope instead of treating a launch as complete validation.

Recorded GENESIS-3.1 acceptance ran 131 scoped tests and ten scenarios. GENESIS-4 recorded 74 hub tests and 305 active workspace regressions in a separate run, plus API, browser, MCP and SQL checks. These counts have different scopes and must not be added together as a new suite. Financial hub acceptance used synthetic effects; SQL adapter checks used temporary tables and rollback.

This documentation change needs only link, consistency, JSON and privacy checks. Future source changes should run the affected existing tests first, with wider regressions when the change or evidence warrants them. Consult the source project's instructions before running commands: some acceptance scripts create synthetic state or launch services.

## Reducing redundant work

Start from the [system inventory](SYSTEM-INVENTORY.md), locate actual source and inspect its current state. Retrieve a matching workflow, verify its prerequisites and rerun only the checks needed for the requested change. Preserve original failures and evidence dates. Avoid changing working dependencies merely to remove non-blocking warnings.

The advanced report measured the same numerical-routing query on a frozen graph with three warmups and 50 alternating old/new pairs: median 10.1314 ms before and 0.3299 ms after indexed lookup changes, with semantic parity. This is a narrow routing measurement, not proof of general application speed or financial benefit.

## Original evidence

- `REPORTS/GENESIS-2-FINAL-REPORT.md`: acquisition/installation summaries and the ta4j entry.
- `REPORTS/GENESIS-3.1-ADVANCED-INTELLIGENCE.md`: sections 3–8 and 11, covering scope, dependencies, interoperability, causal memory, acceptance and performance.
- `REPORTS/GENESIS-4-FINANCIAL-CONTROL.md`: Implementation and reuse; Accounting, state and recovery; Database results; Executed tests.

These paths refer to the original workspace, not files included in this public repository. See [CONTINUATION-GUIDE.md](CONTINUATION-GUIDE.md) before attempting continuation.
