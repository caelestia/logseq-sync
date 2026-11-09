- Let $k$ be a field.
- Theorem. If $A=k[a_1,\cdots,a_n]$ is a finitely generated $k$-algebra and a domain, then $A$ is finite over some $k[x_1,\cdots,x_m]$ where $x_1,\cdots,x_m$ are algebraically independent.
- ## Proof
- ### Idea
- If the generators $a_1,\cdots,a_n$ are alg. indep., there is nothing to prove. So we assume they satisfy a polynomial
  $$f(a_1,\cdots,a_n) = 0.$$
- We would like to deduce that $f$ is monic in $a_n$, i.e. of the form
  $$
  a_n^d + g_{d-1}(a_1,\cdots,a_{n-1}) a_n^{d-1} + \cdots + g_0(a_1,\cdots,a_{n-1}) = 0.
  $$
- By induction on $n$, we can assume $k[a_1,\cdots,a_{n-1}]$ is integral over some polynomial ring. Then $a_n$ is integral over the same ring, and we win.
- So the key step is to perform some change of variables so $f$ becomes monic in $a_n$.
- ### Infinite field
- Let $d=\deg f$ be the total degree of $f$. Let $F_d$ be the highest-degrere