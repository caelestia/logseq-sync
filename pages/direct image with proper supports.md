- Let $f:X\to Y$ be a map between LCH spaces. Let $\mc F$ be a sheaf on $X$.
- The direct image with proper supports (proper pushforward) $f_!\mc F$ is defined as
  $$
  (f_!\mc F)(U) = \{s\in\Gamma(f^{-1}(U),\mc F): \operatorname{supp}s \to U \text{ is proper}\}.
  $$
	- See [definition of proper maps here]([[Proper maps]]).
- ### support
- Lemma. Let $s\in(f_!\mc F)(U)$, also viewed as a section of $\mc F$ over $f^{-1}(U)$. Then
  $$\supp_U(s) = f(\supp_{f^{-1}(U)}(s)).$$
  In particular, note that RHS is closed.
- Proof. Obvious.
- ### composition
- Proposition. If $f:X\to Y$ and $g:Y\to Z$, we have $(g\circ f)_! = g_! \circ f_!$.
	- In particular, if $g=p_Y:Y\to\{\text{pt}\}$, this says $\Gamma_c(X,-)=\Gamma_c(Y,f_!-)$.
	- Proof.
- ## Derived functor
- Observe that $f_!$ is left exact. Using standard injective resolutions, we get a derived functor $Rf_!:D^+(X,k)\to D^+(Y,k)$.
- Definition. We say $\mc F$ is c-soft if for every compact $K\subset X$ the restriction $\Gamma(X,\mc F)\to\Gamma(K,\mc F)$ is surjective.
- Let $X$ be Hausdorff. We have the chain of implications:
  $$
  \text{injective} \implies \text{flasque} \implies \text{c-soft} \implies f_!\text{-acyclic}
  $$
- The first $\implies$ is well-known and the second is [[Sections over compact subset]]. For the third one we need some lemmas first.
- Proposition. $\mc F$ is c-soft iff for every closed $Z\subset X$, the restriction $\Gamma_c(X,\mc F)\to\Gamma_c(Z,\mc F|_Z)$ is surjective.
	- Proof. [[Equivalent definition of c-soft]].
- Proposition. If $\mc F$ is c-soft and $f:X\to Y$ is a continuous map, then $f_!\mc F$ is c-soft.
	- Proof. [[f_! preserves c-softness]]
- Corollary. We have $R(g\circ f)_! = Rg_! \circ Rf_!$. In language of spectral sequences, this gives
  $$
  E_2^{p,q} = R^pg_! \circ R^qf_! (\mc F) \implies R^{p+q} (g\circ f)_! (X).
  $$
	- Taking $g=p_Y$ gives the Leray spectral sequence for $f_!$,
	  $$E_2^{p,q} = H_c^p(Y,R^pf_!\mc F) \implies H_c^{p+q}(X,\mc F)$$