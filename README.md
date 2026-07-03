# p-adic Langlands via p-adic Packet Persistence
## Canonical Lane (defined term): the manifold-constrained local-to-global p-adic correspondence super-architecture (`PAD1-PAD8`)

Canonical Lane super-repo for a flagship umbrella problem in p-adic representation theory, Galois representations, and the Langlands program:
proving persistence of admissible p-adic packets across unitary Banach representations, trianguline parameters, and completed-cohomology packets through a multi-lane p-adic correspondence super-architecture.

## Main Manuscript

- [paper/P_ADIC_LANGLANDS_PREPRINT.md](paper/P_ADIC_LANGLANDS_PREPRINT.md)
- [paper/CANONICAL_ROUTING_INDEX.md](paper/CANONICAL_ROUTING_INDEX.md)

## Super-Repo Role

This repository is not a single primitive p-adic correspondence case. It is the coordinating p-adic correspondence lane for an admissible p-adic correspondence lattice whose native sub-lane families are:

1. unitary Banach representation packages,
2. trianguline and eigenvariety compatibility packages,
3. p-adic Hodge-theoretic comparison packages,
4. locally analytic and completed-cohomology transfer packages,
5. local-global stitching of the declared p-adic packet correspondence.

The runtime surface establishes closure of the declared super-lane, not just one isolated p-adic correspondence example.

## Structure

- `paper/`
  - `P_ADIC_LANGLANDS_PREPRINT.md`
  - `CANONICAL_ROUTING_INDEX.md`
  - `EXTRACTION_SPEC.md`

- `notes/`
  - `EG1_public.md`
  - `EG2_public.md`
  - `EG3_public.md`
  - `EG4_public.md`
  - `IDENTIFICATION_BRIDGE.md`

- `repro/`
  - `REPRO_PACK.md`
  - `THIRD_PARTY_RERUN_PROTOCOL.md`
  - `run_repro.sh`
  - `repro_manifest.json`
  - `certificate_baseline.json`

- `scripts/`
  - `pad_closure_guard.py`
  - `extract_constants.py`
  - `promote_constants.py`
  - `update_manifest.py`
  - `release_gate.py`
  - `README.md`

- `artifacts/`
  - `constants_extraction_inputs.json`
  - `constants_extracted.json`
  - `constants_registry.json`
  - `stitch_constants.json`
  - `promotion_report.json`

## Local Reproducibility Command

```bash
bash repro/run_repro.sh
```

This writes `repro/certificate_runtime.json`.

## How To Read This Professionally

1. Super-lane theorem chain first: read `paper/P_ADIC_LANGLANDS_PREPRINT.md`.
2. Transfer-lattice routing second: audit `paper/CANONICAL_ROUTING_INDEX.md` and the note layer.
3. Constants provenance third: audit `paper/EXTRACTION_SPEC.md`, `artifacts/constants_extraction_inputs.json`, `artifacts/constants_extracted.json`, and `artifacts/promotion_report.json`.
4. Pipeline fourth: run `bash repro/run_repro.sh` to audit hashes, provenance, and gates; it is reproducibility infrastructure, not theorem generation.

Release modes:

- `normalized`: `status=normalized_placeholder` allowed when explicitly labeled.
- `fully_extracted`: requires `status=derived_numeric` for all required constants and stitch keys.

Current PAD runner policy:

- `repro/run_repro.sh` extracts, promotes, runs `scripts/pad_closure_guard.py`, updates `repro/repro_manifest.json`, and enforces `fully_extracted` release-gate mode.

## Routing Rule (inclusion discipline)

Every claim-bearing item must be routed through all three layers:

1. main preprint section/appendix,
2. mirror note under `notes/`,
3. artifact key consumed by `scripts/pad_closure_guard.py`.

Routing map: [paper/CANONICAL_ROUTING_INDEX.md](paper/CANONICAL_ROUTING_INDEX.md)

## Citation

- Metadata: [CITATION.cff](CITATION.cff)
- Manuscript target: [paper/P_ADIC_LANGLANDS_PREPRINT.md](paper/P_ADIC_LANGLANDS_PREPRINT.md)

## Authorship

- Program author: **HautevilleHouse**
- Canonical attribution source: [`CITATION.cff`](CITATION.cff)
