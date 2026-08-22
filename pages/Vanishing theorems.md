- > Following Analytic Methods in Algebraic Geometry by Demailly
- Let $X$ be a compact Kahler manifold of dimension $n$, $(E,h)$ be a Hermitian holomorphic vector bundle of rank $r$.
- Denote the curvature of the Chern connection by $\Theta_E$. Write
- $$\Theta_E = \sum_{j,k,\mu,\lambda} c_{jk\lambda\mu} dz^j \wedge d\bar z^k e_\lambda^*\otimes e_\mu.$$
- $\langle i\Theta_Eu,u\rangle$ can be viewed as a quadratic form on $T_X\otimes E$.
	- Proof. It's well-known from Chern-Weil theory that $\Theta_E$ is skew-Hermitian, so
	- $$i\Theta_{E}\in
	  C^\infty\!\left(X,\Lambda^{1,1}T_X^*\otimes\operatorname{Herm}(E,E)\right).$$
	- This means $c_{jk\lambda\mu}=\overline{c_{kj\mu\lambda}}$.
	- Thus evaluated on any vector $u=\sum u_{j\lambda} \partial_j e_\lambda$, we have
	- $$\langle i\Theta_Eu,u\rangle = \sum_{j,k,\lambda,\mu}c_{jk\lambda\mu}u_{j\lambda}\overline{u_{k\mu}}$$
	- is real.
- If this quadratic form is positive definite, we say that $(E,h)$ is *Nakano positive*.
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
- $$\langle[i\Theta_E,\Lambda]u,u\rangle.$$
- At the center of normal coordinates, write
- $$\varepsilon_j=dz^j\wedge-,\qquad
  \iota_j=\varepsilon_j^*.$$
- Write $E_{\mu\lambda}=e_\lambda^*\otimes e_\mu$. Then by the computation in [[Kahler identities]],
- $$L=i\sum_\ell\varepsilon_\ell\bar\varepsilon_\ell,\qquad
  \Lambda=-i\sum_\ell\bar\iota_\ell\iota_\ell,\qquad
  i\Theta_E=i\sum_{j,k,\lambda,\mu}c_{jk\lambda\mu}
  \varepsilon_j\bar\varepsilon_kE_{\mu\lambda}.$$
- We use
- $$\iota_\ell\varepsilon_j+\varepsilon_j\iota_\ell=\delta_{\ell j},\qquad
  \bar\iota_\ell\bar\varepsilon_k+\bar\varepsilon_k\bar\iota_\ell=\delta_{\ell k},$$
- and holomorphic and antiholomorphic odd operators anticommute. For fixed $j,k,\ell$ this gives
- $$\begin{aligned}
  \varepsilon_j\bar\varepsilon_k\bar\iota_\ell\iota_\ell
  &=\delta_{k\ell}\varepsilon_j\iota_\ell
  +\bar\iota_\ell\varepsilon_j\bar\varepsilon_k\iota_\ell,\\
  \bar\iota_\ell\iota_\ell\varepsilon_j\bar\varepsilon_k
  &=\delta_{j\ell}\delta_{k\ell}
  -\delta_{j\ell}\bar\varepsilon_k\bar\iota_\ell
  +\bar\iota_\ell\varepsilon_j\bar\varepsilon_k\iota_\ell.
  \end{aligned}$$
- Thus
- $$[i\Theta_E,\Lambda]
  =\sum_{j,k,\lambda,\mu}c_{jk\lambda\mu}
  \left(\bar\varepsilon_k\bar\iota_j
  +\varepsilon_j\iota_k-\delta_{jk}\right)E_{\mu\lambda}.$$
- If $|R|=p-1$ and $|S|=q-1$, then removing and reinserting an index gives
- $$\begin{aligned}
  \langle\bar\varepsilon_k\bar\iota_jE_{\mu\lambda}u,u\rangle
  &=\sum_{J,S}u_{J,jS,\lambda}\overline{u_{J,kS,\mu}},\\
  \langle\varepsilon_j\iota_kE_{\mu\lambda}u,u\rangle
  &=\sum_{R,K}u_{kR,K,\lambda}\overline{u_{jR,K,\mu}},\\
  \langle E_{\mu\lambda}u,u\rangle
  &=\sum_{J,K}u_{J,K,\lambda}\overline{u_{J,K,\mu}}.
  \end{aligned}$$
- Substitution into the operator identity yields
- $$\begin{aligned}
  \langle[i\Theta_E,\Lambda]u,u\rangle
  ={}&\sum_{j,k,\lambda,\mu,J,S}
  c_{jk\lambda\mu}u_{J,jS,\lambda}\overline{u_{J,kS,\mu}}\\
  &+\sum_{j,k,\lambda,\mu,R,K}
  c_{jk\lambda\mu}u_{kR,K,\lambda}\overline{u_{jR,K,\mu}}\\
  &-\sum_{j,\lambda,\mu,J,K}
  c_{jj\lambda\mu}u_{J,K,\lambda}\overline{u_{J,K,\mu}}.
  \end{aligned}$$
- ## Nakano Vanishing
- We consider the special case $p=n$.
- Let $I=(1,\ldots,n)$. In the second sum, $u_{kR,K,\lambda}$ and $u_{jR,K,\mu}$ can both be nonzero only when $j=k$ is the unique index missing from $R$. Hence the second and third sums cancel, and
	- $$\langle[i\Theta_E,\Lambda]u,u\rangle
	  =\sum_{j,k,\lambda,\mu,S}
	  c_{jk\lambda\mu}\,u_{I,jS,\lambda}\,
	  \overline{u_{I,kS,\mu}}.$$
- For every fixed $(q-1)$-multiindex $S$, the array $(u_{I,jS,\lambda})_{j,\lambda}$ defines an element of $T_X\otimes E$. Thus Nakano positivity makes the last expression positive for every nonzero $(n,q)$-form $u$ when $q\geq 1$.
	- If $q=0$ then this is always $0$ because $\{S\}=\varnothing$, so not positive.
- Thm. Let $X$ be a compact complex manifold. If $E$ is Nakano positive, then $X$ is Kahler, and
- $$H^{n,q}(E)= H^q(X,K_X\otimes E) = 0.$$
	- Proof. We know $\operatorname{Tr}(i\Theta_E)$ is real by the discussion above. We know it's closed by Bianchi's identity.
-