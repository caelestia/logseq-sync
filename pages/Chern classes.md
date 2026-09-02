# Simplest definition (complex case)
- We can uniquely specify the total Chern class by the following set of axioms:
	- Natu
	  logseq.order-list-type:: number
- ## Line bundle
- This is the base case. Line bundles are classified by $BU(1)\simeq\mathbb{CP}^\infty$, whose cohomology ring is $\mathbb{Z}[T]$, where the generator $T$ has degree $2$.
	- One way to compute this: The Serre spectral sequence.
- If $L$ is a complex line bundle, pulling back $T$ along $\phi:X\to BU(1)$ to a cohomology class $H^2(X,\Z)$ defines the first Chern class $c_1(L):=\phi^*(T)$.
	- Set the total Chern class $c(L):=1+c_1(L)$.
- ## Chern roots
- By the splitting principle, we can pull back the vector bundle to some space, such that the induced homomorphism on cohomology is injective, and the vector bundle splits into line bundles.
- This defines the Chern roots of a rank $n$ bundle $E$, denoted $\alpha_1,\cdots,\alpha_n \in H^2(X,\Z)$.
	- The total Chern class is $c(E)=\prod_{i=1}^n(1+\alpha_i) \in H^\bullet(X,\Z)$.
	- The Chern character is $ch(E)=\sum_{i=1}^n e^{\alpha_i} \in H^\bullet(X,\mathbb Q)$. Note: This is rational.
-