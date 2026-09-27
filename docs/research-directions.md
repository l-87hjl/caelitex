# The four research directions

**These four are co-equal. None is privileged, and the numbering is not a ranking.**
CAELITEX must support all of them without assuming that any one becomes the principal
purpose. Candidate approaches listed below are **candidates** — nothing here is chosen.

---

## 1. Astronomical identity

Observer-independent, or appropriately invariant, representations of astronomical
structures.

Candidate approaches include, but are not limited to: three-dimensional geometric
relationships; pairwise-distance structures; normalized distance matrices; graph
representations; spectral and eigenvalue representations; angular relationships;
higher-dimensional geometric invariants; other mathematical fingerprints.

**The invariance properties are part of the representation, not a side effect.** For any
candidate representation, the following must be **explicit declared properties** rather
than accidental implementation behaviour:

- translation
- rotation
- reflection
- scale
- object ordering
- measurement uncertainty
- temporal evolution

A representation whose behaviour under one of these is unknown is not yet characterized.

---

## 2. Localization and navigation

Whether astronomical observations can determine an observer's **position**,
**orientation**, **distance**, **epoch / time relationship**, and relationship to
identified references.

**Earth is not an unavoidable origin, and the framework must not assume it is.** In
principle, an observer arriving at an unknown location should be able to identify
references, determine its own relationship to them, and reconstruct another catalogued
location — **including Earth** — *without the outbound journey record*.

Reference classes may extend well beyond ordinary stars: stellar groups, pulsars,
globular clusters, galaxies, quasars, and others. **Different reference classes may
solve different parts of the problem**, and the framework should not force one class to
carry all of it.

---

## 3. Representation

Multiple transformations of the same underlying information, including: invariant
mathematical signatures; matrices; graphs; embeddings; machine-readable identifiers;
statistical representations; human-readable visualizations; symbolic or glyph
representations.

One experimental direction is **deterministic glyph generation** — turning intrinsic
relationships into frequency-, curve-, or graph-like visual forms.

> **The glyph is not the underlying identity.** It is one rendering of it. Representation
> must remain separable from the source data and from the mathematical models.

---

## 4. Discovery

Whether transforming astronomical data into alternative mathematical spaces exposes
relationships that are hard to see conventionally. Questions include:

- Do particular invariant geometries recur?
- Do mathematical or glyph families correspond to independent physical properties?
- Can geometry predict age, temperature, mass, metallicity, spectral class, motion, or
  association membership?
- What correlates unexpectedly — and what conspicuously does **not**?
- Are recurring structures astrophysical, statistical, observational, or **artifacts of
  the transformation**?
- Can unusual structures identify interesting targets?
- Can the process be **inverted** — given a signature, which real structures match?

> **A novel pattern is a candidate relationship requiring validation. It is not a
> discovery because it looks interesting.** The controls this demands are in
> [`scientific-discipline.md`](scientific-discipline.md), and they are not optional.

---

## Scale and grouping are open variables

**Do not equate an astronomical "structure" with a traditional Earth constellation.**
Grouping strategies may include historical constellation or asterism membership;
nearest-N neighbours; a fixed physical radius; a fixed angular radius; common motion;
gravitational or physical association; algorithmically discovered groups; and
random or control groups.

Investigate multiple object counts and multiple physical scales rather than assuming one
correct scale. Traditional constellations may be useful **initial demonstrations because
humans recognize them** — not because they are physically privileged.

## Time

Reference structures evolve. Depending on the problem, this may require proper motion,
orbital motion, stellar evolution, galactic motion, reference epoch, and
light-travel / lookback time.

A useful reference may therefore have a measurable **recognition horizon in both space
and time**: how far away, and how far forward or backward in time, its identity remains
recoverable. Tracked as **OQ-40**.

## An information-theoretic branch

One possible branch: **how much information is actually required** to specify a location
to a desired resolution. This makes it possible to compare the information supplied by
stellar geometry, pulsar timing, angular measurements, spectra, parallax, velocities,
extragalactic reference directions, and combinations of these.

**Do not assume more measurements beat fewer.** The question is which measurements
reduce uncertainty most. Tracked as **OQ-41**.
