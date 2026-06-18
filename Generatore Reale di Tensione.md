#ELT

## Output
$P_{u} = Vi = (V_{s} - Ri)i = V_{s}i - Ri^2$
Dove $V_{s}$ è la tensione del generatore ideale, $R$ è la resistenza del generatore reale

$$P_{max} = \frac{V_{S}^2}{4R_{S}}$$

$p_{s} = 2 \cdot p_{max};\ p_{u} = p_{max}  \implies \nu = \frac{p_{u}}{p_s} = \frac{p_{max}}{2p_{max}} = 50\%$


## Generatore di Tensione Reale
```tikz
\usepackage{circuitikz}
\begin{document}

\begin{circuitikz}[american, voltage shift=0.5]
\draw (6,0)
to[short, *-] (0,0)
to[vsource, v=$V_S$] (0,3)
to[R=$R_1$, -*, i>_=$i_1$] (6,3);
\draw (6,0) to[short, i=$V$] (6,3);
\end{circuitikz}

\end{document}
```

$$V = V_{S} - R_{1}i$$
## Generatore di Corrente Reale
```tikz
\usepackage{circuitikz}
\begin{document}

\begin{circuitikz}[american, voltage shift=0.5]
\draw (6,0)
to[short, *-] (0,0)
to[isource, v=$V_S$] (0,3) to[short, -*] (6,3);
\draw (6,0) to[short, i=$V$] (6,3);
\draw (3,0) to[R=$R_1$, *-*] (3,3);
\end{circuitikz}

\end{document}
```
#TODO in serie