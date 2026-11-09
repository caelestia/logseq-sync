- Let $f:X\to Y$ be a map between LCH spaces. Let $\mc F$ be a sheaf on $X$.
- The direct image with proper supports (proper pushforward) $f_!\mc F$ is defined as
  $$
  (f_!\mc F)(U) = \{s\in\Gamma(f^{-1}(U),\mc F): \operatorname{supp}s \to U \text{ is proper}\}.
  $$
	- See [definition of proper maps here]([[Proper maps]]).
- ### composition
- Proposition. If $f:X\to Y$ and $g:Y\to Z$, we have $(g\circ f)_! = g_! \circ f_!$.
	- In particular, if $g=p_Y:Y\to\{\text{pt}\}$, this says $\Gamma_c(X,-)=\Gamma_c(Y,f_!-)$.
	- Proof.
- ## Derived functor
- Definition. We say $\mc F$ is c-soft if for every compact $K\subset X$ the restriction $\Gamma(X,\mc F)\to\Gamma(K,\mc F)$ is surjective.
- Let $X$ be Hausdorff. We have the chain of implications:
  $$
  \text{injective} \implies \text{flasque} \implies \text{c-soft} \implies f_!\text{-acyclic}
  $$
- The first $\implies$ is well-known and the second is [[Sections over compact subset]]. For the third one we need some lemmas first.
- Proposition. $\mc F$ is c-soft iff for every closed $Z\subset X$, the restriction $\Gamma_c(X,\mc F)\to\Gamma_c(Z,\mc F|_Z)$ is surjective.
	- Proof. [[Equivalent definition of c-soft]].
- Proposition. If $\mc F$ is c-soft and $f:X\to Y$ is a continuous map, then $f_!\mc F$ is c-soft.
	- Proof. By the previous, it suffice to show $\Gamma_c(Y,f_!\mc F) \to \Gamma_c(Z,(f_!\mc F)|_Z)$ is surjectivev for every closed $Z\subset Y$.
	- Write $f'=f|_{f^{-1}(Z)}:f^{-1}(Z)\to Z$. An application of proper base change thm gives
	  $$(f_!\mc F)|_Z \simeq f'_! \mc F|_{f^{-1}(Z)}.$$
		- prove directly?
	- Now the above observation gives
	  $$
	  \Gamma_c(X,\mc F) = \Gamma_c(Y,f_!\mc F),\qquad \Gamma_c(f^{-1}(Z),\mc F) = \Gamma_c(Z,(f_!\mc F)|_Z).
	  $$
	-