- #+BEGIN_CENTER
  ![](../assets/tikz/proper-base-change.svg){:height 199, :width 186}
  #+END_CENTER
- Thm. If the square is a Cartesian square, then there is a natural isomorphism
  $$
  (g')^{-1} f_! \longto f'_! g^{-1}.
  $$
- ## Proof
- ### Step 1
- We construct a natural transformation
  $$
  f_! g_* \longto g'_* f'_!
  $$
- Take a section $s\in\Gamma(U,f_!g_* \mc F)$ where $U\subset Y$.
- By definition, $s$ is also a section $s'\in\Gamma(f^{-1}(U),g_*\mc F)$ which has support proper over $U$.
- It's further equivalent to a section $s'' \in \Gamma(g^{-1}f^{-1}(U),\mc F) = \Gamma((f')^{-1}(g')^{-1}(U),\mc F)$.
- Observe that $g(\supp s'') \subset \supp s'$.
	- Say $x\in \supp s''$. Then the stalk of $g_*\mc F$ at $g(x)$ is given by the filtered colimit $\varinjlim_{V\ni x}\Gamma(g^{-1}(V),\mc F)$, so if $s'_{g(x)}=0$ in the colimit, such equality holds already for some $V$, which is impossible for $s''_x\neq0$.
- I claim that $\supp s'' \subset g^{-1}(\supp s')$ is proper over $(g')^{-1}(U)$. Indeed, we have the Cartesian square
- #+BEGIN_CENTER
  ![](../assets/tikz/proper-base-change-proof.svg){:height 135, :width 236}
  #+END_CENTER
- obtained by replacing $X$ with the closed subset $\supp s'$. Since the right arrow is proper, so is the left arrow.
- Thus we obtain a section over $(g')^{-1}(U)$ of $f'_!\mc F$. This gives the desired map.
- ### Step 2
- We construct the base change natural transformation
  $$
  (g')^{-1} f_! \longto f'_! g^{-1}.
  $$
- Start with the unit $\id_{\msf{Sh}(X,k)} \longto g_*g^{-1}$.
- Compose with $f_!$, we get $f_! \longto f_! g_* g^{-1}$.
- Compose with the natural transformation constructed in Step 1, we get $f_! \longto g'_* f'_! g^{-1}$.
- Compose with $(g')^{-1}$ and compose with the counit, we get $(g')^{-1}f_! \longto (g')^{-1}g'_* f'_! g^{-1} \longto f'_! g^{-1}$.
- ### Step 3
-