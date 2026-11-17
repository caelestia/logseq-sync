- Let $k$ be a perfect field.
- **Proposition.** If $A$, $B$ are reduced algebras over $k$, then $A\otimes_kB$ is also reduced.
- ### Proof.
- WLOG assume $A$ and $B$ are finitely generated.
- By the strong [[Nullstellensatz]], $J(A)=J(B)=0$, so we have injective "evaluation" maps
  $$
  A \hookrightarrow \prod_{\ideal m\in\text{MaxSpec}(A)} A/\ideal m, \qquad B \hookrightarrow \prod_{\ideal n\in\text{MaxSpec}(B)} B/\ideal n
  $$
- And by the weak Nullstellensatz, $A/\ideal m$ and $B/\ideal n$ are finite, hence separated, extensions of $k$.
- By flatness, $A\otimes_kB \hookrightarrow \prod_{\ideal m}K_{\ideal m}\otimes_k\prod_{\ideal n}L_{\ideal n}$.
- Claim. RHS embeds into $\prod_{ m, n} K_{ m}\otimes_k L_{ n}$. This works for any two family $K_m$ and $L_n$ of vector spaces over any field.
	- Proof. Denote the natural map as $\Phi$. Suppose $\Phi(z)=0$, where
	  $$
	  z = \sum_{r=1}^s a^{(r)}\otimes b^{(r)}.
	  $$
	- By shortening the sum when necessary, we may assume $\{b^{(r)}\}$ are linearly independent.
	- Then for every $(m,n)$, we have $\sum_r a^{(r)}(m)\otimes b^{(r)}(n)=0$ in $K_m\otimes L_n$.
	- Fix $m$ and choose a basis $\{e_i\}$ of $K_m$. Expand
	  $$
	  a^{(r)}(m) = \sum_i c^{r}_{m,i} e_i,\qquad c^{r}_{m,i} \in k.
	  $$
	- We get
	  $$\sum_r \sum_i c^r_{m,i} e_i \otimes b^{(r)}(n) = \sum_i e_i\otimes \sum_r c^r_{m,i} b^{(r)}(n) = 0,\qquad \forall n.$$
	- Thus $\sum_r c^r_{m,i} b^{(r)} = 0$ in $\prod_n L_n$.
	- By linear independence, we get $a^{(r)}(m)=0$. $m$ is arbitrary, so $a^{(r)}=0$. QED
- It remains to make the following observation.
- Claim. If $K/k$ and $L/k$ are finite extensions,. $K/k$ is separable, then $K\otimes L$ is a product of finite separable extensions.
	- Proof. By the primitive element theorem, $K=k[X]/(f)$, where $f$ has no repeated roots in $\bar k$. Then $f$ splits into distinct irred factors in $L$. By CRT, we win.
- ## When $k$ is not perfect
- counterexample