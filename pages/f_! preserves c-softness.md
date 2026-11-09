- Proposition. If $\mc F$ is c-soft and $f:X\to Y$ is a continuous map, then $f_!\mc F$ is c-soft.
- ## Proof 1
- Take a compact set $K\subset Y$ and a section $s\in\Gamma(K,(f_!\mc F)|_K)$.
- By [[Sections over compact subset]], this comes from some $\widetilde s\in\Gamma(U,f_!\mc F)$ where $U$ is an open nhood of $K$.
-
- ## Proof 2, base change
- By [[Equivalent definition of c-soft]], it suffice to show $\Gamma_c(Y,f_!\mc F) \to \Gamma_c(Z,(f_!\mc F)|_Z)$ is surjective for every closed $Z\subset Y$.
- Write $f'=f|_{f^{-1}(Z)}:f^{-1}(Z)\to Z$ and $\mc F'=\mc F|_{f^{-1}(Z)}$. An application of the proper base change thm gives
  $$(f_!\mc F)|_Z \simeq f'_! \mc F'.$$
	- This is a special case with a closed immersion. prove directly?
- Now the above observation gives
  $$
  \Gamma_c(X,\mc F) = \Gamma_c(Y,f_!\mc F),\qquad \Gamma_c(f^{-1}(Z),\mc F') = \Gamma_c(Z,(f_!\mc F)|_Z).
  $$
- The result follows from commutativity of the square, which can be proved by an explicit...