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
- ### If $k$ is infinite
- Let $d=\deg f$ be the total degree of $f$. Let $F_d$ be the highest-degree homogeneous part of $f$.
- Since $k$ is infinite and $F_d\neq0$, there are constants $u_1,\cdots,u_{n-1}\in k$ such that
  $$
  F_d(u_1,\cdots,u_{n-1},1) \neq 0.
  $$
- Put $b_i = a_i - u_i a_n$ for all $i<n$. We have $A=k[b_1,\cdots,b_{n-1},a_n]$.
- Now we have
  $$
  f(a_1,\cdots,a_n) = f(b_1+u_1a_n,\cdots,b_{n-1}+u_{n-1}a_n,a_n) = F_d(u_1,\cdots,u_{n-1},1)a_n^d + O(a_n^{d-1})
  $$
  as desired.
- ### For all $k$
- The following substitution works over any field $k$.
- Pick $N>d$. Define $b_i = a_i - a_n^{N^i}$ for $i<n$. Then $A=k[b_1,\cdots,b_{n-1},a_n]$ holds.
- If we fully expand $f$ using multi-indices,
  $$
  f = \sum_\alpha c_\alpha X^\alpha,
  $$
  then in $f(a_n^N,a_n^{N^2},\cdots,a_n^{N^{n-1}},a_n)$, every term has a distinct exponent.
-