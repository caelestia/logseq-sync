- Let $\cat A$ be an abelian category with enough injectives.
- Let $F:\cat A \to \cat B$ be a left exact additive functor.
- Hypercohomology is denoted as $\R^nF = H^n \circ R^+F$.
- ## First hypercohomology spectral sequence
- Let $K^\bullet\in C^+(\cat A)$, we have the SS
  $$
  E_2^{p,q} = R^pF (H^q(K^\bullet)) \implies \R^{p+q}F (K^\bullet).
  $$
- ### Proof.
- Let $K^\bullet \to J^{\bullet,\bullet}$ be the Cartan-Eilenberg resolution (the second index is for resolution). Then, in particular, we have
	- For every $q$, $H^q(K^\bullet) \longto H^q(J^{\bullet,0}) \longto H^q(J^{\bullet,1}) \longto \cdots$ is an injective resolution;
	- Moreover, $FH^q(J^{\bullet,p})=H^q(FJ^{\bullet,p})$.
- Then the row-first SS of $FJ^{\bullet,\bullet}$ is
  $$
  E_1^{p,q} = H^q(FJ^{\bullet,p}) = FH^q(J^{\bullet,p}) \implies H^{p+q}(F(\operatorname{tot}J)).
  $$
- The column-first spectral sequence of $J^{\bullet,\bullet}$ collapses at $E_2$-page, giving
  $$
  H^p(K^\bullet) \simeq H^p (\operatorname{tot} J),
  $$
  so $K^\bullet\to\operatorname{tot} J$ is a quasi-isomorphism (to see that the isomorphism is induced by this, we can chase elements under the edge map, or view $K^\bullet$ as a double complex concentrated at the bottom row and use naturality of spectral sequences.)
- Therefore
- ## Second hypercohomology SS (stupid)
-