- Let $G$ be a topological group. The following are equivalent:
	- (a) $G$ is Hausdorff and first countable;
	- (b) $G$ is metrizable as a topological space;
	- (c) $G$ has a left invariant metric.
- ## Proof
- If suffices to prove (a) implies (c).
- Choose a countable neighborhood basis $\{U_n\}_{n\geq1}$ at $1$, such that for all $n\geq1$,
	- $U_n=U_n^{-1}$,
	- $U_{n+1}U_{n+1}U_{n+1}\subset U_n$.
- Next, for each diadic rational number $r=\sum_{i=1}^k c_i2^{-i}$ in $(0,1)$, we assign the open set
  $$U(r):=U_1^{c_1}\cdots U_k^{c_k}.$$
- Also let $U(1)=G$. Now, define
  $$d(x,y)=d(1,x^{-1}y):=\inf\{r\in(0,1]\cap\text{diadic}: x^{-1}y\in U(r) \}.$$
- This satisfies
	- $d(x,y)\geq0$.
	- $d(x,y)=0$ iff $x^{-1}y=1$ iff $x=y$.
	- $