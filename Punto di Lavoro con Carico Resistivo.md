#ELT

```tikz
\usepackage{circuitikz}
\begin{document}

\begin{circuitikz}[american, voltage shift=0.5]
\draw (0,0)
to[isource, l=$I_0$, v=$V_0$] (0,3)
to[R=$R_S$] (4,3) -- (6,3)
to[R=$R_L$] (6,0) -- (0,0);
\draw (4,0) to[short, *-*, i=$v$] (4,3);
\end{circuitikz}

\end{document}
```

$P_{max}:\ \hat{v} = \dfrac{V_{s}}{2};\ \hat{i}=\dfrac{V_{S}}{2R_{S}}$