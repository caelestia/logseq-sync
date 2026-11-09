- Proposition. If $\mc F$ is c-soft and $f:X\to Y$ is a continuous map, then $f_!\mc F$ is c-soft.
- ## Proof 1
-
- ## Proof 2
- By [[Equivalent definition of c-soft]], it suffice to show $\Gamma_c(Y,f_!\mc F) \to \Gamma_c(Z,(f_!\mc F)|_Z)$ is surjectivev for every closed $Z\subset Y$.
- Write $f'=f|_{f^{-1}(Z)}:f^{-1}(Z)\to Z$ and $\mc F'=\mc F|_{f^{-1}(Z)}$. An application of the proper base change thm gives
  $$(f_!\mc F)|_Z \simeq f'_! \mc F'.$$
	- prove directly?
- Now the above observation gives
  $$
  \Gamma_c(X,\mc F) = \Gamma_c(Y,f_!\mc F),\qquad \Gamma_c(f^{-1}(Z),\mc F') = \Gamma_c(Z,(f_!\mc F)|_Z).
  $$
- The result follows from commutativity of the square...