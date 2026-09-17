# CEREBRON OMEGA — COLLATZ THEORY FARM — CHECKPOINT 2026-09-17

MISSION: work on the current arbitrary-N cycle obstruction. Do not restart. Do not claim Collatz solved.

Core exact state:
- T(x)=(3x+1)/2^{v2(3x+1)} on positive odds.
- For a hypothetical odd cycle: A=sum a_i, D=2^A-3^N>0, delta=A ln2-N ln3>0.
- Binary critical runs: 1^{u_j}2^{r_j}.
- H-factorization: 3^{u_j}t_j-1=4^{r_j}h_j and 2^{u_{j+1}}t_{j+1}-1=3^{r_j}h_j.
- h_j odd, h_j ≡ 5 (mod 6), h_j>=5.
- H-LOG exact: delta=sum_j ln[(1+(3^{r_j}h_j)^(-1))/(1+(4^{r_j}h_j)^(-1))].
- H-COUPLING exact: 2^{u_{j+1}+2r_{j+1}}h_{j+1}-3^{u_{j+1}+r_j}h_j=3^{u_{j+1}}-2^{u_{j+1}}.
- 3-adic address: h_j ≡ -4^{-r_j} (mod 3^{u_j}), ord_{3^u}(4)=3^{u-1}.

Primary target: derive a genuinely collective, non-tautological obstruction or upper bound from H-COUPLING + H-LOG + 3-adic constraints. Seek a theorem of the form small h -> large r OR compensatory cost elsewhere, or a monotone inter-run invariant.

Firewall: Dx_i=C_i, D|C_i, simple CRT, simple rotation differences, or any algebraic reconstruction of the cycle are EQUIVALENT-HARDNESS unless an independent new restriction appears.

ARITHMETIC COMPRESSION: SYMBOLIC REDUCTION BEFORE MULTIPLICATION. Factor before expansion; reuse powers/residues/recurrences; filter modulo 2^k or 3^k before large products; cache rho_u(h), Q_u(h), f(r); use log1p representations for H-LOG when only bounds are needed. Every optimization must preserve exactness and report COST BEFORE / TRANSFORMATION / COST AFTER / EQUIVALENCE CHECK / SAVED MULTIPLICATIONS.

Required output per role: ESTABLISHED / NEW DERIVATION / FALSIFICATION / GAP / NEXT LEMMA / STATUS in {VERIFIED,NARROWED,REJECTED,DUPLICATE,EQUIVALENT-HARDNESS,OPEN}. COMPUTATION != PROOF. FINITE TEST != UNIVERSAL PROOF. CONSENSUS != TRUTH.