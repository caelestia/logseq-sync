- *Serre* proof of Lagrange's four squares thm:
	- (Aubry, Davenport and Cassels) Consider an inner product on $\mathbb Q^N$, that is, a positive definite bilinear form $\sum_{i,j}^Na_{ij}X_iY_j$. Put $f(x)=x\cdot x$. Suppose that the $f$ represents some number $n\in\Z$ over $\mathbb Q$, then it also represents it over $\Z$, under the following:
		- Assumption: For every $x\in\mathbb Q^N$, there exists $y\in\Z^n$ such that $f(x-y)<1$.
		- Proof: Suppose $f(x)=t^2n$ is such that the positive integer $t$ is smallest. Take $y\in\Z^N$ such that $z:=x/t-y$ satisfies $f(z)<1$. If $f(z)=0$, $t=1$ so qed. Hence assume $0<f(z)<1$.
		- We then generate a new point $x'$ such that $f(x')=t'^2n$ with $t'<t$. This is given by
			- $a=f(y)-n\ \in\Z$.
			- $b=2(nt-x\cdot y)\ \in\Z$.
			- $t'=at+b\ \in\Z$. Then $t'=tf(z)<t$.
			- $x'=ax+by$.
		- Then $f(x')=t'^2n$. Contradiction.
	- We can apply this to the forms $X^2+Y^2$ and $X^2+Y^2+Z^2$, but not the "four squares". This is because the best appoximation has error $\frac{1}{4}N$.
		- LATER What if we try to approximate with half-integers instead?
		  :LOGBOOK:
		  CLOCK: [2025-11-25 Tue 23:54:35]--[2025-11-25 Tue 23:54:36] =>  00:00:01
		  CLOCK: [2025-11-25 Tue 23:54:42]--[2025-11-25 Tue 23:54:42] =>  00:00:00
		  :END:
	- Using Hasse-Minkowski, we see that: $n$ is the sum of $3$ rational squares IFF $n$ is the sum of three integral squares IFF $-n$ is not a square in $\mathbb Q_2$ IFF $n$ is not of the form $4^a(8b-1)$ for $a,b\in\Z$.
		- Explain the last step. Recall that over the local field $\mathbb Q_p$, the image of the quadratic form is completely determined by the three invariants: its dimension $d$, discriminant $\Delta$ and its Hasse invariant $\varepsilon$.
		-
- Hilbert symbol. For a place $v$ of $\mathbb Q$, the Hilbert symbol is the function $(-,-)_v:\mathbb Q_v\times\mathbb Q_v\longrightarrow\{\pm 1\}$, such that $(a,b)_v=1$ iff $ax^2+by^2=1$ is solvable.
  id:: 695af663-092e-4cca-bd5c-c8cbd075aa06
	- Computation of the Hilbert symbol. = Local criterion.
		- If $v=\infty$, $(a,b)_\infty=1$ iff $a>0$ or $b>0$.
		- For $v=p$, let $a=p^i\alpha$ and $b=p^j\beta$ where $\alpha,\beta\in\Z_p^\times$. Put $r:=(-1)^{ij}a^jb^{-i}\in\Z_p^\times$. Then:
			- If $p$ is odd, $(a,b)_p=(\dfrac{r}{p})$.
			- If $p=2$, $(a,b)_2=(-1)^{\epsilon(\alpha)\epsilon(\beta)+\omega(r)}$ where
			  collapsed:: true
				- $\epsilon(u)=\begin{cases}0,&u\equiv1\pmod4\\1,&u\equiv3\pmod4\end{cases}$
				- $\omega(u)=\begin{cases}0,&u\equiv1,7\pmod8\\1,&u\equiv3,5\pmod8\end{cases}$
			- Proof. Check that RHS satisfies $(a,b)=(b,a)$, $(a,bc)=(a,b)(a,c)$ and $(a,-a)=1$ directly. Thus reduce to the case $a\in\Z_p^\times$ and $b\in\Z_p^\times\cup p\Z_p^\times$. The rest is omitted.
	- Corollary. For odd $p$, we have
		- $(a,p)_p=(-1)^{i\epsilon(p)}(\dfrac{\alpha}{p})$. This is case $b=p$ in the above.
		- $(\alpha,\beta)_p=1$. This is case $i=j=0$.
	- The Hilbert symbol is a non-degenerate $\mathbb F_2$-bilinear form on $\mathbb Q_v^\times/\mathbb Q_v^{\times2}$.
		-