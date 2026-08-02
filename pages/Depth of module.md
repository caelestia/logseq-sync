# Basic definitions
- Let $R$ be a ring, $M$ be an $R$-module.
- Regular sequences.
	- Let $x_1,\cdots,x_n\in R$, and let $M_i := M/( x_1,\cdots,x_i ) M$.
	- We say that the sequence $x_1,\cdots,x_n$ is $M$*-regular*, if $M_n\neq0$ and for every $i$, $x_i$ is not a zero-divisor on $M_{i-1}$.
- Let $I\subset R$ be an ideal. If every $x_i\in I$ we say $x_1,\cdots,x_n$ is an $M$-regular sequence in $I$.
	- For a local ring (which is what we usually assume), a regular sequence is the same as a regular sequence in $\mathfrak{m}$.
- Depth.
	- There is a technicality here. We have two cases.
		- When $IM\neq M$, the $I$-*depth* of $M$, $\text{depth}_I(M)$ is the maximal length of $M$-regular sequences in $I$.
		- When $IM=M$, define $\text{depth}_I(M):=\infty$.
	- For $R$ local, this problem does not exist by Nakayama, and we put $\text{depth}(M)=\text{depth}_\mathfrak{m}(M)$.
- # Characterization by Ext groups
- Let $(R,\mathfrak m,k)$ be a Noetherian local ring and let $M\neq0$ be finitely generated. We have
- $$\operatorname{depth}(M)
  =
  \inf\{i\ge 0:\operatorname{Ext}^i_R(k,M)\neq 0\}.$$
- We prove this by induction. This base case is more interesting.
- ## Base case
-
-
-
- Auslander–Buchsbaum.
- Serre's conditions.