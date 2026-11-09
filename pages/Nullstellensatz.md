## Weak Nullstellensatz
- Let $k$ be an alg closed field. Let $I \trianglelefteq k[X_1,\cdots,X_n]$.
- Theorem. If $V(I)=\varnothing$ then $1\in I$.
- ### reduction
- Take a maximal ideal $\mathfrak m$ containing $I$, then $V(\mathfrak m) \subset V(I) = \varnothing$. Thus it amounts to prove the following statement (which is also called the weak Nullstellensatz in some cases).
- Proposition. If a field extension $L/K$ is finitely generated as a $k$-algebra (of finite type), then $[L:K]<\infty$ (finite).
- ### proof
- By [[Noether normalization]], $K \to L$ factorizes as two inclusions $K \to K[T_1,\cdots,T_d] \to L$ where the second inclusion is finite.
- Since $L$ is a field, this implies $K[T_1,\cdots,T_d]$ is also a field. Thus $d=0$.