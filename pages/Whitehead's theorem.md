## Simplicial Sets
- ### Review of Kan complexes
- Definition. A Kan complex is a simplicial set where every horn has a filler.
	- [[Kan complexes are the fibrant objects]]
- For any topological space $X$, $\operatorname{Sing}_\bullet(X)$ is a Kan complex.
- The following lemmas won't be proven here.
	- Lemma 1. A Kan complex $X$ is contractible iff it is connected and $\pi_n(X,x)=1$ for every $n>0$ and every $x\in X$, iff $X\to\Delta^0$ is a trivial fibration.
		- [[Contractible Kan complexes]]
	- Lemma 2, Long exact sequence of fibration. If $(X,*)\to(Y,*)$ is a fibration of pointed Kan complexes, $(F,*)$ is the fiber over the base point, then $F$ is obviously a Kan complex and we have a long exact sequence
		- $$\cdots \rightarrow \pi _1(Y,*) \xrightarrow {\partial } \pi _{0}(F, *) \rightarrow \pi _0( X,*) \rightarrow \pi _0(Y,*).$$
- ### Weak homotopy equivalence
- Definition. Let $f:X\to Y$ be a morphism of simplicial sets. We say $f$ is a weak homotopy equivalence if, for every Kan complex $Z$, the induced map $[Y,Z]\to[X,Z]$ is a bijection.
- Theorem. Let $f:X\to Y$ be a morphism of Kan complexes. The following are equivalent:
	- (a) $f$ is a weak homotopy equivalence;
	- (b) $f$ is a homotopy equivalence;
	- (c) $\pi_0(f)$ is a bijection, and for every $x\in X$ and $n>0$, $\pi_n(f):\pi_n(X,x)\to\pi_n(Y,f(x))$ is an isomorphism.
- #### Proof.
- (a) implies (b) directly follows from the definition. Since $X$ is a Kan complex, by surjectivity of $[Y,X]\to[X,X]$, there is $g:Y\to X$ such that $gf\simeq\mathrm{id}_X$. Now $fgf\simeq\mathrm{id}_Y\circ f$, so by injectivity of $[Y,Y]\to[X,Y]$ (because $Y$ is a Kan complex), $fg\simeq\mathrm{id}_Y$.
- (b) implies (a) is obvious.
- (b) implies (c) is the homotopy invariance, which is clear since $\pi_n(-)=[S^n,-]$. For turning the homotopy equivalence into a pointed one, see [here](https://kerodon.net/tag/04GD). Note that this step requires $X,Y$ be Kan complexes.
- (c) implies (a). First, factor $f$ as $X\to Z\to Y$, where $X\to Z$ is a trivial cofibration and $Z\to Y$ is a fibration. Since $Z\to Y\to *$ is a fibration, $Z$ is a Kan complex. It remains to show that $g:Z\to Y$ is an acyclic fibration. By the two lemmas above, the fiber $F$ of $g$ over any base point is contractible.
- We need to solve the following lifting problem:
	- <!-- https://q.uiver.app/#q=WzAsNCxbMCwwLCJcXHBhcnRpYWxcXERlbHRhXm4iXSxbMCwxLCJcXERlbHRhXm4iXSxbMSwwLCJaIl0sWzEsMSwiWSJdLFsxLDMsIlxcc2lnbWEiLDJdLFsyLDMsImciXSxbMCwyLCJcXGJldGEiXSxbMCwxXSxbMSwyLCIiLDEseyJzdHlsZSI6eyJib2R5Ijp7Im5hbWUiOiJkYXNoZWQifX19XV0= -->
	  <iframe class="quiver-embed" src="https://q.uiver.app/#q=WzAsNCxbMCwwLCJcXHBhcnRpYWxcXERlbHRhXm4iXSxbMCwxLCJcXERlbHRhXm4iXSxbMSwwLCJaIl0sWzEsMSwiWSJdLFsxLDMsIlxcc2lnbWEiLDJdLFsyLDMsImciXSxbMCwyLCJcXGJldGEiXSxbMCwxXSxbMSwyLCIiLDEseyJzdHlsZSI6eyJib2R5Ijp7Im5hbWUiOiJkYXNoZWQifX19XV0=&embed" width="200" height="200" style="border-radius: 8px; border: none;"></iframe>
- For this, we use HELP to reduce to the case where $\sigma=c_y$, $y\in Y$. In details, since $\Delta^n$ is contractible, there is $y\in Y$ and a homotopy $\overline{h}:\Delta^1\times\Delta^n\to Y$ from $\sigma$ to some $c_y$. For $c_y$, the desired map $\Delta^n\to Z$ exists by contractibility of $F_y:=g^{-1}(y)$ (lemma 1). Denote this map as $u$. Next, we find a homotopy "on the walls" $k:\Delta^1\times\partial\Delta^n\to Z$, satisfying
	- logseq.order-list-type:: number
	  $$gk=\overline{h}_{\Delta^1\times\partial\Delta^n},$$
	- logseq.order-list-type:: number
	  $$k|_{\{0\}\times\partial\Delta^n}=\beta.$$
- Invoking HELP, we can then lift $\overline{h}$ to a homotopy $h:\Delta^1\times\Delta^n\to Z$ from some $h(0)$ to $u$, while also extending $k$. Such $h(0)$ is our desired lift of $\sigma$.
- Finally, the existence of $k$ is clear from the diagram:
- <!-- https://q.uiver.app/#q=WzAsNCxbMCwwLCJcXHswXFx9XFx0aW1lc1xccGFydGlhbFxcRGVsdGFebiJdLFswLDEsIlxcRGVsdGFeMVxcdGltZXNcXHBhcnRpYWxcXERlbHRhXm4iXSxbMSwwLCJaIl0sWzEsMSwiWSJdLFsxLDMsIlxcb3ZlcmxpbmUgaHxfe1xcdGV4dHt3YWxsc319IiwyXSxbMiwzLCJnIl0sWzAsMiwiXFxiZXRhIl0sWzAsMSwiIiwwLHsic3R5bGUiOnsidGFpbCI6eyJuYW1lIjoiaG9vayIsInNpZGUiOiJ0b3AifX19XSxbMSwyLCIiLDEseyJzdHlsZSI6eyJib2R5Ijp7Im5hbWUiOiJkYXNoZWQifX19XV0= -->
  <iframe class="quiver-embed" src="https://q.uiver.app/#q=WzAsNCxbMCwwLCJcXHswXFx9XFx0aW1lc1xccGFydGlhbFxcRGVsdGFebiJdLFswLDEsIlxcRGVsdGFeMVxcdGltZXNcXHBhcnRpYWxcXERlbHRhXm4iXSxbMSwwLCJaIl0sWzEsMSwiWSJdLFsxLDMsIlxcb3ZlcmxpbmUgaHxfe1xcdGV4dHt3YWxsc319IiwyXSxbMiwzLCJnIl0sWzAsMiwiXFxiZXRhIl0sWzAsMSwiIiwwLHsic3R5bGUiOnsidGFpbCI6eyJuYW1lIjoiaG9vayIsInNpZGUiOiJ0b3AifX19XSxbMSwyLCIiLDEseyJzdHlsZSI6eyJib2R5Ijp7Im5hbWUiOiJkYXNoZWQifX19XV0=&embed" width="200" height="200" style="border-radius: 8px; border: none;"></iframe>
- If the left map is an acyclic cofibration, then the dashed arrow exists. But it's clearly a cofibration and a homotopy equivalence, so everything follows from *(b) implies (a)*. QED
- ## Topological spaces
- Definition. A morphism $f:X\to Y$ of topological spaces is a weak homotopy equivalence if $\pi_0(f)$ is a bijection, and for every $x\in X$ and $n>0$, $\pi_n(f):\pi_n(X,x)\to\pi_n(Y,f(x))$ is an isomorphism.
- From the adjunction pair $|\cdot|\dashv\operatorname{Sing}$, it is easy to show that
	- $$\pi_n(X,A):=[(|\Delta^n|,|\partial\Delta^n|),(X,A)]=[(\Delta^n,\partial\Delta^n),(\operatorname{Sing}(X),\operatorname{Sing}(A))]$$
- Hence $\pi_n(X,x)\simeq\pi_n(\operatorname{Sing}(X),x)$ naturally for all $n>0$. Same for $\pi_0$.
- By the last section, we have $f$ is a weak homotopy equivalence
	- $\Longleftrightarrow$ $\operatorname{Sing}(f)$ is a weak homotopy equivalence 
	  $\Longleftrightarrow$ $\operatorname{Sing}(f)$ is a homotopy equivalence
- ### Whitehead's theorem
- Theorem (Whitehead). If $f:X\to Y$ is a weak homotopy equivalence and $X,Y$ are homotopy equialent to CW complexes, then $f$ is a homotopy equivalence.
-