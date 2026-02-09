- Our goal is to define the three classes of special morphisms on $\mathsf{sSet}$, and check that they satisfies the axioms of a model category:
	- (M0) The category is complete and cocomplete;
	- (M1) all three classes are closed under retracts;
	- (M2) weak equivalences satisfies 2 out of 3;
	- (M3) acyclic cofibrations have the left lifting property against fibrations;
	- (M4) cofibrations have the left lifting property against acyclic fibrations;
	- (M5) every morphism can be factorized as an acyclic cofibration with a fibration;
	- (M6) every morphism can be factorized as a cofibration with an acyclic fibration.
- ### Definitions
- The cofibrations are the monomorphisms.
- The fibrations are the morphisms having right lifting property against the horn inclusions $\Lambda^n_k\to\Delta^n$.
- Kan complexes are the fibrant objects, equivalently, those with the horn filling property.
- A morphism $f:X\to Y$ is a weak homotopy equivalence iff, for every Kan complex $Z$, the induced map $f^*:[Y,Z]\to[X,Z]$ is a bijection.
- ## Checking the axioms
- ### Trivial things
- M0. This is known for presheaf categories.
- M2. Given $X\xrightarrow{f}Y\xrightarrow{g}Z$, any Kan complex $W$, we have $f^*g^*=(gf)^*$. Since bijections satisfy 2 out of 3, we're done.
- M1. This is easy for all three classes:
	- Retracts of monomorphisms are monomorphisms.
	- Retracts preserve all lifting properties. In particular, if $f$ has the right lifting property against some morphism $l$, then so does any retract of $f$. Hence fibrations are closed under retract.
	- Retracts are absolute, in particular, they are preserved by the functor $[-,W]$ where $W$ is any Kan complex. In $\mathsf{Set}$, retracts of bijections are bijections. Hence weak equivalences are closed under retract.
- ### M6: factorization into cofibration + acyclic fibration
  id:: 698606cb-087e-4eba-9bfc-d28b33011b70
- The following is called the small object argument with the set of inclusions $\{\partial\Delta^n\to\Delta^n\}_{n\geq 0}$.
- Let $f:X\to Y$ be a morphism of simplicial sets. Put $X(0)=X$. For $i\geq0$, let $\sigma$ run through all commutative squares of the form <!-- https://q.uiver.app/#q=WzAsNCxbMCwwLCJcXHBhcnRpYWxcXERlbHRhXm4iXSxbMSwwLCJYKGkpIl0sWzEsMSwiWSJdLFswLDEsIlxcRGVsdGFebiJdLFswLDNdLFszLDJdLFsxLDJdLFswLDFdXQ== -->
  <iframe class="quiver-embed" src="https://q.uiver.app/#q=WzAsNCxbMCwwLCJcXHBhcnRpYWxcXERlbHRhXm4iXSxbMSwwLCJYKGkpIl0sWzEsMSwiWSJdLFswLDEsIlxcRGVsdGFebiJdLFswLDNdLFszLDJdLFsxLDJdLFswLDFdXQ==&embed" width="200" height="200" style="border-radius: 8px; border: none;"></iframe>
- And define $X(i+1)$, as well as the map $X(i+1)\to Y$, by the pushout
  <!-- https://q.uiver.app/#q=WzAsNCxbMCwwLCJcXGNvcHJvZF97bixcXHNpZ21hfVxccGFydGlhbFxcRGVsdGFebiJdLFsxLDAsIlgoaSkiXSxbMSwxLCJYKGkrMSkiXSxbMCwxLCJcXGNvcHJvZF97bixcXHNpZ21hfVxcRGVsdGFebiJdLFswLDNdLFszLDJdLFsxLDJdLFswLDFdLFswLDIsIiIsMSx7InN0eWxlIjp7Im5hbWUiOiJjb3JuZXItaW52ZXJzZSJ9fV1d -->
  <iframe class="quiver-embed" src="https://q.uiver.app/#q=WzAsNCxbMCwwLCJcXGNvcHJvZF97bixcXHNpZ21hfVxccGFydGlhbFxcRGVsdGFebiJdLFsxLDAsIlgoaSkiXSxbMSwxLCJYKGkrMSkiXSxbMCwxLCJcXGNvcHJvZF97bixcXHNpZ21hfVxcRGVsdGFebiJdLFswLDNdLFszLDJdLFsxLDJdLFswLDFdLFswLDIsIiIsMSx7InN0eWxlIjp7Im5hbWUiOiJjb3JuZXItaW52ZXJzZSJ9fV1d&embed" width="200" height="200" style="border-radius: 8px; border: none;"></iframe>
- Let $X'=\varinjlim_iX(i)$. We have a factorization of $f$ as $X\hookrightarrow X'\xrightarrow{p} Y$. Then $p$ clearly has the right lifting property against the boundary embeddings $\partial\Delta^n\to\Delta^n$. To conclude, we need
- **Proposition**. A map $p:X\to Y$ is a trivial fibration if it has the right lifting property against the boundary embeddings.
- *Proof*. Since the horns $\Lambda^n_k$ are inside the boundary $\partial\Delta^n$, $p$ is clearly a fibration. To show that $p$ is a weak equivalence, we inductively find a section of $p$ which is a homotopy inverse. [Details of this step.]([[Section of trivial fibration]]) QED
- ### M4: cofibration lifts with acyclic fibration
- We must show the converse of the above proposition. The idea is to find a minimal fibration which is a deformation retract of our acyclic fibration $p$.
- LATER
  :LOGBOOK:
  CLOCK: [2026-02-09 Mon 10:05:24]
  :END:
- [ref](https://mat.uab.cat/~kock/crm/hocat/advanced-course/Quadern47.pdf)
- ### M5: factorization into acyclic cofibration + fibration
- This follows from a small object argument on the inclusions $\{\Lambda^n_k\to\Delta^n\}_{n,k}$.
- Denote the resulting factorization as $X\to X'\to Y$, then the second map is a fibration by construction. The first map is an acyclic cofibration because acyclic cofibrations are closed under pushout and transfinite composition.
- ### M3: acyclic cofibration lifts with fibration
-