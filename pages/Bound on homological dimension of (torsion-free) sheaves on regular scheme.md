- Let $X$ be a locally Noetherian regular scheme of finite dimension $\dim(X)\geq1$.
- At an arbitrary point $x\in X$, put
- $$R = \mathcal{O}_{X,x},\;\; d = \dim R.$$
- Recall the following facts:
	- $d\leq\dim(X)$.
	  logseq.order-list-type:: number
	- $R$ is a [UFD](https://stacks.math.columbia.edu/tag/0FJH).
	  logseq.order-list-type:: number
	- Noetherian regular local rings are Cohen-Macaulay, so $\operatorname{depth}(R) = d$.
	  logseq.order-list-type:: number
	- [We have](https://stacks.math.columbia.edu/tag/00OC) $\text{gl.dim}(R)=d$, i.e., for every $R$-module $M$ we have $\operatorname{pd}(M)\leq d$.
	  logseq.order-list-type:: number
- Now let $F$ be a coherent sheaf.
	- It immediately follows that
	- id:: 6a6f5160-f4fb-4af2-a7d2-02b67c95bb9d
	  $$\operatorname{hd}(F) = \max\{\operatorname{pd}(F_x):x\in X\} \leq \dim(X).$$
- Now suppose $F$ is torsion free. We will show that
- $$\operatorname{hd}(F) \leq \dim(X) - 1.$$
	- Proof. Fix $x\in X$. If $d=0$, $R$ is a field, and trivially $\text{gl.dim}=0$. So suppose $d\geq1$. Then we can pick some $a\in\mathfrak{m}_x$.
	- Since $R$ is a domain and $F_x$ is torsion-free, $a$ must be $F_x$-regular. In particular, we have
	- $$\operatorname{depth}(F_x) \geq 1.$$
	- By the