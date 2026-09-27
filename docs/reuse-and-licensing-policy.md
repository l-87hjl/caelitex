# Reuse, licensing and provenance policy

This document states the **policy**. The project's **outbound** licence is settled; the
**inbound** question is not, and never will be — it recurs for every component.

## The outbound licence — settled

> **CAELITEX is licensed under the Apache License, Version 2.0.**
> **`SPDX-License-Identifier: Apache-2.0`** · full text in [`../LICENSE`](../LICENSE).
>
> **Ruled by Geoff, 2026-09-27**, closing **OQ-01**.

This is compatible with the stated goal: CAELITEX is public and should remain compatible
with **broad reuse, including commercial use**.

### Why Apache-2.0 rather than MIT

Both permit commercial use and both can absorb MIT/BSD-licensed code. The deciding
considerations were:

| | **MIT** | **Apache-2.0** — chosen |
|---|---|---|
| Length / simplicity | Very short | Substantially longer |
| Patent grant | **No explicit grant** | **Explicit patent grant**, plus patent-retaliation termination |
| Attribution mechanism | Copyright notice only | Copyright notice **plus `NOTICE` file handling** — a defined home for third-party attributions |
| Commercial use | Permitted | Permitted |
| Contributions from others | No explicit term | §5 addresses inbound contributions |

A project that **intends to absorb permissively licensed third-party machinery** is
exactly the case the `NOTICE` mechanism and the explicit patent grant were designed for.
The cost is more text and a slightly higher compliance burden on downstream users.

### What the ruling does *not* settle

**It settles what CAELITEX grants outward. It settles nothing about what CAELITEX may
take in.** Being Apache-2.0 licensed does not make an inbound component compatible, does
not pre-approve a licence class, and does not remove any step below. The reuse order, the
per-component record, and the copyleft review all still apply in full, every time.

### The `LICENSE` file is unmodified, including its appendix

The committed text is the standard Apache-2.0 body verbatim, appendix included. **The
appendix's per-file header boilerplate is a suggestion, and it has deliberately not been
applied** — there are no source files, so applying it would have meant inventing files.
**Guidance for later, not an action now:** when source files do exist, the conventional
practice is a short header naming the copyright holder and pointing at the licence, and
`SPDX-License-Identifier: Apache-2.0` is the compact modern form of it. Decide that
alongside the language choice (**OQ-10**); it is not decided here.

### There is no `NOTICE` file, deliberately

Apache-2.0 §4(d) obliges a redistributor to carry a `NOTICE` **only if the work has
one**. There are currently **no third-party attributions to carry**, so a `NOTICE` now
would be an empty file that nevertheless creates a propagation obligation for everyone
downstream — ritual with a cost and no content.

**Create it at the moment it has something to say:** the first time a component is
adopted whose licence requires attribution — which is the same moment the per-component
record below gets its first entry. Apache-2.0 §4(d) then governs what goes in it.

## Three different licensing questions, routinely confused

1. **Software licensing** — the terms on the code.
2. **Astronomical / data licensing** — the terms on catalogues, surveys and derived data
   products.
3. **Names, content and other IP rights** — project names, trademarks, published figures,
   documentation text.

**The Apache-2.0 ruling answers (1) for CAELITEX's own output, and only that.** It says
nothing about the terms on a catalogue, and nothing about names or content rights —
including Apache-2.0 §6, which grants no trademark permission.

> **Do not assume permissively licensed software makes its source data permissively
> licensed.** An MIT-licensed tool bundling or fetching a restrictively licensed
> catalogue gives you the tool, not the catalogue.

**Copyleft or otherwise restrictive dependencies require explicit review** against this
project's licensing and reuse goals. They are never casually incorporated.

## Preferred reuse order

1. **Existing dependency or API** — use the thing as it ships.
2. **Thin adapter** around it.
3. **Narrow, permissively licensed adaptation**, where justified.
4. **Fork** — only where continuing independent development actually warrants it.

Prefer technically suitable permissively licensed existing machinery over reproducing a
mature solution.

## The record required for every reused or adapted component

For each one, future work must record:

- source repository or project
- **exact revision / version**
- capability reused
- licence, with **SPDX identifier**
- required notices / attribution
- whether it is used as a **dependency**, **wrapped**, **adapted**, **ported**, or
  **merely studied**
- commercial-use implications
- copyleft implications
- maintenance status
- alternatives considered
- **disposition and reasoning**

"Merely studied" is a real and useful category, and recording it prevents a later reader
from assuming code was copied when only an idea was.

## Where these records will live

**Undecided**, because it depends on the eventual repository layout (**OQ-11**). Until
then, record them in [`../develop/`](../develop/) and move them once there is a canonical
home. The fields above are fixed; the file path is not.
