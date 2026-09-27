# docs/ — canonical intent

Canonical material: the project's stated intent, scope, and policy. Speculative work
belongs in [`develop/`](../develop/) instead.

| Document | What it fixes, and what it deliberately does not |
|---|---|
| [`research-directions.md`](research-directions.md) | The four co-equal directions. Fixes *that they are co-equal*; fixes no approach. |
| [`data-and-provenance.md`](data-and-provenance.md) | Fixes that provenance and uncertainty are preserved. **Fixes no schema.** |
| [`scientific-discipline.md`](scientific-discipline.md) | Fixes that controls, leakage detection, and permitted/withheld records are required of experiments. Fixes no experiment. |
| [`prior-art.md`](prior-art.md) | Fields and named leads to investigate. **No item here is an approved dependency.** |
| [`reuse-and-licensing-policy.md`](reuse-and-licensing-policy.md) | Fixes the reuse ordering and the record required per reused component. **Does not choose the project's licence** — that is OQ-01. |
| [`glossary.md`](glossary.md) | Fixes vocabulary. Records which terms are deliberately left undefined. |

## What is absent, and why

There is no `ARCHITECTURE.md`. The standard repository shape expects one, and writing it
now would mean choosing an architecture — which is precisely the decision this bootstrap
is preserving. Recorded as **OQ-30** in [`OPEN-QUESTIONS.md`](../OPEN-QUESTIONS.md). The
composable-machine sketch in the root `README.md` is a *philosophy*: it says the pipeline
must be made of interchangeable stages, not what any stage is.
