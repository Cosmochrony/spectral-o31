# spectral-o31

**SU(3) from Colour Triplet Co-admissibility: Towards the Complete Standard Model Gauge Group**

O31 paper — Spectral Admissibility Sub-programme.

## Abstract

Papers O27--O30 complete the analytical account of the SU(2) sector of the admissibility
programme, closing the chain emergence => su(2) => d_rho = 2 => lambda_1/lambda_2 = 2.
The only remaining non-numerical open problem in the gauge sector is the identification of
SU(3) as an admissibility fixed point, and thereby the derivation of the full Standard Model
gauge group SU(3) x SU(2) x U(1) as a composite.
The present paper formulates this problem precisely and develops the structural framework for
its resolution.

Three main contributions are obtained.

First, the O23 quaternionic minimality argument cannot directly yield d_rho = 3: the
Born--Infeld parity forces the unique minimal admissible algebra to be H (quaternions), with
dim_R Im(H) = 3 spectral directions and effective sector dimension d_rho = 2. A new input is
therefore required.

Second, the colour triplet is defined as an unordered set {c_1, c_2, c_3} in (Z/qZ)^*
satisfying c_1 + c_2 + c_3 = 0 (mod q) and pairwise non-conjugacy. Hypothesis [H-color] is
stated: the BFS fingerprint observables satisfy sigma_{c_1}(n) = sigma_{c_2}(n) = sigma_{c_3}(n)
for all shells n (triplet co-admissibility). Colour triplets exist if and only if q = 1 (mod 3).

Third, if [H-color] holds, the group of Born--Infeld-compatible fibre-preserving transformations
of V_color = C^3 is SU(3) (Theorem 5.2). The Standard Model gauge group G_SM = SU(3) x SU(2)
x U(1) follows as a composite of three independent admissibility fixed points.

Additionally, [H-color] is proved unconditionally for the colour-adapted Cayley graph
Cay(G_q, S_q^(3)) via the metaplectic intertwining identity (Theorem 4.4). U1 universality
implies |sigma_c - sigma_{omega c}| = O(q^{-1/2}) for any generating set, making the SU(3)
identification generating-set-independent in the large-q limit (two-tier result).

The paper also proves generator-twist isospectrality (Theorem 5.3): for every c in (Z/qZ)^*,
the Weil-sector Markov operators on S_q and on phi_omega(S_q) are unitarily conjugate, hence
isospectral. This is confirmed numerically for all primes q = 1 (mod 3), q <= 157.
However, spec(rho_c(P_{S_q})) =/= spec(rho_{omega c}(P_{S_q})) in general (max |Delta lambda|
approx 0.3-0.4), establishing that [H-color] on the standard graph cannot be derived from
global Markov-spectrum equality; the BFS capacity is a strictly finer observable.

Section 6 provides the conceptual unification: U(1), SU(2), SU(3) arise from BI-admissible
fibre orbits of size 1, 2, 3 respectively (phase non-injectivity, minimal correlated
non-injectivity, relational correlated non-injectivity), with non-factorisability (Foundation M
Axiom A3) as the uniform origin.

The O32 numerical campaign confirms [H-color] for q in {151, 211, 307} (4/4 triplets
each, R <= 0.5); at q=307, R = 0.31 with delta_tri = 12.355 ≈ 3*delta_c (deviation 1.5%).
The four-prime dataset q in {61, 151, 211, 307} is complete.

## Key results

- **Obstruction** (Proposition 2.2, proved): the O23 Hurwitz argument cannot produce d_rho = 3.
- **Colour triplet existence** (Proposition 3.2, proved): exist iff q = 1 (mod 3).
- **[H-color] for S_q^(3)** (Theorem 4.4, proved): metaplectic intertwining forces spectral
  degeneracy on the colour-adapted Cayley graph.
- **Naturality of S_q^(3)** (Proposition 4.6, proved): minimal generating set extending S_q
  and closed under phi_omega.
- **Approximate co-admissibility** (Proposition 4.7, proved from U1): |sigma_c - sigma_{omega c}|
  = O(q^{-1/2}) for the standard graph.
- **SU(3) uniqueness** (Theorem 5.2, proved conditional on [H-color]): the symmetry group is
  exactly SU(3); U(3), SO(3), U(2), G_2 are excluded.
- **G_SM derivation** (Corollary 5.5): SU(3) x SU(2) x U(1) as composite fixed point.
- **Generator-twist isospectrality** (Theorem 5.3, proved): spec(rho_c(P_{S_q})) =
  spec(rho_c(P_{phi_omega(S_q)})) for all c, confirmed for all q <= 157 with q = 1 (mod 3).
- **Closure** (Remark 5.4): spec(rho_c) =/= spec(rho_{omega c}) in general, so [H-color] on
  the standard graph requires a direct BFS capacity argument.
- **Intra-coset Vandermonde symmetry** (Lemma, proved): Schur's lemma forces the Heisenberg
  centre to act as a scalar in each irreducible representation rho_{c_i}; the triplet phase
  matrix (lambda_j = e^{2*pi*i*c_j/q}) is Vandermonde with non-zero determinant, so each
  horizontal coset (a,b) contributes exactly one independent direction to each colour
  summand V_{c_i}.
- **Colour sector rank equality** (Proposition, proved unconditionally): r_c(n) = r_{omega c}(n)
  = r_{omega^2 c}(n) for all BFS depths n, for any seed. Proves [H-color] at the BFS sector
  rank level, unconditionally. The algebraic mechanism (Schur + Vandermonde) is independent of
  any global Markov spectral property.
- **Gauge hierarchy** (Section 6): U(1)/SU(2)/SU(3) from fibre orbits of size 1/2/3.

## DOI

https://doi.org/10.5281/zenodo.20247746

## Compilation

```bash
bash compile.sh
```

Output: `out/Spectral-O31.pdf`
