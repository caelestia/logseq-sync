# Preliminaries
- Let $G$ be a group. Fix the commutative ring $k$ throughout, and all $G$-modules are over $k[G]$.
- If $M$ is a $G$-module, the *group cohomology* $H^\bullet(G;M)$ is the derived functor of $(\cdot)^G:k[G]\text{--Mod}\to k\text{--Mod}$.
- Since $(\cdot)^G=\operatorname{Hom}_{G}(k,\cdot)$, we have $H^\bullet(G;M)=\operatorname{Ext}^\bullet_{k[G]}(k,M)$.
- Hence, to compute the group cohomology, we often use the following "standard resolution"
  $$L_\bullet \xrightarrow{\epsilon} k$$
	- Each $L_{n}$ is a free $k$-module on the basis $G^{n+1}$, whose elements are the *homogeneous chains*.
	- As a $k[G]$-module with the diagonal action, $L_n$ has a basis of $G^n$. The basic elements are written as $(g_1|g_2|\cdots|g_n)\in G^n$. This is the *bar construction*.
	- The correspondence is $(g_1|\cdots|g_n) \mapsto (1_G,g_{[1,1]},g_{[1,2]},\cdots,g_{[1,n]})$.
-
- In the following we will define the *cup product* and *cross product* structures. This requires a $k$-algebra structure on $M$, given by $\mu:M\otimes M\to M$.
- For ease of notation, let's fix $M=k$.
- # First construction
-