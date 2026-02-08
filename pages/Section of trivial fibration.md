- Given a morphism of simplicial sets $p:X\to Y$ having the right lifting property against boundary inclusions $\partial\Delta^n\to\Delta^n$, we will find a section $s$ to $p$, and a homotopy $sp\simeq\mathrm{id}_X$.
- Recall the Eilenberg-Zilber lemma: every simplex has a unique expression as a degeneracy of a non-degenerate simplex.
- ### Construction of $s$
- Use induction on degree $n\geq0$. Suppose that $s$ is constructed for all simplices of degree $<n$ and commutes with all face and degeneracy maps between them. Let $\sigma$ be an $n$-simplex.
- If $\sigma$ is degerate, write $\sigma=Sz$ where $S$ is a composition of degeneracy maps and $z$ is non-degnerate, then simply put $s(\sigma)=Ss(z)$. This is well-defined by Eilenberg-Zilber. By definition $s$ commutes with all degeneracy maps. If $D$ is a composition of face maps, we have
- $$Ds(\sigma)=DSs(z)=S'D's(z)=s(S'D'z)=s(D\sigma).$$
- If $\sigma$ is non-degenerate, we find a lift by solving
  <!-- https://q.uiver.app/#q=WzAsNCxbMCwwLCJcXHBhcnRpYWxcXERlbHRhXm4iXSxbMSwwLCJYIl0sWzEsMSwiWSJdLFswLDEsIlxcRGVsdGFebiJdLFswLDNdLFszLDIsIlxcc2lnbWEiLDJdLFsxLDIsInAiXSxbMCwxLCJiIl0sWzMsMSwiIiwxLHsic3R5bGUiOnsiYm9keSI6eyJuYW1lIjoiZGFzaGVkIn19fV1d -->
  <iframe class="quiver-embed" src="https://q.uiver.app/#q=WzAsNCxbMCwwLCJcXHBhcnRpYWxcXERlbHRhXm4iXSxbMSwwLCJYIl0sWzEsMSwiWSJdLFswLDEsIlxcRGVsdGFebiJdLFswLDNdLFszLDIsIlxcc2lnbWEiLDJdLFsxLDIsInAiXSxbMCwxLCJiIl0sWzMsMSwiIiwxLHsic3R5bGUiOnsiYm9keSI6eyJuYW1lIjoiZGFzaGVkIn19fV1d&embed" width="200" height="200" style="border-radius: 8px; border: none;"></iframe>
- where the top map $b$ exists by induction hypothesis. This $s(\sigma)$ obviously commutes with taking faces. QED
- ### Construction of the homotopy
- This proof is very similar to the above, so we won't explain the treatment of degenerate simplices. We wish to find a map $h:\Delta^1\times X\to X$, such that
	- $h$ lifts the constant homotopy $\overline{h}=p\circ\mathrm{pr}_2$, i.e. $ph=\overline{h}$;
	  logseq.order-list-type:: number
	- $h(0)=sp$;
	  logseq.order-list-type:: number
	- $h(1)=\mathrm{id}_X$.
	  logseq.order-list-type:: number
- Induct on the degree $n\geq0$. Suppose $h$ is constructed for all simplices of degree $<n$ satisfying 1. and commutes with face and degeneracy.
- Given a non-degenerate $n$-simplex $\sigma$ not contained in $\partial\Delta^1\times X$, its faces are already constructed, and we're left with the extension problem
-