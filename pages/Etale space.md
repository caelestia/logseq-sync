- Let $X$ be a topological space, $\tau(X)$ be the category of open subsets. Let $\mathsf{Top}/X$ be the over category.
- *Fact*. $\mathsf{Top}/X$ is cocomplete. More precisely, the forgetful $\mathsf{Top}/X \to \mathsf{Top}$ creates colimits.
	- Proof. The universal property of colimits applies to the maps $\to X$ as well.
- **Definition**. The etale space functor $\mathrm{Et}:\mathsf{PSh}(X)\to\mathsf{Top}/X$ is the left Kan extension of the inclusion functor $\tau(X)\to\mathsf{Top}/X$ along the Yoneda embedding $\tau(X)\to\mathsf{PSh}(X)$.
- By the general theory about Yoneda embedding (abstract realization/nerve), $\mathrm{Et}$ has a right adjoint given by
  $$\underline{E}\mapsto\left[U\mapsto\operatorname{Hom}_{\mathsf{Top}/X}(\underline{U},\underline{E})\right]$$
  That is, the (pre)sheaf of continuous sections functor. The "nerve".
- To compute $\mathrm{Et}$, we have
  $$\mathrm{Et}(\mathcal{F})=\varinjlim_=\int^{U\in\tau(X)} U\times\mathcal{F}(U).$$
-