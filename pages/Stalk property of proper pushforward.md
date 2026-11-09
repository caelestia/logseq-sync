- Lemma. Let $f:X\to Y$ be a map between LCH spaces. Let $\mc F$ be a sheaf on $X$.
  $$
  (R^nf_!\mc F)_y = H_c^n(F_y, \mc F|_{F_y})
  $$
  for all $y\in Y$ and $n\geq0$.
	- Definition of [[Proper pushforward]]
	- This is a special case of the [[Proper base change theorem]].
- ### Proof
- It suffices to prove the statement for $n=0$. We will prove that the restriction map
  $$
  (f_!\mc F)_y \longto \Gamma_c(F_y,\mc F)
  $$
  is a bijection.
- ### Injectivity
- Suppose $s\in \mc F(f^{-1}(U))$ satisfies $\operatorname{supp} s\to U$ is proper, and $s|_{F_y}=0$.
- Then $U\setminus f(\operatorname{supp} s)$ is an open nhood of $y$ such that $s|_V=0$