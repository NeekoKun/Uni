#ELT 
```tikz
\usepackage{circuitikz}
\begin{document}

\begin{circuitikz}[american, voltage shift=0.5]
\draw (0,0) -- (2,0) -- (2,-2) -- (0,-2);
\draw (7,-2) -- (4,-2)
to[vcsource, invert, v_=$ri_1$] (4,0) -- (7,0);
\end{circuitikz}

\end{document}
```