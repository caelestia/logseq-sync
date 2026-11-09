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
- Suppose $s\in (f_!\mc F)(U)$, i.e. $s\in \mc F(f^{-1}(U))$ satisfies $\operatorname{supp} s\to U$ is proper, and $s|_{F_y}=0$.
- Then $U\setminus f(\operatorname{supp} s)$ is an open nhood of $y$ such that $s|_V=0$. Thus $s_y=0$.
- ### Surjectivity
- Let $s\in\Gamma_c(F_y,\mc F)$. Put $K=\operatorname{supp}s$.
- By [[Sections over compact subset]], we have
  $$\varinjlim_{U\supset K}\Gamma(U,\mc F) = \Gamma(K,\mc F),$$
  so there is $U\supset K$ and $t\in\mc F(U)$ such that $t|_{K}=s|_K$.
- Shrink $U$ so that $t|_{U\cap F_y}=s|_{U\cap F_y}$.
	- This is easily: set $U$ to be the union of  open nhoods around each point in $K$