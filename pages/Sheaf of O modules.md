- Fix a topological space $X$. Let $\mathcal{O}$ be a sheaf of commutative rings.
- A sheaf of abelian groups $\mathcal{M}$ is called a sheaf of $\mathcal{O}$-modules if $\mathcal{M}(U)$ has a $\mathcal{O}(U)$-module structure, and for every $U\supset V$, the diagram
  $$$$\begin{array}{ccc}
  \mathcal{O}(U) \otimes \mathcal{M}(U) & \longrightarrow & \mathcal{M}(U) \\
  \downarrow & & \downarrow \\
  \mathcal{O}(V) \otimes \mathcal{M}(V) & \longrightarrow & \mathcal{M}(V)
  \end{array}$$$$
  of abelian groups commutes.
- ## Sheafification
- From the above definition we also get the notion of a presheaf of $\mathcal{O}$-modules.
- We want to establish the usual adjoint pair $\text{sheafification}\dashv\text{inclusion}$.
- **Lemma.** If $\mathcal{M}$ is a presheaf of $\mathcal{O}$-modules, then $\mathcal{M}_x$ is an $\mathcal{O}_x$-module.
	- Proof. In $\mathsf{Ab}$, filtered colimit preserves finite products. Result follows from above diagram.
- Then an action $\mathcal{O}(U)\curvearrowright\mathcal{M}^+(U)$ is defined. Indeed,
  $$\mathcal{M}^+(U)=\{(m_x\in\mathcal{M}_x)_{x\in U}:\text{locally induced by sections}\}.$$
  Hence, we can sheafify a presheaf of $\mathcal{O}$-modules and get a sheaf of $\mathcal{O}$-modules.
- ## Abelian & Closedness
- **Lemma.** $\mathcal{O}\text{--}\mathsf{Mod}$ admits all small limits and colimits.
	- Proof. The $\mathcal{O}$-action can be safely ignored for this (this falls into the general rule that forgetful base change admits both a left and a right adjoint). Hence all limits and colimits are computed in the category $\mathsf{Sh}(\mathsf{Ab})$, i.e., compute component-wise and sheafify for colimits.  QED
- **Lemma.** $\mathcal{O}\text{--}\mathsf{Mod}$ is an Abelian category.
	- Proof. Obvious.
- Next, we define the tensor product. Let's first review that in $R\text{--}\mathsf{Mod}$. The tensor product of two modules $M,N$ is the coequalizer of the diagram in $\mathsf{Ab}$
  $$M\otimes R\otimes N \rightrightarrows M\otimes N.$$
- Given $\mathcal{O}$-modules $\mathcal{M}$ and $\mathcal{N}$, the tensor product is defined as the coequializer of the analogous diagram in $\mathsf{Sh(Ab)}$, or in other words, the sheafification of the presheaf $U\mapsto \mathcal{M}(U)\otimes_{\mathcal{O}(U)}\mathcal{N}(U)$.
- **Lemma.** $(\mathcal{M\otimes_ON})_x=\mathcal{M}_x\otimes_{\mathcal{O}_x}\mathcal{N}_x$.
	- Proof. The coequializer diagram commutes with filtered colimits. QED
- The category $\mathcal{O}\text{--}\mathsf{Mod}$ also admits internal Hom. This is not just for modules, but a general fact for sheaves taking value in any category. Given two sheaves $\mathcal{F,G}$, define
  $$\mathcal{Hom(F,G)}(U)=\operatorname{Hom}_{\text{Sheaf}(U)}(F|_U,G|_U),$$
  which is automatically a sheaf by locality & patching of sheaf morphisms.
- However, there is a catch. In general, $\mathcal{Hom(F,G)}_x$ will be different from $\operatorname{Hom}_{\mathcal{O}_x}(\mathcal{F}_x,\mathcal{G}_x)$.
- **Proposition.** There is a canonical map $\mathcal{Hom_O(M,N)}_x\to\operatorname{Hom}_{\mathcal{O}_x}(\mathcal{M}_x,\mathcal{N}_x)$. This is injective if $\mathcal M$ is of finite type, and is an isomorphism if $\mathcal M$ is locally finitely presented.
	- Proof. Restricting $X$ to open subsets, consider an exact sequence
	  $$\mathcal{K}\longrightarrow\bigoplus_{i=1}^n\mathcal{O}\longrightarrow\mathcal{M}\longrightarrow0$$
	- Apply $\mathcal{Hom(-,N)}$ and taking stalks, we get
	  $$0\longrightarrow\mathcal{Hom(M,N)}_x\longrightarrow\bigoplus_{i=1}^n\mathcal{N}_x\longrightarrow\mathcal{Hom(K,N)}_x\tag{1}$$
	- On the other hand, we have
	  $$0\longrightarrow\operatorname{Hom}_{\mathcal{O}_x}(\mathcal{M}_x,\mathcal{N}_x)\longrightarrow\bigoplus_{i=1}^n\mathcal{N}_x\longrightarrow\operatorname{Hom}_{\mathcal{O}_x}(\mathcal{K}_x,\mathcal{N}_x)\tag{2}$$
	- And a map from sequence (1) to (2). The result follows. QED
- **Lemma.** $\mathcal{O}\text{--}\mathsf{Mod}$ is a closed symmetric monoidal category with tensor product and internal Hom described above.
	- Proof. We can check
	- $$\mathcal{Hom}\mathcal{(F\otimes G,H)} \simeq \mathcal{Hom}\mathcal{(F,Hom(G,H))}.$$
	- QED
-