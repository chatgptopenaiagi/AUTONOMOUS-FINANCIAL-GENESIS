# Continuation guide

A new Codex instance can use this repository to recover project context. It must discover what source code and tools are actually available before attempting implementation.

## Read and orient

1. Read [README.md](README.md) for identity, scope and boundaries.
2. Read [AGENTS.md](AGENTS.md) for persistent repository instructions.
3. Inspect [ARCHITECTURE.md](ARCHITECTURE.md) for component responsibilities.
4. Read [SYSTEM-INVENTORY.md](SYSTEM-INVENTORY.md) for historical implementation locations and dependencies.
5. Review [ENGINEERING-KNOWLEDGE.md](ENGINEERING-KNOWLEDGE.md) for previous working approaches and repairs.
6. Review [ROADMAP.md](ROADMAP.md) to distinguish proposed work from delivered behavior.
7. Identify the actual local operating system, installed tools and relevant accessible environments using bounded, read-only inspection.
8. Determine whether the original implementation repositories and their evidence are accessible. Inspect their own instructions and current repository state.
9. Reuse verified work where available, checking only the freshness and compatibility needed for the requested change.
10. Continue the user's specific engineering objective with a small implementation and appropriate verification; preserve unrelated work and record the outcome.

The [knowledge index](KNOWLEDGE-INDEX.md) connects the documents and identifies private original evidence sources. Do not treat inaccessible reports as publicly verifiable artifacts.

## If implementation sources are available

Locate the relevant component from the inventory, read its existing code and manifests, and inspect prior test results before editing. Preserve isolated environments and upstream repositories. Establish a scoped baseline when necessary, then verify affected behavior after the change. Read historical commands as evidence, not automatic execution instructions.

Check that versions, executable paths, operating system and interfaces still match the recorded workflow. Prefer the existing compatible environment over a redundant installation. A historical pass does not override a newer failure.

## If only this documentation repository is available

You can improve documentation, compare designs, identify missing requirements and prepare technical proposals. You cannot run the original application or reproduce its complete state from these Markdown files and summary JSON.

Request or locate the required source through authorized access before claiming to continue implementation. Reconstructing missing software from descriptions would require a separately agreed scope, dependencies, tests and source/licensing review. Do not describe reconstruction as reuse of the original tested platform.

## Keep financial scope explicit

The hub's recorded providers and money are simulated. GENESIS-1's broker-demo evidence is separate. Do not start services, connect accounts, execute orders or initiate payments merely to validate this documentation. Any later operational task needs its own authorization and safeguards.
