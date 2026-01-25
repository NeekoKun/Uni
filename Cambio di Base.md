#GAL
> [!warning] Definizione
> Dato $L:V\to V$ [[Endomorfismi|Endorfismo]] con basi $B$ e $C$, definiamo il cambio di base come:
> $$M^{B,B}_{L} = M^{C, B}_{id_{V}} \cdot M^{C,C}_{L} \cdot M^{B,C}_{id_{V}}$$
> Infatti

 ```tikz
\usepackage{tikz-cd}
\usepackage{amssymb}
\begin{document}
\begin{tikzcd}[row sep=huge, column sep=huge,  cells={font=\huge}, arrows={line width=0.8pt}, labels={font=\large}]
	V \arrow[rrr, "L"] \arrow[ddd, "Q_B"] \arrow[dr, "id_V"] & & & V \arrow[ddd, "Q_B"] \\
	& V \arrow[r, "L"] \arrow[d, "Q_C"] & V \arrow[ur, "id_V"] \arrow[d, "Q_C"] & \\
	& \mathbb{R}^n \arrow[r, "M^{C,C}_L"] & \mathbb{R}^n \arrow[dr, "M^{C,B}_{id_V}"] & \\
	\mathbb{R}^n \arrow[ur, "M^{B,C}_{id_V}"] \arrow[rrr, "M^{B,B}_L"] & & & \mathbb{R}^n
\end{tikzcd}
\end{document}
```
> [!info] Osservazione
> $M^{B,B}_{id_{V}} e M^{C,C}_{id_{V}}$ sono quindi [[Matrici Simili]]