- Let $X$ be a compact Kahler manifold.
- $c_1$ is a map from holomorphic line bundles to $2\pi i H^2(X,\Z)$, fitting into the exponential sequence:
- $$H^1(X,\mathcal O^\times) \xrightarrow{c_1} 2\pi i H^2(X,\Z) \xrightarrow{\iota_*} H^2(X,\mathcal O)$$
- induced by the SES $0 \to 2\pi i \Z \xrightarrow{\iota} \mathcal O \xrightarrow{\exp} \mathcal O^\times \to 0$.
- The Lefschetz theorem states that $c_1$ is surjection onto $2\pi i H^2(X,\Z)\cap H^{1,1}(X)$.
- Proof. By exactness and the Hodge decomposition, we need to show
	- if $\alpha\neq0$ is a (2,0)-form, then $\iota_*(\alpha)\neq 0$.
	  logseq.order-list-type:: number
	- if $\beta$ is a (1,1)-form, then $\iota_*(\beta)=0$.
	  logseq.order-list-type:: number
	- If $\gamma\neq0$ is a (0,2)-form, then $\iota_*(\gamma)\neq0$.
	  logseq.order-list-type:: number
- Since $c_1$ gives integral, in particular real, forms, we have symmetry between 1. and 3.
- Now, we compute $\iota$ by resolving using standard resolutions of $\underline{\mathbb C}$ and $\mathcal O$:
- <!-- https://q.uiver.app/#q=WzAsMTIsWzAsMCwiMCJdLFswLDEsIjAiXSxbMSwwLCJcXHVuZGVybGluZXsgXFxtYXRoYmIgQ30iXSxbMSwxLCJcXG1hdGhjYWx7T30iXSxbMiwwLCJcXE9tZWdhXjAiXSxbMywwLCJcXE9tZWdhXjEiXSxbNCwwLCJcXE9tZWdhXjIiXSxbNSwwLCJcXGNkb3RzIl0sWzIsMSwiXFxPbWVnYV57MCwwfSJdLFszLDEsIlxcT21lZ2FeezAsMX0iXSxbNCwxLCJcXE9tZWdhXnswLDJ9Il0sWzUsMSwiXFxjZG90cyJdLFswLDJdLFsxLDNdLFsyLDQsIiIsMCx7InN0eWxlIjp7InRhaWwiOnsibmFtZSI6Imhvb2siLCJzaWRlIjoidG9wIn19fV0sWzQsNSwiZCJdLFs1LDYsImQiXSxbNiw3XSxbOSwxMCwiXFxiYXJcXHBhcnRpYWwiLDJdLFs4LDksIlxcYmFyXFxwYXJ0aWFsIiwyXSxbMyw4LCIiLDAseyJzdHlsZSI6eyJ0YWlsIjp7Im5hbWUiOiJob29rIiwic2lkZSI6InRvcCJ9fX1dLFsxMCwxMV0sWzIsMywiXFxpb3RhIiwyXSxbNCw4LCJcXHBpXnswLDB9IiwyXSxbNSw5LCJcXHBpXnswLDF9IiwyXSxbNiwxMCwiXFxwaV57MCwyfSIsMl1d -->
  <iframe class="quiver-embed quiver" src="https://q.uiver.app/#q=WzAsMTIsWzAsMCwiMCJdLFswLDEsIjAiXSxbMSwwLCJcXHVuZGVybGluZXsgXFxtYXRoYmIgQ30iXSxbMSwxLCJcXG1hdGhjYWx7T30iXSxbMiwwLCJcXE9tZWdhXjAiXSxbMywwLCJcXE9tZWdhXjEiXSxbNCwwLCJcXE9tZWdhXjIiXSxbNSwwLCJcXGNkb3RzIl0sWzIsMSwiXFxPbWVnYV57MCwwfSJdLFszLDEsIlxcT21lZ2FeezAsMX0iXSxbNCwxLCJcXE9tZWdhXnswLDJ9Il0sWzUsMSwiXFxjZG90cyJdLFswLDJdLFsxLDNdLFsyLDQsIiIsMCx7InN0eWxlIjp7InRhaWwiOnsibmFtZSI6Imhvb2siLCJzaWRlIjoidG9wIn19fV0sWzQsNSwiZCJdLFs1LDYsImQiXSxbNiw3XSxbOSwxMCwiXFxiYXJcXHBhcnRpYWwiLDJdLFs4LDksIlxcYmFyXFxwYXJ0aWFsIiwyXSxbMyw4LCIiLDAseyJzdHlsZSI6eyJ0YWlsIjp7Im5hbWUiOiJob29rIiwic2lkZSI6InRvcCJ9fX1dLFsxMCwxMV0sWzIsMywiXFxpb3RhIiwyXSxbNCw4LCJcXHBpXnswLDB9IiwyXSxbNSw5LCJcXHBpXnswLDF9IiwyXSxbNiwxMCwiXFxwaV57MCwyfSIsMl1d&embed" width="200" height="200" style="border-radius: 8px; border: none;"></iframe>
- Since $d=\partial+\bar\partial$, commutativity is obvious. Hence $\iota_*$ at $H^2$ level is induced by $\pi^{0,2}$.
- This proves 2. and 3.