# AGENT.md — caelitex

Repository identity, boundaries, and safe-participation rules. Read
[`README.md`](README.md) and [`OPEN-QUESTIONS.md`](OPEN-QUESTIONS.md) first.

## Identity

| | |
|---|---|
| **Purpose** | Exploratory, modular research framework for transforming astronomical relationships into alternative mathematical, machine-readable, navigational, symbolic and visual representations. |
| **Repository type** | Research / experimental. Not a product, not a service, not yet an implementation. |
| **Visibility** | **Public.** Assume anything committed here is world-readable, permanently. |
| **Stage** | **Bootstrap.** Intent recorded; nothing chosen. |

## The one rule that matters at this stage

> **Do not build CAELITEX yet.**

Substantive implementation is **not** authorized by the existence of this repository. A
research and design phase has to be able to evaluate alternatives deliberately, and it
cannot do that if a bootstrap has already picked the winners by accident.

Specifically, do **not** introduce a language, package architecture, canonical data
model, module interface, transform API, database, catalogue, visualization stack, glyph
algorithm, ML framework, navigation algorithm, mathematical invariant, dependency, or
code directory layout **as a side effect of some other change**. Each of those is an
entry in [`OPEN-QUESTIONS.md`](OPEN-QUESTIONS.md).

**Do not create speculative implementation skeletons to make the repository look
populated.** An empty directory tree with placeholder modules is a decision wearing a
disguise.

## How to add something

1. If it resolves an open question, **record the decision** in
   [`OPEN-QUESTIONS.md`](OPEN-QUESTIONS.md) — the reasoning and the alternatives
   rejected — in the same change.
2. If it would force a choice the project is not ready to make, prefer **deferral** or
   the **least-opinionated reversible** option, and add an open-question entry saying
   so.
3. Speculative and incomplete material goes in [`develop/`](develop/), which is
   explicitly allowed to be wrong. Everything **outside** `develop/` should serve a
   stable purpose and be explainable from `README.md`.

## High-risk operations

| Operation | Why it is high-risk here |
|---|---|
| Adding a dependency | Sets the stack (OQ-22) **and** drags in an inbound licence that has to be reviewed against Apache-2.0 and recorded. |
| Changing the project's licence | Apache-2.0, ruled by Geoff 2026-09-27 (OQ-01, resolved). **A user decision, not an agent's** — and so is relicensing. |
| Committing catalogue data | Software licensing, data licensing and naming/content rights are three different questions. See [`docs/reuse-and-licensing-policy.md`](docs/reuse-and-licensing-policy.md). |
| Reporting a pattern as a finding | Novel patterns are **candidate relationships requiring validation**, not discoveries because they look interesting. See [`docs/scientific-discipline.md`](docs/scientific-discipline.md). |
| Hand-writing `AGENTS.md` | Deliberately absent — OQ-35. The fleet's pointer is generated and this repo is ineligible because it is public. |

## Ecosystem position

Whether `caelitex` is a curated member of the Symniqs ecosystem is **unresolved**
(OQ-02) and is recorded there rather than assumed here. Shared cross-agent coordination,
if any, is owned by `metaOps`; this repository owns only its own implementation truth.
