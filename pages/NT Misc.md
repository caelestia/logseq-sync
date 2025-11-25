- *Serre* proof of Lagrange's four squares thm:
	- (Aubry, Davenport and Cassels) Consider an inner product on $\mathbb Q^N$, that is, a positive definite bilinear form $\sum_{i,j}^Na_{ij}X_iY_j$. Put $f(x)=x\cdot x$. Suppose that the $f$ represents some number $n\in\Z$ over $\mathbb Q$, then it also represents it over $\Z$, under the following:
	  collapsed:: true
		- Assumption: For every $x\in\mathbb Q^N$, there exists $y\in\Z^n$ such that $f(x-y)<1$.
		- Proof: Suppose $f(x)=t^2n$ is such that the positive integer $t$ is smallest. Take $y\in\Z^N$ such that $z:=x/t-y$ satisfies $f(z)<1$. If $f(z)=0$, $t=1$ so qed. Hence assume $0<f(z)<1$.
		- We then generate a new point $x'$ such that $f(x')=t'^2n$ with $t'<t$. This is given by
		  collapsed:: true
			- $a=f(y)-n\ \in\Z$.
			- $b=2(nt-x\cdot y)\ \in\Z$.
			- $t'=at+b\ \in\Z$. Then $t'=tf(z)<t$.
			- $x'=ax+by$.
		- Then $f(x')=t'^2n$. Contradiction.
	- We can apply this to the forms $X^2+Y^2$ and $X^2+Y^2+Z^2$, but not the "four squares". This is because the best appoximation has error $\frac{1}{4}N$.
	  collapsed:: true
		- LATER What if we try to approximate with half-integers instead?
		  :LOGBOOK:
		  CLOCK: [2025-11-25 Tue 23:54:35]--[2025-11-25 Tue 23:54:36] =>  00:00:01
		  CLOCK: [2025-11-25 Tue 23:54:42]--[2025-11-25 Tue 23:54:42] =>  00:00:00
		  :END:
	- Together with Hasse-Minkowski, we see that
-