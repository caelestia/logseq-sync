### Setup
- Suppose $X$ is a locally contractible space. This is necessary as indicated by the Warsaw circle.
- In the following we describe the outline of the proof from Global Calculus. We need to assume all open sets $U$ are paracompact. In the more natural [proof via hypersheaves](https://arxiv.org/pdf/2102.06927) this condition can be removed.
- Let $S^\bullet$ be the complex of presheaves of singular cochains in an abelian group $A$. $X$ is locally contractible means
- id:: 6971f907-ad12-4dc3-a10e-4beae435cfed
  $$0 \longrightarrow \underline{A} \longrightarrow S^\bullet$$
- is a resolution.
- Now observe for all $k\geq 0$:
	- $S^k$ is flasque, viz. the restrictions $S^k(U)\to S^k(V)$ are surjective for all $V\subset U$ open.
	- $S^k$ satisfies the glueing axiom of sheaves: If sections $\sigma_i\in S^k(U_i)$ agree on pairwise intersections then there exists $\sigma\in S^k(\bigcup_iU_i)$ glueing them.
	- However, $S^k$ are not sheaves unless $k=0$, since the glueing is obviously not unique.
- Hence we sheafify to get a complex of sheaves
- $$0 \longrightarrow \underline{A} \longrightarrow \tilde S^\bullet$$
- To conclude the proof, we need to show that
	- Lemma 1. If $U$ is paracompact, then the natural map $S^k(U)\to\tilde S^k(U)$ is surjective.
	- If follows that the sheaves $\tilde S^k$ are flasque, hence acyclic.
	- Lemma 2. Under our assumption of $X$, the morphism of complexes $S^\bullet(X)\to\tilde S^\bullet(X)$ is a quasi-isomorphism.
- ### Lemma 1
- A section in $\tilde{\mathcal{F}}(U)$ is given by sections