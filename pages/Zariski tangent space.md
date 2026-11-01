- Let $X$ be a scheme, $x\in X$. Let $k$ be the residue field at $x$.
- There are two equivalent definitions of the tangent space at $x$:
	- $T_xX := \mathrm{Der}( \mathcal{O}_{X,x},k) \simeq (\mathfrak{m}_{x}/\mathfrak{m}_{x}^2)^\vee$, which is a $k$-vector space.
	  logseq.order-list-type:: number
	- $T_xX := \big[X(k[\varepsilon])\overset{\,\varepsilon\mapsto0\,}{\longrightarrow} X(k)\big]^{-1}x$, where $k[\varepsilon]:=k[\varepsilon]/(\varepsilon^2)$.
	  logseq.order-list-type:: number
- We now explain how to obtain the $k$-vector space on the second definition.
	- The scalar multiplication is clear.
	- To get addition, let $R := k[\varepsilon_1] \times_k k[\varepsilon_2]$. Indeed, its elements are of the form $(a+b\varepsilon_1,a+c\varepsilon_2)$, so
	- $$R \simeq k[\varepsilon_1,\varepsilon_2]/(\varepsilon_1^2,\varepsilon_2^2,\varepsilon_1\varepsilon_2).$$
	- Now by definition of the fiber product (in Set), $T_xX \times T_xX$ has a natural morphism into $\big[X(R)\longrightarrow X(k)\big]^{-1}x$.
	- Now addition is induced by the ring homomorphism
	- $R \longrightarrow k[\varepsilon]$, given by $\varepsilon_1 \mapsto \varepsilon$ and $\varepsilon_2 \mapsto \varepsilon$.