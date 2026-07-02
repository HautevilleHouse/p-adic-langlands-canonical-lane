# EG4 Public Note (Rigidity and Endpoint Transfer)

Mature wording: `bad-limit exclusion / endpoint transfer`.

In-paper anchor: `paper/P_ADIC_LANGLANDS_PREPRINT.md` (`PAD_G4`, `PAD_G5`).

## Goal
Separate the rigidity job from the endpoint-transfer job for `proving persistence of admissible p-adic packets across unitary Banach representations, trianguline parameters, and completed-cohomology packets through a multi-lane p-adic correspondence super-architecture`.
The older wording `rigidity and endpoint-transfer` corresponds to bad-limit exclusion plus the bridge into the intended endpoint object.

## Objects

- bad-limit class: candidates extracted by the compactness gate but incompatible with closure.
- rigidity floor: `rho_rigidity`.
- endpoint-transfer lock: `packet_padic`.
- coherence interface: `eps_coh` remains available to the bridge and final margin.

## Closure Criterion

`PAD_G4` closes when `rho_rigidity` excludes bad endpoint alternatives: bad nonfunctorial countermodels are excluded.
`PAD_G5` closes when `packet_padic` transfers the surviving endpoint to the intended target class: rigid limits p-adic correspondence to the predicted automorphic endpoint packets.
Together they feed the strict margin `M_PAD`.

## Lemma Chain and Proof Payload

### Lemma EG4.1 (bad-limit exclusion)
Every extracted bad limit contradicts a declared rigidity constraint or leaves the admissible class.

Payload: check `rho_rigidity` in the registry and certificate surfaces.

### Lemma EG4.2 (endpoint transfer)
The surviving rigid representative is locked to the standard problem-side endpoint by `packet_padic`.

Payload: read this note together with `notes/IDENTIFICATION_BRIDGE.md`.

### Theorem EG4.3 (rigidity/transfer gate closure)
If bad limits are excluded and the endpoint lock is active, then `PAD_G4` and `PAD_G5` deliver the boundary object needed by the final margin.

## Current Instantiation

- rigidity gate: `PAD_G4`
- rigidity artifact key: `rho_rigidity`
- transfer gate: `PAD_G5`
- transfer artifact key: `packet_padic`
- mature equivalent: `bad-limit exclusion / endpoint identification`
- audit surface: `notes/IDENTIFICATION_BRIDGE.md` and `repro/certificate_runtime.json`
