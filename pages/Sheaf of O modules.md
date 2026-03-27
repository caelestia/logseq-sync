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
	- Proof. The $\mathcal{O}$-action can be safely ignored for this (this falls into the general rule that forgetful base change admits both a left and a right adjoint). Hence all limits and colimits are computed in the category $\mathsf{Sh}(\mathsf{Ab})$, i.e., computed component-wise and sheafify for colimits.  QED
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
- ## Grothendieck category
- **Proposition.** $\mathcal{O}\text{--}\mathsf{Mod}$ is a Grothendieck category, i.e., it's cocomplete and admits a generator, and filtered colimits are exact.
	- Proof. Taking stalks of a presheaf commutes with taking filtered colimits, and sheafification does not change the stalks. Hence filtered colimits are exact. To find a generator, we construct a generating family $\{\mathcal{F}_U\}_{U}$ and take $G=\bigoplus_U\mathcal{F}_U$ by cocompleteness. Let $\mathcal{F}_U=i_{U!}\mathcal{O}|_U$ be the extension by $0$ of the restriction of $\mathcal{O}_X$. By the adjunction $i_{U!} \dashv i_U^{-1}$, we get
	- $$\operatorname{Hom}_{\mathcal{O}_X}(\mathcal{F}_U,\mathcal{G})=\operatorname{Hom}_{\mathcal{O}|_U}(\mathcal{O}|_U,\mathcal{G}|_U)=\mathcal{G}(U)$$
	- Indeed, if $\mathcal{G}(U)=0$ for all $U$, then $\mathcal{G}=0$. This proves our claim. QED
- It follows formally that $\mathcal{O}\text{--}\mathsf{Mod}$ has enough injectives (Tohoku paper). This is due to Baer's critetion: $\mathcal{I}$ is injective iff $\mathcal{I}\to0$ has right lifting property against subobjects of $G$, and an application of the small object argument.
- Another way to construct injectives is this. If $\mathcal{F}$ is any $\mathcal{O}$-module, there is a canonical flasque resolution (induction), given by $\mathcal{F}_{\text{God}}:U\mapsto\prod_{x\in U}\mathcal{F}_x$. We can further embed this in $U\mapsto\prod_{x\in U}I_x$ where $I_x$ is an injective $\mathcal{O}_x$-module.