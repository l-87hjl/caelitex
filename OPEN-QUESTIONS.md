# Open questions — the unresolved-decision register

This file exists so that unresolved decisions stay **visible** rather than being
settled silently by the first person or agent who needs an answer. Every entry is a
decision that has **not** been made.

**Rules for this file.** Do not resolve an entry by acting; resolve it by recording the
decision, its reasoning, and the alternatives rejected — then move it to the
*Resolved* section with a date. An entry marked *user decision* is not the framework's
to settle. Adding an entry is cheap and is preferred over quietly assuming an answer.

Status values: `open`, `user decision`, `deferred by design`.

---

## Blocking or near-term

| ID | Question | Status | Notes |
|---|---|---|---|
| **OQ-01** | **Which licence?** | **user decision** | A public repo with **no** licence is *all rights reserved*, which contradicts the broad-reuse goal. The realistic candidates are **MIT** (shortest, most permissive, no explicit patent grant, no `NOTICE` mechanism) and **Apache-2.0** (explicit patent grant, `NOTICE` handling, attribution machinery that suits a project intending to absorb third-party permissively licensed machinery, but more text). Both are commercial-use compatible and both are compatible with absorbing MIT/BSD code. See [`docs/reuse-and-licensing-policy.md`](docs/reuse-and-licensing-policy.md). **Not to be chosen by an agent.** |
| **OQ-02** | Should CAELITEX be registered as a curated member of the Symniqs ecosystem (`metaOps/ecosystem-registry.yaml`), or recorded in `excluded_from_ecosystem`? | open | Membership is editorial judgement and the registry is governance-gated (PR from every surface). Absence is ambiguous either way, so *some* record is wanted. Also affects whether `metaOps/repos/caelitex/` is scaffolded. |

## Deliberately deferred — architecture and implementation

None of the following has been chosen. **Each entry is a constraint on later work, not
a backlog item to clear quickly.**

| ID | Question | Status |
|---|---|---|
| **OQ-10** | Programming language(s) and runtime | deferred by design |
| **OQ-11** | Package / module architecture, and therefore the code directory layout | deferred by design |
| **OQ-12** | Data model(s). **No mandatory canonical schema is to be established** — see [`docs/data-and-provenance.md`](docs/data-and-provenance.md) | deferred by design |
| **OQ-13** | Transform interface / module composition API | deferred by design |
| **OQ-14** | Storage or database technology, if any | deferred by design |
| **OQ-15** | Which astronomical catalogue(s), and at what epoch | deferred by design |
| **OQ-16** | Visualization technology | deferred by design |
| **OQ-17** | Glyph generation algorithm — *and whether glyphs are pursued at all* | deferred by design |
| **OQ-18** | Mathematical invariant(s) to investigate first, and how each handles translation, rotation, reflection, scale, ordering, uncertainty and time as **explicit declared properties** | deferred by design |
| **OQ-19** | Navigation / localization model, and which reference classes (ordinary stars, stellar groups, pulsars, globular clusters, galaxies, quasars, others) suit which sub-problem | deferred by design |
| **OQ-20** | ML / statistical framework, if any | deferred by design |
| **OQ-21** | Grouping strategy and physical/angular scale. Traditional constellations may be useful *demonstrations* because humans recognize them, **not** because they are physically privileged | deferred by design |
| **OQ-22** | Dependency stack. **No dependency has been added.** Prior-art items in [`docs/prior-art.md`](docs/prior-art.md) are leads, not approved dependencies | deferred by design |

## Deferred repository scaffolding

These are ordinary repository conventions that were **not** created because creating
them would have forced a deferred decision above.

| ID | Item | Why it is absent |
|---|---|---|
| **OQ-30** | `docs/ARCHITECTURE.md` | Would require committing to an architecture (OQ-11, OQ-13). The composable-machine sketch in `README.md` is a philosophy, not an architecture. |
| **OQ-31** | CI workflow (`.github/workflows/`) | Every useful workflow presupposes a language and a test runner (OQ-10). |
| **OQ-32** | Package manifest (`pyproject.toml`, `package.json`, …) | Same: presupposes OQ-10. |
| **OQ-33** | Language-specific `.gitignore` entries | The committed `.gitignore` covers OS and editor noise only. Language sections are added when OQ-10 is answered. |
| **OQ-34** | `AGENT_OPERATIONS.md` | The portable standard asks for an initialization / inspection / planning / verification procedure. There is no build, no test and no runbook to describe yet, so the file would be fiction. Add it with the first real procedure. |
| **OQ-35** | `AGENTS.md` | **Not hand-written on purpose.** The fleet's `AGENTS.md` is generated and deploys only into a **private, non-forked** remote; `caelitex` is public, so it is ineligible and the generator reports `public`. A hand-written substitute would be exactly the stale duplicate that rule exists to prevent. |

## Open research framing questions

| ID | Question | Status |
|---|---|---|
| **OQ-40** | What is a structure's **recognition horizon** — how far in space, and how far forward or backward in time, does its identity remain recoverable? | open |
| **OQ-41** | How much information is actually required to specify a location to a desired resolution, and which measurements reduce uncertainty most? **Do not assume more measurements beat better-chosen ones.** | open |
| **OQ-42** | Which recurring structures are astrophysical, which statistical, which observational, and which artifacts of the transformation itself? | open |
| **OQ-43** | Can the pipeline be inverted — given a signature, which real structures match? | open |
| **OQ-44** | What role, if any, does **"Caeliform"** eventually take as a technical term? Deliberately unfixed. | deferred by design |

## Resolved

*None yet. Entries move here with a date, the decision, and the alternatives rejected.*
