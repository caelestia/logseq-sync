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
- Claim that $\supp s''$ is proper over $(g')^{-1}(U)$.