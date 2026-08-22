- > Following Analytic Methods in Algebraic Geometry by Demailly
- Let $X$ be a compact Kahler manifold of dimension $n$, $(E,h)$ be a Hermitian holomorphic vector bundle of rank $r$.
- Denote the curvature of the Chern connection by $\Theta_E$. Write
- $$i\Theta_E =: \sum_{j,k,\mu,\lambda} c_{jk\lambda\mu} dz^j \wedge d\bar z^k e_\lambda^*\otimes e_\mu.$$
- $\langle i\Theta_Eu,u\rangle$ can be viewed as a quadratic form on $T_X\otimes E$.
- If this is positive definite, we say that $(E,h)$ is *Nakano positive*.
- ## Bochner-Kodaira-Nakano
- In [[Nakano identities]], we computed
- $$\Delta_{\bar\partial_E}-\Delta_{\partial_E}=[i\Theta_E,\Lambda]$$
- The Bochner technique is essentially a "completing of squares". We know $\Delta_{\partial_E}$, as a Laplacian, is positive definite. If $u$ is a harmonic $(p,q)$-form, i.e. $\Delta_{\bar \partial_E}u=0$, we get
- $$\langle [i\Theta_E,\Lambda]u,u\rangle \leq 0.$$
- If $E$ satisfies a condition forcing $[i\Theta_E,\Lambda]$ to be positive definite, we get $u=0$, so by Hodge theory
- $$H^{p,q}(E)=\mathcal{H}^{p,q}(E)=0.$$
- Our next step is to expand this in coordinates.
- ## A computation
- Consider a $(p,q)$-form $u=\sum_{J,K,\lambda} u_{J,K,\lambda} dz^J\wedge d\bar z^K e_\lambda$. We want to compute
- $$\langle [i\Theta_E,\Lambda]u,u\rangle.$$
- Caution about the factors of $i$: since $[i\Theta_E,\Lambda]=i\Theta_E\Lambda-i\Lambda\Theta_E$ and $\Lambda^*=L$,
	- $$\langle[i\Theta_E,\Lambda]u,u\rangle
	=\langle i\Theta_E\Lambda u,u\rangle-\langle i\Theta_Eu,Lu\rangle.$$
	- Thus, if $\Theta_E=\partial_E\bar\partial_E+\bar\partial_E\partial_E$ is substituted, each term on the right carries a factor $i$.
	- The two summands $\partial_E\bar\partial_E$ and $\bar\partial_E\partial_E$ are not separately zero-order curvature operators, so splitting the first term according to their order is not useful for the pointwise computation. In particular, the two resulting scalars are not literally complex conjugates of one another.
- Choose normal holomorphic coordinates and an $h$-orthonormal frame at the point in question. Extend the coefficients $u_{J,K,\lambda}$ alternatingly in $J$ and $K$, so that inserting an index includes the appropriate wedge sign. Let $|R|=p-1$ and $|S|=q-1$. A direct wedge-contraction computation gives
	- $$\begin{aligned}
	\langle[i\Theta_E,\Lambda]u,u\rangle
	={}&\underbrace{\sum_{j,k,\lambda,\mu,J,S}
	c_{jk\lambda\mu}\,u_{J,jS,\lambda}\,
	\overline{u_{J,kS,\mu}}}_{A}\\
	&+\underbrace{\sum_{j,k,\lambda,\mu,R,K}
	c_{jk\lambda\mu}\,u_{kR,K,\lambda}\,
	\overline{u_{jR,K,\mu}}}_{B}\\
	&-\underbrace{\sum_{j,\lambda,\mu,J,K}
	c_{jj\lambda\mu}\,u_{J,K,\lambda}\,
	\overline{u_{J,K,\mu}}}_{C}.
	\end{aligned}$$
	- Here the sums over $J,K,R,S$ may equivalently be taken over increasing multiindices, provided coefficients with inserted indices are interpreted alternatingly.
- $B$ has the same shape as $A$ after interchanging the holomorphic and antiholomorphic form indices, but it is not the complex conjugate of $A$ for a fixed $E$-valued $(p,q)$-form. Actual conjugation also sends $u$ to a $\bar E$-valued $(q,p)$-form and uses the Hermitian symmetry $c_{jk\lambda\mu}=\overline{c_{kj\mu\lambda}}$.
- ## Nakano Vanishing
- We consider the special case $p=n$.
- Let $I=(1,\ldots,n)$. In the $B$-sum, $u_{kR,K,\lambda}$ and $u_{jR,K,\mu}$ can both be nonzero only when $j=k$ is the unique index missing from $R$. Hence $B=C$, and
	- $$\langle[i\Theta_E,\Lambda]u,u\rangle
	=\sum_{j,k,\lambda,\mu,S}
	c_{jk\lambda\mu}\,u_{I,jS,\lambda}\,
	\overline{u_{I,kS,\mu}}.$$
- For every fixed $(q-1)$-multiindex $S$, the array $(u_{I,jS,\lambda})_{j,\lambda}$ is an element of $T_X\otimes E$. Thus Nakano positivity makes the last expression positive for every nonzero $(n,q)$-form when $q\geq 1$.
-
