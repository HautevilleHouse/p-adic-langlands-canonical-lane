# Reviewer Map

## Claim Scope

- Canonical-lane claim: inside the `manifold_constrained` p-adic correspondence lattice, if the theorem chain in this repository holds and the guard certificate passes, the repository-level super-lane closure claim is satisfied.
- Standard target claim: admissible `L`-group morphisms in the declared p-adic correspondence lattice produce the predicted automorphic endpoint packets with matching local/global observables.
- External-strengthening rule: any statement beyond the admissible class must retain the explicit remainder carried by the defect/coherence ledgers; see `notes/GEOMETRIC_GALOIS_BRIDGE.md`.

## Super-Lane Families

The manuscript treats the following as routed sub-lane families inside one coordinating super-repo:

1. unitary Banach representation packages,
2. trianguline and eigenvariety compatibility packages,
3. p-adic Hodge-theoretic comparison packages,
4. locally analytic and completed-cohomology transfer packages,
5. local-global stitching of the declared p-adic packet correspondence.

## Theorem Dependency Chain

1. `EG1`: coercive p-adic correspondence response and active floor.
2. `EG2`: local matching capture across the p-adic correspondence lattice.
3. `EG3`: compactness and no-collapse spacing for packet towers.
4. `EG4`: rigidity and endpoint p-adic correspondence.
5. Identification bridge: strict coherence on the determining class.
6. Scalar closure: `PAD_G1, PAD_G2, PAD_G3, PAD_G4, PAD_G5, PAD_G6, PAD_GM` all `PASS`.

Primary files:

- `paper/P_ADIC_LANGLANDS_PREPRINT.md`
- `notes/EG1_public.md`
- `notes/EG2_public.md`
- `notes/EG3_public.md`
- `notes/EG4_public.md`
- `notes/IDENTIFICATION_BRIDGE.md`
- `notes/GEOMETRIC_GALOIS_BRIDGE.md`

## Closure Gates

| Gate | Constant | Description |
|------|----------|-------------|
| `PAD_G1` | `kappa_padic` | projected p-adic correspondence response has a strict positive floor |
| `PAD_G2` | `sigma_matching` | local matching defect stays above capture floor across admissible p-adic correspondence losses |
| `PAD_G3` | `kappa_compact` | normalized near-failure packet towers are precompact |
| `PAD_G4` | `rho_rigidity` | bad nonfunctorial countermodels are excluded |
| `PAD_G5` | `packet_padic` | rigid limits p-adic correspondence to predicted target packets |
| `PAD_G6` | `eps_coh` | strict coherence on the determining class |
| `PAD_GM` | derived | final strict margin |

## Falsification Conditions

- `repro/certificate_runtime.json` has any non-`PASS` gate.
- `lane.active_lane != "manifold_constrained"`.
- `all_pass != true`.
- Any manifest hash mismatch under `repro/repro_manifest.json`.
- A verified counterexample to any routed sub-lane p-adic correspondence theorem used by the super-repo.
