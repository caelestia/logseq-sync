- https://amathew.wordpress.com/2012/02/18/the-bochner-technique/
- [[Linear algebra of Hodge theory]]
- [[Definition of Kahler manifold]]
- [[Kahler identities]], [[Nakano identities]]
- [[Vanishing theorems]]
- [[Kodaira Embedding Theorem]]
- {{renderer code_diagram,tex}}
	- ```tikz
	  \usepackage{tikz}
	  \usetikzlibrary{positioning}
	  \begin{document}
	  \begin{tikzpicture}[
	  roundnode/.style={circle, draw=green!60, fill=green!5, very thick, minimum size=7mm},
	  squarednode/.style={rectangle, draw=red!60, fill=red!5, very thick, minimum size=5mm},
	  ]
	  %Nodes
	  \node[squarednode]      (maintopic)                              {2};
	  \node[roundnode]        (uppercircle)       [above=of maintopic] {1};
	  \node[squarednode]      (rightsquare)       [right=of maintopic] {3};
	  \node[roundnode]        (lowercircle)       [below=of maintopic] {4};
	  
	  %Lines
	  \draw[->] (uppercircle.south) -- (maintopic.north);
	  \draw[->] (maintopic.east) -- (rightsquare.west);
	  \draw[->] (rightsquare.south) .. controls +(down:7mm) and +(right:7mm) .. (lowercircle.east);
	  \end{tikzpicture}
	  \end{document}
	  
	  ```
	-