# EG2 Public Note (Capture and Restart)

Canonical wording: `transport / local-to-global transfer`.

In-paper anchor: `paper/P_ADIC_LANGLANDS_PREPRINT.md` (`PAD_G2`).

## Goal
Expand the compressed capture/restart language into the local-to-global transport gate for `proving persistence of admissible p-adic packets across unitary Banach representations, trianguline parameters, and completed-cohomology packets through a multi-lane p-adic correspondence super-architecture`.

## Objects

- transport carrier: the admissible evolution, deformation, or routed lattice declared in the preprint.
- capture floor: `sigma_matching`.
- restart law: the normalization/re-entry rule that keeps corrective steps inside the admissible class.
- carried losses: defect, restart, and normalization losses that must remain explicit.

## Closure Criterion

`PAD_G2` closes when `sigma_matching` survives admissible losses and restart corrections: local matching defect stays above capture floor across admissible p-adic correspondence losses.
This is the transport contribution to `M_PAD`.

## Lemma Chain and Proof Payload

### Lemma EG2.1 (transport accounting)
Every transport step used by the lane is charged to the declared defect ledger instead of being absorbed into prose.

Payload: check that the capture constant `sigma_matching` is present in the constants registry and extraction inputs.

### Lemma EG2.2 (restart preservation)
Restart or normalization preserves the declared admissible class and does not create an untracked remainder.

Payload: inspect the repro script and guard output for the gate tied to `sigma_matching`.

### Theorem EG2.3 (capture gate closure)
If transport accounting and restart preservation hold, then `PAD_G2` carries local control forward without breaking admissibility.

## Current Instantiation

- gate: `PAD_G2`
- artifact key: `sigma_matching`
- canonical equivalent: `transport / local-to-global transfer`
- audit surface: `repro/run_repro.sh` and `repro/certificate_runtime.json`
