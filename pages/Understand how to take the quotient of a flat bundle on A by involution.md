- Consider a polydisc or some nice contractible $0\in D\subset\mathbb C^2$, and the trivial rank $2$ vector bundle $D\times \mathbb C^2$ over it.
- We want to lift the involution linearly $\iota$ to $\tilde\iota$ on this bundle.
	- At the fixed point $(0,0)$, the matrix satisfies $M^2=1$, so it is diagonalizable and has eigenvalues $\pm1$.
	- Let it have $p=0,1,2$ plus one's and $q=2-p$ minus one's. Call this matrix $I_{p,q}$.
	- Since the bundle trivializes, the fibers can be identified, whence $\tilde\iota$ acts on all points by a matrix of the form $I_{p,q}$. But by continuity they must all be the same.
	- Hence we can suppose $\tilde\iota((x,y),(s,t))=((-x,-y),I_{p,q}(s,t))$.
- Let $U=D\setminus\{0\}$. Consider two charts $U_x=\{x\neq0\}$ and $U_y=\{y\neq0\}$. We have:
	- These are Stein manifolds.
		- This follows from the following two standard facts:
			- Any open subset of $\mathbb C$ is a Stein manifold.
			  logseq.order-list-type:: number
			- The product of two Stein manifolds is a Stein manifold.
			  logseq.order-list-type:: number
	- Oka-Grauert principle applies:
		- https://ncatlab.org/nlab/show/Oka+principle
		- On a Stein manifold, two vector bundles are holomorphically isomorphic iff they are topologically isomorphic.
	- These charts are homotopy equivalent to $S^1$.
		- By the clutching construction, topological vector bundles of rank $n$ are characterized by $\pi_0(\mathrm{GL}_n(\mathbb C))$.
		- This is always trivial since $\mathrm{GL}_n(\mathbb C)$ is connected.
- We conclude that all vector bundles are trivial over $U_x$ and $U_y$.
	- In particular, all vector bundles on $U$ will be characterized by a transition matrix on $U_x\cap U_y$.
- ---
- Next we need to consider $U/\langle\iota\rangle$. I have three ways of finding charts on it:
	- Obviously, we can cover it with four charts:
	  logseq.order-list-type:: number
		- $\{Re(x)>0\} \cup \{Im(x)>0\} \cup \{Re(y)>0\} \cup \{Im(y)>0\}$
	- We can also cover it with two charts as follows.
	  logseq.order-list-type:: number
		- The map $\pi:\mathbb C^2\setminus\{0\} \to \mathbb P^1$, $(x,y)\mapsto[x:y]$ shows that $\mathbb C^2\setminus\{0\}$ is the total space of $\mathcal{O}_{\mathbb{P}^1}(-1)$ minus the zero section.
		- When we take the quotient by $\iota$, the transition function gets squared. So we have
		- $$(\mathbb{C}^2\setminus\{0\})/\langle\iota\rangle \simeq \text{total space of }\mathcal{O}_{\mathbb P^1}(-2) \setminus \text{zero section}$$
		- Now $\mathcal{O}_{\mathbb P^1}(-2)$ is the same as the cotangent bundle.
		- This bundle trivializes when we cover $\mathbb{P}^1$ with two charts $\{x\neq0\}$ and $\{y\neq0\}$.
			- $V_x=\{x\neq0\}=\{[1:y]:y\in\mathbb C\}$,
			  id:: 6a52f976-5d51-47c5-a1e7-20b82541d37c
			- $V_y=\{y\neq0\}=\{[x:1]:x\in\mathbb C\}$.
		- Then:
			- These charts are isomorphic to $\mathbb C\times\mathbb C^\times$.
			- As in the first part, holomorphic vector bundles on $V_x$ and $V_y$ are trivial.
		- We then restrict the fibers to some small punctured disc $\Delta\setminus\{0\}$.
	- Try the AG description.
	  logseq.order-list-type:: number
		- We need to cover $\operatorname{Spec}(\mathbb C[u,v,w]/(uv=w^2))$ with
-