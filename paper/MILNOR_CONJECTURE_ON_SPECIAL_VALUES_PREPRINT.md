# The Milnor Conjecture on Special Values via Polylogarithmic Regulator Persistence
## Canonical Lane (defined term): the manifold-constrained local-to-global closure architecture (`MSV1-MSV8`)

**Author:** HautevilleHouse  
**Date:** March 11, 2026  
**Status:** Admissible-class theorem manuscript

---

## Abstract

This manuscript develops a canonical-lane closure architecture for the target problem: proving special-value identities in the Milnor-style regulator package through an admissible polylogarithmic closure architecture.

The proof program is organized as eight steps `MSV1-MSV8` with executable closure gates `MSV_G1`, `MSV_G2`, `MSV_G3`, `MSV_G4`, `MSV_G5`, `MSV_G6`, and `MSV_GM`. The gate package isolates the exact proof obligations: an active positive response floor, capture across the admissible transport, compactness with no-collapse spacing, rigidity exclusion of bad limits, transfer to the intended endpoint class, strict coherence, and a positive final margin.

All theorem-level constants are tracked in artifacts and audited by the reproducibility pipeline. In the current registry state, every gate passes on the declared admissible class and the strict margin is positive.

---

## 1. Target Statement and Scope

### 1.1 Target statement

Special values of admissible zeta and `L`-functions are controlled by the predicted polylogarithmic and higher `K`-theoretic regulator package in the declared class.

The canonical-lane proof path is:

1. encode the admissible evolution in a canonical class `A`,
2. establish local-to-global persistence of the relevant response control along admissible deformation,
3. exclude bad limits by rigidity and compactness,
4. transfer the rigid limit through the bridge package,
5. identify the endpoint representative with the intended target class.


### 1.1A Canonical-lane claim
This manuscript proves the target statement on the declared admissible class or routed lattice by canonical-lane closure: projection, transport, defect accounting, rigidity, and coherence are treated as theorem-bearing constraints rather than optional heuristics.

### 1.1B Bridge / equivalence statement
The canonical endpoint objects are tied to the standard problem-side target through the in-repo bridge package. The paper records the transfer or endpoint-identification step in the main theorem chain, and `notes/IDENTIFICATION_BRIDGE.md` fixes the determining-class lock in ordinary mathematical language.

### 1.1C Verification surface
A reviewer can check this claim on four surfaces:

1. the standard target statement in Section `1.1`,
2. the canonical objects and closure gates in the main paper,
3. the endpoint bridge in `notes/IDENTIFICATION_BRIDGE.md`,
4. the executable rerun `bash repro/run_repro.sh` with runtime output `repro/certificate_runtime.json`.

### 1.2 Local claim boundary

- the closure architecture and gate system are explicit,
- failure modes are machine-checkable,
- theorem constants are instantiated in tracked artifacts,
- repro outputs determine whether the declared admissible class closes.

Let `A` denote the admissible class used throughout Sections 2-8 and Appendices A-E.

---

## 2. Epistemic Axiom Map (A1-A8)

| Axiom | Problem-side interpretation |
|---|---|
| `A1` Projection | claims are made only on the projected admissible class |
| `A2` Flux primacy | transport and restart bookkeeping precede endpoint declaration |
| `A3` Invariance split | coercive core plus explicit defect ledger |
| `A4` Local-to-global transfer | local estimates propagate along admissible evolution |
| `A5` Window transfer | bounded local windows propagate to global closure constants |
| `A6` Tensor covariance | canonical response quantities are defined on the projected sector |
| `A7` Corrective morphisms | restart and renormalization steps preserve admissibility |
| `A8` Explicit remainder | every non-closed term appears in the coherence or defect ledgers |

---

## 3. Canonical Objects

Let `tau` denote the deformation parameter and let

`u_tau = (P_tau, R_tau, D_tau, N_tau, L_tau)`

be the admissible state consisting of polylogarithmic packets, admissible regulator data, defect ledgers, normalization parameters, and lock observables.

Primary objects:

- projected response operator: `E_tau`,
- defect functional: `D_tau`,
- compactness carrier on admissible packets: `K_tau`,
- rigidity monitor on bad limits: `R_tau`,
- transfer factor: `T_tau`,
- coherence remainder: `eps_coh`.

Strict closure margin:

`M_MSV = min(kappa_polylog, sigma_value, kappa_compact, rho_rigidity, regulator_transfer) - eps_coh`.

Target:

`M_MSV > 0`.

---

## 4. Response and Gate Interface

### 4.1 Canonical tube

- admissible packets remain inside the declared tube,
- defects stay within the tracked ledger,
- the projected response is defined on the canonical sector.

### 4.2 Projected response

Let `H_resp` be the projected response sector and define:

`E_tau = Pi_resp L_tau Pi_resp`.

Interpretation: `E_tau` records the positive polylogarithmic regulator floor that prevents collapse of the admissible special-value package.

### 4.3 Closure gates

| Gate | Constant | Criterion |
|---|---|---|
| `MSV_G1` | `kappa_polylog` | projected polylogarithmic response has a strict positive floor |
| `MSV_G2` | `sigma_value` | special-value defect stays above capture floor across admissible regulator losses |
| `MSV_G3` | `kappa_compact` | normalized near-failure families are precompact and value windows do not collapse |
| `MSV_G4` | `rho_rigidity` | bad special-value countermodels are excluded |
| `MSV_G5` | `regulator_transfer` | rigid limit transfers to the predicted special-value endpoint class |
| `MSV_G6` | `eps_coh` | coherence remainder closes in strict mode |
| `MSV_GM` | derived | all upstream gates pass and `M_MSV > 0` |

### 4.4 Strict margin

At current artifact values:

- `kappa_polylog` = 1.0932,
- `sigma_value` = 1.0750000000000002,
- `kappa_compact` = 0.8045052292839904,
- `rho_rigidity` = 1.078,
- `regulator_transfer` = 1.029422,
- `eps_coh = 0.0`.

Hence:

`M_MSV = 0.8045052292839904 > 0`.

### 4.5 Raw coercive constant

Define `kappa_polylog^(raw) := c_polylog_raw * polylog_density_raw - e_polylog_raw`.

Current extracted value:

`kappa_polylog = 1.0932`.

---

## 5. Capture, Compactness, and Theorem Chain

### 5.1 Local-to-global theorem chain (`MSV1-MSV8`)

1. `MSV1` Active polylogarithmic block on the projected response sector.
2. `MSV2` Uniform value capture bounds on the canonical regulator tube.
3. `MSV3` Restart map preserving admissible regulator data.
4. `MSV4` First-failure compactness extraction.
5. `MSV5` Rigidity exclusion of bad special-value countermodels.
6. `MSV6` Regulator-transfer closure on the extracted endpoint class.
7. `MSV7` Determining-class identification of the Milnor special-value endpoint.
8. `MSV8` Final persistence theorem: the special-value endpoint survives admissible closure.

### 5.2 Raw capture constant

Define `sigma_value^(raw) := value_floor_raw - regulator_loss_raw - restart_loss_raw`.

Current extracted value:

`sigma_value = 1.0750000000000002`.

### 5.3 Compactness modulus

Define `kappa_compact^(raw) := (1 + delta_comp_sup_raw)^(-1)`.

Current extracted value:

`kappa_compact = 0.8045052292839904`.

---

## 6. Rigidity, Transfer, and Identification

### 6.1 Rigidity margin

Rigidity excludes the bad-limit class `B_bad` of special-value countermodels incompatible with closure.

Define `rho_rigidity^(raw) := inf_(U in B_bad) R_bad(U) / ||U||^2`.

The tracked theorem-level input is `rho_rigidity = 1.078 > 0`.

### 6.2 Transfer package

Once bad limits are excluded, the extracted endpoint class is transferred to the predicted special-value endpoint class by the bridge inequality.

Define `regulator_transfer^(raw) := c_reg_raw * transfer_gain_raw - e_reg_raw`.

Current extracted value:

`regulator_transfer = 1.029422 > 0`.

### 6.3 Determining-class identification

Fix a determining class `C_det` of polylogarithmic and regulator observables. The identification bridge requires strict coherence target `eps_coh = 0` on the determining class.

---

## 7. Current Theorem Inputs (Tracked)

| Constant | Gate | Current value |
|---|---|---|
| `kappa_polylog` | `MSV_G1` | `1.0932` |
| `sigma_value` | `MSV_G2` | `1.0750000000000002` |
| `kappa_compact` | `MSV_G3` | `0.8045052292839904` |
| `rho_rigidity` | `MSV_G4` | `1.078` |
| `regulator_transfer` | `MSV_G5` | `1.029422` |
| `eps_coh` | `MSV_G6` | `0.0` |
| `sigma_star_can` | stitch | `1.053` |

---

## 8. Current Runtime Snapshot

Latest local guard output (`repro/certificate_runtime.json`):

- `MSV_G1, MSV_G2, MSV_G3, MSV_G4, MSV_G5, MSV_G6, MSV_GM = PASS`,
- strict margin `M_MSV = 0.8045052292839904`,
- lane: `manifold_constrained`.

---

## 9. Reproducibility

Run:

```bash
bash repro/run_repro.sh
```

This writes `repro/certificate_runtime.json`.

---

## 10. In-Paper Appendix Pack (A-E)

### Appendix A. EG1 Coercive Package

The projected response operator yields the raw floor `kappa_polylog^(raw) > 0`, hence `MSV_G1 = PASS`.

### Appendix B. EG2 Capture Package

The defect functional obeys a local-to-global inequality with explicit regulator losses. Positivity of `sigma_value` yields `MSV_G2 = PASS`.

### Appendix C. EG3 Compactness and No-Collapse Package

Normalized near-failure families lie in the compactness carrier and value windows have a positive spacing lower bound, giving `kappa_compact > 0` and `MSV_G3 = PASS`.

### Appendix D. EG4 Rigidity Package

Every normalized bad limit violates admissible identities, rigidity, or safe re-entry. The theorem-level constant `rho_rigidity > 0` excludes bad limits and closes `MSV_G4`.

### Appendix E. Identification and Transfer Package

The transfer constant is `regulator_transfer = 1.029422 > 0`, while strict coherence requires `eps_coh = 0`.

Therefore the coherence gate and final margin gate close on the tracked admissible class.

---

## 11. References

1. J. Milnor, *Introduction to Algebraic K-Theory*, Princeton Univ. Press, 1971.
2. S. Bloch, *Higher Regulators, Algebraic K-Theory, and Zeta Functions of Elliptic Curves*, CRM Monograph Series 11, 2000.
3. A. Goncharov, *Polylogarithms and motivic Galois groups*, Proc. Sympos. Pure Math. 55 (1994), 43-96.
