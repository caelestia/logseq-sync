### Lifting of symbol
- On a smooth manifold, the first order symbol (Atiyah) sequence is
  $$0\to\mathcal{A}\xrightarrow{\iota}\mathcal{D}^1\xrightarrow{\sigma}\mathcal{T}\to0$$
- This is a SES of locally free *right* $\mathcal{A}$-modules. The idea of a connection is closely related to the obstruction of writing a section $T$ of $\mathcal{D^1}$ into a sum $\iota(a)+\sigma(T)$.
	- Recall that $\mathcal{D}^1$ is the $\R$-linear endormorphisms of $\mathcal{A}$ satisfying $[T,f]=:\sigma(T)f\in\Gamma(\mathcal{A})$.
	- In local coordinates, $\mathcal{D}^1\simeq\mathcal{A}\oplus\mathcal{T}$, because we can exponentiate (i.e. parallel transport) a tangent vector at any point into a vector field around the point.
- A section $\nabla$ of $\sigma$ is a connection on the trivial line bundle.
	- The difference of two connections maps a tangent vector to a number, that is, a 1-form.
	-
- Tensor from the right by the dual of a locally free sheaf $\mathcal{E}^\vee$
  $$0\to\mathcal{A}\otimes\mathcal{E}^\vee\xrightarrow{\iota}\mathcal{D}^1\otimes\mathcal{E}^\vee\xrightarrow{\sigma}\mathcal{T}\otimes\mathcal{E}^\vee\to0$$
- A section $\nabla$ of $\sigma$ is a connection on $E$:
	- $\nabla:\mathcal{T}\to\mathcal{E\otimes D\otimes E}^\vee=:\mathcal{D}^1(\mathcal{E,E})$, such that $[\nabla_X,f]=\sigma(X)f=Xf\in\Gamma(\mathcal{A})$.
	-