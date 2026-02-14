- Fix $X$ paracompact Hausdorff. Let $\mathcal{U}=\{U_i\}_{i\in I}$ be a locally finite good open cover (viz. all nonempty finite intersections are contractible), we have the nerve $N_\mathcal{U}$, which can be viewed as a simplicial set (or, a simplicial complex).
	- ref: Shastri
- **Theorem**. There is a homotopy equivalence $h_\mathcal{U}:X\to|N_\mathcal{U}|$.
- First, recall that the CW complex $|N_\mathcal{U}|$ has a cell for each non-degenerate simplex in $N_\mathcal{U}$. We get a map $\rho:|N_\mathcal{U}|\to\mathcal{P}(X)$. Define
  $$\mathcal{D}:=\mathcal{D}_\mathcal{U}=\{(a,x):x\in\rho(a)\}.$$
  This has projections $p,q$ to $N:=|N_\mathcal{U}|, X$ respectively.
- We proceed in two steps:
	- Step 1. There is a section $s$ of $q$ such that $s(X)\simeq X$ is a DR of $\mathcal{D}$. Thus $q$ is a homotopy equivalence.
	- Step 2. $\mathcal{D}$ is a deformation retract of $M(p)$. Thus $p$ is a homotopy equivalence.
- ### Step 1
- Pick $\theta_i$ a partition of unity subordinate to $\mathcal{U}$. Since $\theta_i(x)>0\Longleftrightarrow x\in\operatorname{supp}\theta_i$ holds for finitely many $i$, we have a map $\Theta:x\mapsto[j\mapsto\theta_j(x)]\in|N_\mathcal{U}|$ mapping $x$ to the simplex given by these $i$.
- Then $s:x\mapsto(\Theta(x),x)$ is a section of $q$ and we can check its continuity locally.
- It is clearly a deformation retract, as we can exhibit the homotopy
  $$H:\mathcal{D}\times I\to\mathcal{D},\quad ((a,x),t)\mapsto(t\Theta(x)+(1-t)a,x)$$ 
  because the simplex is convex.
- ### Step 2
- Let $\mathcal{D}^k=p^{-1}(N^{(k)})$ and $p^k=p|_{\mathcal{D}^k}$.
- First we show that for all $k\geq0$, $\mathcal{D}^k\cup M(p^{k-1})$ is a SDR of $M(p^k)$, naturally in $k$, by induction.
	- If $k=0$, $\mathcal{D}^0=\bigsqcup_i\{i\}\times U_i$, and $M(p^0)$ is the disjoint union of cones over the $U_i$. Since each $U_i$ is contractible, there is a DR