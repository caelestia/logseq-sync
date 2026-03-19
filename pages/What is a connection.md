### Splitting of symbol sequence
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
	- That is, the Leibniz rule $\nabla_X(fs)=f\nabla_Xs+Xf\otimes s$.
	- Thus the symbol of $\nabla_X$ is $X\otimes\mathrm{id}_\mathcal{E}$.
- ### Lifting of symbol
- If we view the connection as a smooth section of $\mathcal{D^1(E,T^*\otimes E)}$, then it's symbol (viewed as an element of $\operatorname{Hom}(\mathcal{T^*\otimes E,T^*\otimes E})$ via the natural isomorphsim) is $\mathrm{id}_{\mathcal{T^*\otimes E}}$.
	- To see this,
- ### Vertical and horizontal spaces
- A connection is equivalently a splitting of the tangent bundle of the total space $E$:
  $$T_E = V \oplus H$$
- Let $e\in E$, $x:=\pi(e)$, where $\pi:E\to M$ is the projection. The *vertical space* $V_e:=\ker(d\pi)_e$ at $e$. Clearly, this is canonically isomorphic to the vector space $\pi^{-1}(x)$. We have the SES
  $$0 \longrightarrow V_e \longrightarrow T_{E,e} \xrightarrow{d\pi_e} T_{M,x} \longrightarrow 0$$
- Thus there are two ways to obtain the splitting:
	- We can define a section of $d\pi_e$. This amounts to finding a local section that's parallel at $x$.
	- We can also find a projection $T_{E,e}\to V_e$.
- To show that $H$ is a subbundle of $T_E$,