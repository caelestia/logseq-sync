- Let $f:X\to Y$ be a map between LCH spaces. Let $\mc F$ be a sheaf on $X$.
- The direct image with proper supports (proper pushforward) $f_!\mc F$ is defined as
  $$
  (f_!\mc F)(U) = \{s\in\Gamma(f^{-1}(U),\mc F): \operatorname{supp}s \to U \text{ is proper}\}.
  $$
	- See [definition of proper maps here]([[Proper maps]]).
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
	- Proof.
-