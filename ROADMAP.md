# Roadmap

These are future development ideas. They extend the existing engineering platform and simulated Financial Control Hub; they are not promises of delivered functionality or financial performance. No dates are committed.

## 1. Deeper autonomous engineering

- Improve requirement decomposition and comparison of small, complete tool combinations.
- Expand reusable workflows with exact environment bindings, proof scope and recovery steps.
- Make freshness checks and failed-probe handling more precise as software changes.

Success would mean a new task can reuse a suitable verified workflow, explain remaining uncertainty and avoid a known dependency failure without installing redundant tools.

## 2. Improved financial intelligence

- Add clearer cash-flow, exposure, reconciliation and exception analysis.
- Explain financial results through ledger entries and provider confirmations.
- Keep recommendations, operator approvals and execution authority explicit.

Validate against known synthetic cases before connecting any external provider.

## 3. More sophisticated trading research

- Compare strategies across independently maintained research engines.
- Add out-of-sample evaluation, reproducible datasets and robustness checks.
- Model fees, slippage, financing, liquidity and execution uncertainty more realistically.

Keep synthetic simulation, historical backtesting, broker-demo execution and any future real-money operation separately labeled. Research success must not be presented as proof of future returns.

## 4. Better mathematical modelling

- Reuse verified Python, GNU Octave and Maxima workflows where appropriate.
- Develop uncertainty analysis, sensitivity tests and numerical validation.
- Use native or GPU implementations only when measured workloads justify the added complexity.

Compare results with reference calculations and record assumptions, precision and limitations.

## 5. Intelligent financial reporting

- Produce readable explanations of account changes, fees, reconciliations and exceptions.
- Link report statements to accounting evidence and distinguish observations from forecasts.
- Improve exportable summaries and dashboards with currency-aware reporting.

Reports should reproduce ledger totals and expose unresolved differences rather than hide them.

## 6. Future financial-provider integrations

- Design explicitly authorized bank, payment and broker adapters around the existing provider contract.
- Begin with provider sandboxes and verify authentication, consent, rate limits, webhooks and duplicate handling.
- Exercise timeout, partial confirmation, restart and manual-resolution scenarios before broader use.
- Evaluate dedicated SQL Server snapshot deployment separately from any decision to replace the operational SQLite ledger.

Real-provider work requires owner authorization and production controls appropriate to the intended use. No real connector is claimed as implemented by this roadmap.

## 7. Continued software capability learning

- Retain causal explanations of failures, repairs and successful rechecks.
- Refresh only affected graph relationships after inventory changes.
- Improve workflow retrieval while preserving historical evidence and incompatible environment boundaries.
- Measure routing latency, selection correctness and actual reuse under comparable conditions.

The guiding principle remains: discover what already works, select the smallest suitable implementation, verify the result and preserve the evidence for the next task.

## Continuing from this roadmap

For each proposed improvement, first identify an accessible existing component through the [system inventory](SYSTEM-INVENTORY.md) and check the [engineering lessons](ENGINEERING-KNOWLEDGE.md). Define the smallest useful change, its dependencies and a bounded acceptance check before implementation.

If the original source is unavailable, follow the [continuation guide](CONTINUATION-GUIDE.md) and make the missing access explicit. A documentation proposal does not mean the feature has been built, deployed or independently verified.
