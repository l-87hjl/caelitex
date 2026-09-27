# CAELITEX

**CAELITEX is an open, modular research framework for transforming astronomical
relationships into alternative mathematical, machine-readable, navigational, and
human-readable representations, with applications in astronomical identification,
localization, visualization, and discovery.**

> **Status: bootstrap.** This repository currently contains intent, scope, and an
> explicit register of unresolved decisions — and nothing else. **No language, data
> model, module interface, transform, catalogue, algorithm, or dependency has been
> chosen**, deliberately. See [`OPEN-QUESTIONS.md`](OPEN-QUESTIONS.md) and
> [`AGENT.md`](AGENT.md) before adding anything.

## The originating problem

Familiar constellations are **observer-dependent projections**. A pattern recognizable
from Earth may look entirely different from elsewhere, because its stars occupy
different positions in three-dimensional space. The initiating question was:

> Can a collection of astronomical objects be represented by **intrinsic
> relationships** that remain identifiable despite changes in observer position,
> orientation, ordering, or other irrelevant transformations?

That question expanded into a broader framework, which must support several related but
distinct problems **without assuming any one of them becomes the principal purpose**.

## Four research directions — co-equal, none privileged

1. **Astronomical identity** — observer-independent or appropriately invariant
   representations of astronomical structures.
2. **Localization and navigation** — whether observations can determine an observer's
   position, orientation, distance, epoch, and relationship to identified references,
   *without privileging Earth as an unavoidable origin*.
3. **Representation** — many transformations of the same underlying information:
   mathematical, machine-readable, statistical, visual, symbolic.
4. **Discovery** — whether alternative mathematical spaces expose relationships that
   are hard to see conventionally.

Each is described in [`docs/research-directions.md`](docs/research-directions.md).
**They are listed in an order, not a ranking.**

## Composable-machine philosophy

CAELITEX must not become one monolithic algorithm. It is architecturally — *not
cryptographically* — analogous to a configurable rotor machine, or to a loom:

```
astronomical observations / data
  → selectable transforms
    → intermediate representations
      → selectable transforms
        → mathematical / machine / navigational / visual outputs
```

Different valid module selections may produce different representations, or answer
different questions. **The first transform, representation, data model, glyph
algorithm, navigation model or experiment does not define CAELITEX.**

## Name

**"caeli"** (of the heavens, of the sky) + Latin **"texere"** (to weave) — weaving
celestial relationships into alternative representations.

**"Caeliform"** is retained as project vocabulary, **not** a separate repository and
**not** a rigid technical definition. See [`docs/glossary.md`](docs/glossary.md).

## What is here

| Path | What it is |
|---|---|
| [`OPEN-QUESTIONS.md`](OPEN-QUESTIONS.md) | **The unresolved-decision register.** Deliberately at the root, deliberately visible. |
| [`AGENT.md`](AGENT.md) | Repository identity, boundaries, and what is *not* authorized yet. |
| [`docs/`](docs/) | Canonical intent: research directions, data philosophy, scientific discipline, prior art, reuse and licensing policy, glossary. |
| [`develop/`](develop/) | Non-canonical incubation zone. Allowed to be incomplete, speculative, and self-contradictory. |
| [`LICENSE`](LICENSE) | Apache License 2.0, unmodified. |

There is **no** `src/`, no package manifest, no CI workflow and no
`docs/ARCHITECTURE.md`. Their absence is a recorded decision, not an oversight —
see [`OPEN-QUESTIONS.md`](OPEN-QUESTIONS.md).

## Licence

Licensed under the **Apache License, Version 2.0**. See [`LICENSE`](LICENSE) for the full
text.

```
SPDX-License-Identifier: Apache-2.0
Copyright 2026 the CAELITEX authors
```

Ruled by Geoff on 2026-09-27, closing **OQ-01**. Apache-2.0 was chosen over MIT for its
explicit patent grant and its `NOTICE` mechanism, which gives third-party attributions a
defined home in a project that intends to absorb permissively licensed third-party
machinery.

**This settles the licence *this project grants outward*. It settles nothing about what
the project may take in.** Every reused or adapted component still needs the
compatibility review and the per-component record in
[`docs/reuse-and-licensing-policy.md`](docs/reuse-and-licensing-policy.md) — and
software licensing, data licensing, and naming/content rights remain three separate
questions.

There is no `NOTICE` file yet, deliberately: there are no third-party attributions to
carry. See the policy document for when one becomes required.
