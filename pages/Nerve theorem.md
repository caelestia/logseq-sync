- Fix $X$ paracompact Hausdorff. Let $\mathcal{U}=\{U_i\}_{i\in I}$ be a locally finite good open cover (viz. all nonempty finite intersections are contractible), we have the nerve $N_\mathcal{U}$, which can be viewed as a simplicial set (or, a simplicial complex).
	- ref: Shastri
- **Theorem**. There is a homotopy equivalence $h_\mathcal{U}:X\to|N_\mathcal{U}|$.
- First, recall that the CW complex $|N_\mathcal{U}|$ has a cell for each non-degenerate simplex in $N_\mathcal{U}$. We get a map $\rho:|N_\mathcal{U}|\to\mathcal{P}(X)$. Define
  $$\mathcal{D}:=\mathcal{D}_\mathcal{U}=\{(a,x):x\in\rho(a)\}.$$
  This has projections $p,q$ to $|N_\mathcal{U}|, X$ respectively.
- Lemma. There is a deformation retract $X$