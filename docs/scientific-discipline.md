# Scientific discipline

Discovery work must guard against **generating artifacts and mistaking them for
astronomical phenomena**. The transformation pipeline is itself a source of structure;
without controls there is no way to tell its structure from the sky's.

## Controls future experiments must be able to run

An experiment framework should support comparison against, at least:

- random stellar groups
- synthetic populations
- randomized positions
- shuffled physical attributes
- randomized velocities
- populations with the density distribution preserved but the relationships altered
- physically simulated comparison populations
- uncertainty propagation
- held-out properties
- leakage detection

This is a list of capabilities the framework must not preclude. It is **not** a
prescribed experimental protocol, and it does not choose a statistics stack.

## Permitted and withheld information — the record that makes a claim meaningful

> An experiment must be able to record **which information a transform was permitted to
> use** and **which properties were withheld**.

This is the load-bearing requirement on this page. A claim that *geometry predicts
temperature* is **meaningless** if temperature, or any proxy for it, leaked into the
representation. Colour indices, spectral class, catalogue selection effects and
distance-dependent completeness are all plausible proxies, and the leak is usually
upstream of the model rather than in it.

So the permitted/withheld record is not documentation added after a result. It is part of
what makes the result a result.

## What a novel pattern is

> **A novel pattern is a candidate relationship requiring validation. It is not a
> discovery because it looks interesting.**

Before a recurring structure is reported as astrophysical, the alternatives have to be
addressed: is it statistical, is it observational (a selection or completeness effect),
or is it an artifact of the transformation itself? Tracked as **OQ-42**.
