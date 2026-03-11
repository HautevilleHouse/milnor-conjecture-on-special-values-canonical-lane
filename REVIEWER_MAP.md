# Reviewer Map

    ## Claim Scope

    - Canonical-lane claim: inside the `manifold_constrained` lane, if the theorem chain in this repository holds and the guard certificate passes, the repository-level closure claim is satisfied.
    - Standard target claim: carried by the in-repo bridge theorems tying the lane to the target statement.

    ## Theorem Dependency Chain

    1. `EG1`: coercive response and active control floor.
    2. `EG2`: capture and admissible continuation.
    3. `EG3`: compactness and no-collapse spacing.
    4. `EG4`: rigidity and transfer.
    5. Identification bridge: strict coherence on the determining class.
    6. Scalar closure: `MSV_G1, MSV_G2, MSV_G3, MSV_G4, MSV_G5, MSV_G6, MSV_GM` all `PASS`.

    Primary files:

    - `paper/MILNOR_CONJECTURE_ON_SPECIAL_VALUES_PREPRINT.md`
    - `notes/EG1_public.md`
    - `notes/EG2_public.md`
    - `notes/EG3_public.md`
    - `notes/EG4_public.md`
    - `notes/IDENTIFICATION_BRIDGE.md`

    ## Closure Gates

    | Gate | Constant | Description |
    |------|----------|-------------|
    | `MSV_G1` | `kappa_polylog` | projected polylogarithmic response has a strict positive floor |
| `MSV_G2` | `sigma_value` | special-value defect stays above capture floor across admissible regulator losses |
| `MSV_G3` | `kappa_compact` | normalized near-failure families are precompact and value windows do not collapse |
| `MSV_G4` | `rho_rigidity` | bad special-value countermodels are excluded |
| `MSV_G5` | `regulator_transfer` | rigid limit transfers to the predicted special-value endpoint class |
| `MSV_G6` | `eps_coh` | strict coherence / identification closure |
| `MSV_GM` | derived | final strict margin |

    ## Falsification Conditions

    - `repro/certificate_runtime.json` has any non-`PASS` gate.
    - `lane.active_lane != "manifold_constrained"`.
    - `all_pass != true`.
    - Any manifest hash mismatch under `repro/repro_manifest.json`.
    - A verified counterexample to any EG theorem statement used in the paper.
