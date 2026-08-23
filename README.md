# spectral-o31

**Withdrawal Notice for O31: Unsupported Colour-Triplet Co-admissibility and Gauge-Group Claims**

Cosmochrony — Spectral Admissibility Sub-programme.

## Status

This record carries a **withdrawal notice**, not a paper. Eight results of the previous version are
withdrawn, three counterexamples are given in full, and the remaining material is under re-audit.

**No positive conclusion about groups, gauge factors, or the Standard Model gauge group is asserted
by this record, and none should be inferred from it.**

Earlier versions remain available and citable in the record's version history, for traceability.

## Withdrawn

1. Uniqueness of SU(3) among connected compact subgroups acting irreducibly on C^3.
2. Irreducibility of the group of Born–Infeld-compatible fibre-preserving transformations.
3. Co-admissibility of the individual profiles sigma_{c_1}, sigma_{c_2}, sigma_{c_3}.
4. The arithmetic criterion "colour triplets exist iff q = 1 (mod 3)".
5. The metaplectic identity as used, which changes the central character while the automorphism
   invoked fixes the centre.
6. The Delta(27) spectral proposition relating characters and adjacency eigenvalues.
7. The rank-8 test in End(C^3), which is mistyped: dim_C End(C^3) = 9.
8. Every derivation of a gauge factor and of the Standard Model gauge group as a composite,
   together with the determinant-one condition, the commutation of the putative factors and the
   direct-product structure.

## Counterexamples

- **Uniqueness fails.** SO(3) ⊂ SU(3) is a proper connected compact subgroup (dim 3 < 8) whose
  action on C^3 is the complexification of its defining representation, irreducible over C by
  Schur.
- **Irreducibility fails.** The diagonal torus T^2 = {diag(e^{i a}, e^{i b}, e^{-i(a+b)})} ⊂ SU(3)
  satisfies every constraint imposed while preserving the three coordinate lines. Requiring each
  sector to be mapped to itself in fact forces reducibility.
- **The arithmetic criterion fails.** For every prime q >= 7, {1, 2, q-3} is an admissible colour
  triplet under the published definition: its pairwise sums are 3, q-2 and q-1, none divisible by
  q. q = 5 fails only because q-3 = 2 duplicates. For instance q = 11 admits {1, 2, 8}, and
  11 = 2 (mod 3).

## Under re-audit

The scalar, arithmetic and discrete-group material of the previous version is under re-audit and is
not asserted. The generator-twist isospectrality statement at fixed central character may be
recoverable; if an autonomous proof is established it will appear as a separate work.

## DOI

Concept DOI (always resolves to the latest version): https://doi.org/10.5281/zenodo.20030491

## Compilation

The notice carries no bibliography, so `compile.sh` (which runs bibtex under `set -e`) is not used:

```bash
mkdir -p out
pdflatex -file-line-error -interaction=nonstopmode -output-directory=out tex/Spectral-O31.tex
pdflatex -file-line-error -interaction=nonstopmode -output-directory=out tex/Spectral-O31.tex
```

Output: `out/Spectral-O31.pdf`
