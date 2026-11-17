- Let $k$ be a perfect field.
- **Proposition.** If $A$, $B$ are reduced algebras over $k$, then $A\otimes_kB$ is also reduced.
- ### Proof.
- By the strong [[Nullstellensatz]], $J(A)=J(B)=0$, so we have injective maps
  $$
  A \hookrightarrow \prod_{\ideal m\in\text{MaxSpec}(A)} A/\ideal m, \qquad B \hookrightarrow \prod_{\ideal n\in\text{MaxSpec}(B)} B/\ideal n
  $$
- By flatness, $A\otimes_kB \hookrightarrow \prod_{\ideal m}K_{\ideal m}\otimes_k\prod_{\ideal n}L_{\ideal n}$.
- Claim. RHS embeds into $\prod_{\ideal m,\ideal n} K_{\ideal m}\otimes_k L_{\ideal n}$.
	- Proof. Denote the natural map as $\Phi$. Suppose $\Phi(z)=0$, where
	  $$
	  z = \sum_{r=1}^s a^{(r)}\otimes b^{(r)}.
	  $$
	- Then for every $(m,n)$, we have $\sum_r a^{(r)}(m)\otimes b^{(r)}(n)=0$ in $K_m\otimes L_n$.
	-
-
- ## When $k$ is not perfect