# Prior art and reuse leads

> **Nothing on this page is an approved dependency.** These are **leads to investigate**.
> No dependency has been added to this repository, and adding one is a high-risk
> operation (**OQ-22**, [`../AGENT.md`](../AGENT.md)).

CAELITEX should **aggressively investigate prior art rather than recreating solved
machinery**. Several of the sub-problems here are decades old and have mature solutions.

## Fields to investigate

- spacecraft **star trackers** and *lost-in-space* attitude determination
- **geometric hashing**
- astronomical **coordinate and reference systems**
- **Gaia** and other catalogue tooling
- **pulsar timing / XNAV** navigation
- **astrodynamics**
- **clustering in stellar phase space**
- **stellar-stream detection**
- **anomaly detection**
- **graph and spectral methods**
- **dimensionality reduction**
- **uncertainty propagation**
- **astronomical visualization**

The lost-in-space problem in star-tracker literature is, in substance, a version of this
project's identity question with a solved engineering answer under specific assumptions.
Understanding *which assumptions* is more valuable than reimplementing the algorithm.

## Named leads

| Lead | Why it is noted | Status |
|---|---|---|
| **Astropy** / **astroquery** | Established Python astronomy and catalogue-query tooling. Noted as potentially relevant. | **lead — not a dependency.** Noting it does not choose Python (**OQ-10**). |
| **Sidereon** | Identified as one potentially useful **MIT-licensed** project for later examination. | **lead — not a dependency, not examined yet.** |
| Permissively licensed star-identification and astrodynamics projects generally | The class most likely to contain directly reusable machinery. | **leads.** |

**Before any of these is adopted**, the per-component record in
[`reuse-and-licensing-policy.md`](reuse-and-licensing-policy.md) has to be filled in —
including the exact revision, the licence, the commercial-use implications, and the
alternatives considered.

Licence facts stated here are **recorded claims, not verified findings**. Verify the
licence at the exact revision at adoption time; a project's licence can change and its
dependencies may not match its own terms.
