# Reuse, licensing and provenance policy

This document states the **policy**. It does **not** choose the project's licence — that
is a user decision, tracked as **OQ-01**.

## The project's licensing goal

CAELITEX is **public** and should remain compatible with **broad reuse, including
possible commercial use**.

> **The repository currently has no `LICENSE` file, and a public repository with no
> licence is *all rights reserved*.** That is the opposite of the stated goal, so it
> wants resolving soon rather than eventually.

### The choice, stated neutrally

| | **MIT** | **Apache-2.0** |
|---|---|---|
| Length / simplicity | Very short; easy to read and to comply with | Substantially longer |
| Patent grant | **No explicit grant** | **Explicit patent grant**, plus patent-retaliation termination |
| Attribution mechanism | Copyright notice only | Copyright notice **plus `NOTICE` file handling**, which gives third-party attributions a defined home |
| Commercial use | Permitted | Permitted |
| Absorbing MIT/BSD-licensed code | Compatible | Compatible |
| Contributions from others | No explicit contribution term | §5 addresses inbound contributions |

The relevant consideration for *this* project is that it **intends to absorb
permissively licensed third-party machinery**, which is the case Apache-2.0's `NOTICE`
mechanism and explicit patent grant were designed for — at the cost of more text and a
slightly higher compliance burden on downstream users than MIT's. **This is a
recommendation of the trade-off to consider, not a decision.**

## Three different licensing questions, routinely confused

1. **Software licensing** — the terms on the code.
2. **Astronomical / data licensing** — the terms on catalogues, surveys and derived data
   products.
3. **Names, content and other IP rights** — project names, trademarks, published figures,
   documentation text.

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
