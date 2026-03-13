# Constant Extraction Spec (PAD)

This file defines the theorem-constant extraction contract for the p-adic correspondence super-repo.

## Objective

1. extract raw constants from explicit component inputs and formulas,
2. normalize by declared references,
3. promote into `artifacts/constants_registry.json` and `artifacts/stitch_constants.json`.

## Inputs

- `artifacts/constants_extraction_inputs.json`

## Outputs

- `artifacts/constants_extracted.json`
- `artifacts/constants_registry.json`
- `artifacts/stitch_constants.json`
- `artifacts/promotion_report.json`

## Super-Repo Interpretation

The constants do not certify one primitive p-adic correspondence case. They certify the load-bearing parts of the admissible p-adic correspondence lattice:

- projected p-adic correspondence coercivity,
- local matching capture,
- compactness of packet towers,
- rigidity against nonfunctorial bad limits,
- endpoint p-adic correspondence to predicted target packets,
- strict coherence on the determining class.

## Formula Set

- `kappa_padic_raw = c_padic_raw * packet_density_raw - e_padic_raw`
- `sigma_matching_raw = matching_floor_raw - stabilization_loss_raw - restart_loss_raw`
- `kappa_compact_raw = 1.0 / (1.0 + delta_comp_sup_raw)`
- `rho_rigidity_raw = rho_rigidity_raw`
- `packet_padic_raw = c_packet_raw * padic_gain_raw - e_packet_raw`
- `eps_coh_raw = eps_coh_raw`
- `sigma_star_can_raw = sigma_star_can_raw`

## Validations

- positivity required for: `kappa_padic`, `sigma_matching`, `kappa_compact`, `rho_rigidity`, `packet_padic`, `sigma_star_can`
- nonnegative required for: `eps_coh`
- strict-zero required for: `eps_coh` in strict mode

## Execution

`repro/run_repro.sh` runs:

1. `scripts/extract_constants.py`
2. `scripts/promote_constants.py`
3. `scripts/pad_closure_guard.py`
