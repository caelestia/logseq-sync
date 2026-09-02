# Simplest definition (complex case)
- Let $E$ be a complex vector bundle on a topological space $X$.
- We can uniquely specify the total Chern class $c(E)\in H^\bullet(X,\Z)$ by the following set of axioms:
	- Naturality: If $f:Y\to X$, then $c(f^*E)=f^*c(E)$.
	  logseq.order-list-type:: number
	- Whitney sum formula. $c(E\oplus F)=c(E)\cup c(F)$.
	  logseq.order-list-type:: number
	- Normalization. We will specify the Chern class of line bundles now, in two equivalent definitions.
	  logseq.order-list-type:: number
- ## Line bundles (classification)
- Line bundles are classified by $BU(1)\simeq\mathbb{CP}^\infty$, whose cohomology ring is $\mathbb{Z}[T]$, where the generator $T$ has degree $2$.
	- One way to compute this: The Serre spectral sequence.
- If $L$ is a complex line bundle, pulling back $T$ along $\phi:X\to BU(1)$ to a cohomology class $H^2(X,\Z)$ defines the first Chern class $c_1(L):=\phi^*(T)$.
	- Set the total Chern class $c(L):=1+c_1(L)$.
- There is a small problem: we need to pick an "orientation", i.e. the generator $T\leftrightarrow-T$ has ambiguity. Generally we want $T$ to be the hyperplane divisor. The quick fix is to add the following.
	- $c_1(\mathcal{O}_{\mathbb{CP}^n}(1))=\text{PD}(H)$ for all $n\geq1$. But just having $n=1$ is enough.
- ## Line bundles (exponential sequence)
- On a complex manfold, $c_1$ is very easy to define. By
- $$0 \to 2\pi i\Z \to \mathcal{O}_X \to \mathcal{O}_X$$
- ## Chern roots
- By the splitting principle, we can pull back the vector bundle to some space, such that the induced homomorphism on cohomology is injective, and the vector bundle splits into line bundles.
- This defines the Chern roots of a rank $n$ bundle $E$, denoted $\alpha_1,\cdots,\alpha_n \in H^2(X,\Z)$.
	- The total Chern class is $c(E)=\prod_{i=1}^n(1+\alpha_i) \in H^\bullet(X,\Z)$.
	- The Chern character is $ch(E)=\sum_{i=1}^n e^{\alpha_i} \in H^\bullet(X,\mathbb Q)$. Note: This is rational.
- The basic properties, e.g. Chern classes of SES, tensor product and dual, all follows from computing the Chern roots.
- ---
- https://en.wikipedia.org/wiki/Chevalley_restriction_theorem