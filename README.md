# The Residual Core of the Collatz Problem: A Structural Decomposition

**2026**

Identifies the precise residual structure of the Collatz problem within the renewal framework. The unsolved core is not probabilistic drift — the average Lyapunov exponent is provably negative. The residual is a single question: can one rule out infinite arithmetic memory along a single orbit?

> This repository does not claim a proof of the Collatz conjecture.

---

## Overview

The paper organises all known results into four levels of rigidity and locates the exact boundary of what remains open:

- **Level 0** (Rigid): Renewal system is exact; exact covariance decay and finite total mutual information (2 log 2) are proved
- **Level 1** (Divergence constraints): If an orbit diverges it must violate empirical typicality (Theorems D1-bwd, NGM)
- **Level 2** (Memory rigidity gap): Atypicality implies infinite arithmetic memory — conditional on persistent correlation (Theorem IT2b)
- **Level 3** (Arithmetic obstruction): Individual orbit decorrelation — the parity barrier — remains open

---

## Main Results

### Proved (Rigorous)

| Result | Method | Status |
|--------|--------|--------|
| Level 0: exact covariance Cov_π(k₀, kₙ) = 2·(1/2)^N | Renewal operator | ✓ proved |
| Level 0: total mutual information Σ I_π = 2 log 2 (finite) | Information theory | ✓ proved |
| Theorem D1-bwd: divergent orbit has liminf avg valuation ≤ log₂ 3 | Contrapositive | ✓ proved |
| Theorem NGM: divergent orbit cannot be π-typical | Measure theory | ✓ proved |
| Theorem OE_J: prime-starting iterates equidistributed mod 2^K | Congruence | ✓ proved |

### Conditional

| Result | Condition | Status |
|--------|-----------|--------|
| Theorem IT2b: persistent correlation → infinite memory | Persistent correlation hypothesis | conditional |

---

## Structure

```
§1   What is already rigid (Level 0)              ✓
§2   What divergence must violate (Level 1)       ✓ (Theorems D1-bwd, NGM)
§3   The memory rigidity gap (Level 2)            conditional (Theorem IT2b)
§4   The arithmetic obstruction (Level 3)         open (parity wall)
§5   The residual core — summary table
§6   The residual obstruction
§7   Comparison with prior approaches
§8   Roadmap
```

---

## Open Problems

- **Core question**: Can one rule out infinite arithmetic memory along a single Collatz orbit?
- Level 3: individual orbit parity decorrelation (the parity barrier)
- Removal of the persistent-correlation condition in Theorem IT2b

---

## Repository Structure

```
collatz-residual-core/
├── README.md
├── paper/
│   └── residual_core_structural_decomposition.pdf
└── LICENSE
```

---

## Related Work

This paper is part of a series on Collatz dynamics:

- [collatz-act1](https://github.com/KAMANOI/collatz-act1) — Foundational paper: prime survival dynamics and Chen-type theorem (v11)
- [collatz-renewal-structure](https://github.com/KAMANOI/collatz-renewal-structure) — Paper A: exact operator structure and finite information memory
- [collatz-finite-mixing-geometry](https://github.com/KAMANOI/collatz-finite-mixing-geometry) — Paper B: finite-level mixing geometry
- [collatz-spectral-amplification](https://github.com/KAMANOI/collatz-spectral-amplification) — Paper C: spectral amplification
- [collatz-scale-coherence](https://github.com/KAMANOI/collatz-scale-coherence) — Paper D: scale-coherence rigidity
- [collatz-valuation-renewal](https://github.com/KAMANOI/collatz-valuation-renewal) — Valuation renewal, finite residue connectivity, and orbitwise gap
- [collatz-residual-core](https://github.com/KAMANOI/collatz-residual-core) — The residual core: structural decomposition
- [collatz-congruence-synchronization](https://github.com/KAMANOI/collatz-congruence-synchronization) — Paper H: nested congruence constraints on synchronization
- [collatz-record-renewal](https://github.com/KAMANOI/collatz-record-renewal) — Paper N: record renewal compatibility
- [collatz-hensel-escape](https://github.com/KAMANOI/collatz-hensel-escape) — Paper O: Hensel memory and 2-adic escape target
- [collatz-hensel-scarcity](https://github.com/KAMANOI/collatz-hensel-scarcity) — Paper T: Hensel conditional scarcity and telescoping contradiction
- [collatz-prefix-counting](https://github.com/KAMANOI/collatz-prefix-counting) — Paper V: direct prefix counting and synchronization collapse
- [collatz-first-passage](https://github.com/KAMANOI/collatz-first-passage) — Paper W: first-passage obstruction (closes series A–V)
- [collatz-series-summary](https://github.com/KAMANOI/collatz-series-summary) — Series summary: research program on Collatz synchronization dynamics
- [collatz-prime-survival](https://github.com/KAMANOI/collatz-prime-survival) — Paper X v20: prime survival in affine Collatz dynamics

---

## Author

Hiroki Kamanoi
hirokikamanoi@gmail.com
2026

---
Related research and services by HDR (Human Driven Reality): https://hdr-ai.com/#research
