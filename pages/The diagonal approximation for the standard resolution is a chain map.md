- The construction:
  $$\Delta_{n}:L_n \longrightarrow \bigoplus_{p=0}^n L_p\otimes L_{n-p}$$
- $$(g_0,\cdots,g_n) \longmapsto ((g_0,\cdots,g_p)\otimes(g_p,\cdots,g_n))_{p=0}^n$$
- Also recall that $\partial_n(g_0,\cdots,g_n)=\sum_{i=0}^n(-1)^i(g_0,\cdots,\hat{g_i},\cdots,g_n)$
- ## Goal
- We will check that $\Delta_\bullet$ is a chain homomorphism $L_\bullet \to L_\bullet \otimes L_\bullet$.
	- Recall that the tensor product is the total complex, following the Koszul sign rule.
- More precisely, we show the following equation.
- $$[\Delta_{n-1}\partial_n(g_0,\cdots,g_n)]_j = [\partial_n\Delta_n(g_0,\cdots,g_n)]_j \;\;\in L_j\otimes L_{n-1-j}$$
- ## LHS
- $$\begin{align*}
  \text{LHS} &= [\Delta_{n-1}\sum_{i}(-1)^i(g_0,\cdots,\hat{g_i},\cdots,g_n)]_j \\
  &= \sum_{i\leq j} (g_1,\cdots,\hat{g_i},\cdots,g_{j+1}) \otimes (g_{j+1},\cdots,g_n) + \sum_{i>j} (g_1,\cdots,g_j) \otimes (g_j,\cdots,\hat{g_i},\cdots,g_n) \\
  &=: S_1 + S_2 
  \end{align*}$$
- ## RHS
- $$\begin{align*}
  \text{RHS} &= [\partial_n\Delta_n(g_0,\cdots,g_n)]_j \\
  &= \partial^\vartriangleright[\Delta_n(g_0,\cdots,g_n)]_{j+1} 
  + (-1)^j \partial^\triangledown[\Delta_n(g_0,\cdots,g_n)]_j \\
  &= \partial(g_0,\cdots,g_{j+1}) \otimes (g_{j+1},\cdots,g_n)
  + (-1)^j (g_0,\cdots,g_j) \otimes \partial(g_j,\cdots,g_n) \\
  &=: T_1 + T_2
  \end{align*}$$
- Compute these two terms:
- $$\begin{align*}
  T_1 &= \sum_{i\leq j}(-1)^i(g_0,\cdots,\hat{g_i},\cdots,g_{j+1})\otimes(g_{j+1},\cdots,g_n) + (-1)^{j+1}(g_0,\cdots,g_j)\otimes(g_{j+1},\cdots,g_n) \\
  &=: S_1 + (-1)^{j+1}
  \end{align*}$$