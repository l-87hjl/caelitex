# Data philosophy and provenance

## Preserve the source, not just the subset

**Preserve source information and provenance even when an experiment needs only a
subset.** An experiment that reduces a catalogue to three columns should still be able to
say where those columns came from, at what version, and what was discarded.

## No mandatory canonical schema

> **Do not establish a mandatory canonical schema.**

Properties that may eventually matter include, but are not limited to: position;
distance; velocity and proper motion; radial velocity; uncertainty and covariance; mass
estimates; radius; luminosity; temperature; metallicity; age estimates; spectral
properties; variability; multiplicity; and temporal / reference-epoch information.

That list is a reminder of breadth, **not a schema and not a required field set**. A
schema fixed now would decide which of the four research directions is easy and which is
awkward, which is exactly the decision this project is deferring (**OQ-12**).

## Uncertainty is data, not noise

**The project must remain able to represent uncertainty rather than treating catalogue
measurements as exact truth.** Any representation that silently promotes a measurement
with error bars to an exact value has discarded information that some of the research
questions depend on — notably the invariance-under-uncertainty property in
[`research-directions.md`](research-directions.md) §1 and the information-theoretic
branch (**OQ-41**).

## Time and epoch

Positions are statements about a moment. Reference epoch, proper motion and light-travel
time are properties of the data, so a data representation that cannot carry them cannot
support the temporal questions at all.

## Data licensing is a separate question from software licensing

See [`reuse-and-licensing-policy.md`](reuse-and-licensing-policy.md). Committing
catalogue data into this repository is a high-risk operation and is not authorized by
this document.
