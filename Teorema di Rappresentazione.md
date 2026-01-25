#GAL 
> [!error] Teorema
> $L: V \to W$ [[Applicazioni Lineari|Applicazione Lineare]] dove:
> - $B = \{ \underline{b}_{1},\dots,\underline{b}_{n} \}$ base di $V$
> - $C = \{ \underline{w}_{1}, \dots, \underline{w}_{m} \}$ base di $W$
> - $A = M_{L}^{B, C} = \{ [L(\underline{b}_{1})]_{C}, \dots, [L(\underline{b}_{n})]_{C} \}$
> 
> Il diagramma commuta: $\boxed{Q_{C} \circ L = T_{A} \circ Q_{B}}$

> [!error] Dimostrazione
> Sia $\underline{v} \in V$, dobbiamo dimostrare $Q_{A} \circ L = T_{A}(\underline{v}) \circ Q_{B}(\underline{v})$
> Scriviamo $\underline{v} = c_{1} \underline{b}_{1} + \dots + c_{n}\underline{b}_{n}$ dove $[\underline{v}]_{B} = \begin{pmatrix}c_{1} \\ \vdots \\ c_{n} \end{pmatrix} \in \mathbb{R}^n$
> Calcoliamo $L(\underline{v})$:
> $$L(\underline{v}) = L(c_{1}\underline{b}_{1} + \dots + c_{n}\underline{b}_{n}) = c_{1}L(\underline{b}_{1}) + \dots + c_{n}L(\underline{b}_{n})$$
> $$Q_{C}(L(\underline{v})) = Q_{C}(c_{1}L(\underline{b}_1) + \dots + c_{n}L(\underline{b}_{n})) = c_{1}Q_{C}(L(\underline{b}_{1})) + \dots + c_{n}Q_{C}(L(\underline{b}_{n}))$$
> $$= c_{1}[L(\underline{b}_{1})]_{C} + \dots + c_{n}[L(\underline{b}_{n})]_{C}$$
> Che è una combinazione lineare delle colonne di $A$, quindi:
> $$Q_{C}(L(\underline{v})) = A \cdot \begin{pmatrix}c_{1} \\ \vdots \\ c_{n}\end{pmatrix} = T_{A}(Q_{B}(\underline{v})) = T_{A} \circ Q_{B}(\underline{v})$$

```tikz
\usepackage{tikz-cd}
\usepackage{amssymb}

\begin{document}
\begin{tikzcd}[row sep=huge, column sep=huge,  cells={font=\huge}, arrows={line width=0.8pt}, labels={font=\large}]
	V \arrow[r, "L"] \arrow[d, "Q_B"] & W \arrow[d, "Q_C"] \\
	\mathbb{R}^n \arrow[r, "T_A"] & \mathbb{R}^m
\end{tikzcd}
\end{document}
```
## Corollari
> [!error] Corollario
> Anche il diagramma arricchito di $P_{B}$ e $P_{C}$, Mappe di Coordinate, commuta. dove:
> $$L = P_{C} \circ T_{A} \circ Q_{B}$$
> $$T_{A} = Q_{C} \circ L \circ P_{B}$$
> $$L \circ P_{B} = PC \circ T_{A}$$
> etc.

> [!error] Dimostrazione
> Segue dal **Teorema** e dal fatto che $Q_{B}, P_{B}$ e $Q_{C}, P_{C}$ sono inverse:
> Dal [[Teorema di Rappresentazione]]: 
> $$Q_{C} \circ L = T_{A} \circ Q_{B}$$
> $$P_{C} \circ Q_{C} \circ L = P_{C} \circ T_{A} \circ Q_{B}$$
> ma $P_{C} = Q_{C}^{-1}$, quindi:
> $$\boxed{L = P_{C} \circ T_{A} \circ Q_{B}}$$
```tikz
\usepackage{tikz-cd}
\usepackage{amssymb}

\begin{document}
\begin{tikzcd}[row sep=huge, column sep=huge,  cells={font=\huge}, arrows={line width=0.8pt}, labels={font=\large}]
	V \arrow[r, "L"] \arrow[d, shift left, harpoon, "Q_B"]
	& W \arrow[d, shift left, harpoon, "Q_C"] \\
    \mathbb{R}^n \arrow[r, "T_A"] \arrow[u, shift left, harpoon, "P_B"]
    & \mathbb{R}^m \arrow[u, shift left, harpoon, "P_C"]
\end{tikzcd}
\end{document}
```


---

> [!error] Corollario (Applicazioni Lineari e Matrici)
> 1. $\mathrm{Ker}(L) = P_{B}(\mathrm{Ker}(A)) \Leftrightarrow \mathrm{Ker}(A) = Q_{B}(\mathrm{Ker}(L))$
> 2. $\Im(L) = P_{C}(\mathrm{col}(A))$
> 3. $\mathrm{dim}(\mathrm{Ker}(L)) = \mathrm{dim}(V) - \mathrm{rK}(A)$
> 4. $\mathrm{dim}(\Im(L)) = \mathrm{rK}(A)$
> 5. [[Teorema di Nullità + Rango]] per [[Applicazioni Lineari]]: 
> 	$\mathrm{dim}(\Im(L)) + \mathrm{dim(Ker(L)) = \mathrm{dim}(V)}$
> 6. $L$ è iniettiva $\Leftrightarrow \mathrm{rK}(A) = \mathrm{dim}(V)$
> 7. $L$ è suriettiva $\Leftrightarrow \mathrm{rK}(A) = \mathrm{dim}(W)$
> 8. $L$ è isomorfismo $\Leftrightarrow \mathrm{rK}(A) = \mathrm{dim}(W) = \mathrm{dim}(V)$
> 9. $\mathrm{dim}(V) < \mathrm{dim}(W) \implies L$ non è suriettiva
> 10. $\mathrm{dim}(V) > \mathrm{dim}(W) \implies L$ non è iniettiva

> [!error] Dimostrazione
> Seguono tutti da 1. e 2., quindi basta dimostrare quei due:
> 1. $\underline{v} \in \mathrm{Ker}(L) \Leftrightarrow L(\underline{v}) = \underline{0} \in W \underset{Q_{C} \text{ isomorfismo}}{\Leftrightarrow} Q_{C}(L(\underline{v})) = Q_{C}(\underline{0}) = \underline{0} \in \mathbb{R}^m$
> $\Leftrightarrow T_{A}(Q_{B}(\underline{v})) = \underline{0} \in \mathbb{R}^m \Leftrightarrow Q_{B}(\underline{v}) \in \mathrm{Ker}(T_{A}) = \mathrm{Ker}(A) \Leftrightarrow \underline{v} \in P_{B}(\mathrm{Ker}(A))$

---
> [!error] Corollario (Rappresentazione della Composizione)
> $V, W, U$ [[Spazi Vettoriali]]
> $B, C, D$ Rispettive [[Base|Basi]]
> $L:V \to W, N : W \to U$ [[Applicazioni Lineari]]

```tikz
\usepackage{tikz-cd}
\usepackage{amssymb}

\begin{document}
\begin{tikzcd}[row sep=huge, column sep=huge,  cells={font=\huge}, arrows={line width=0.8pt}, labels={font=\large}]
	  V \arrow[r, "L"] \arrow[rr, bend left, "L \circ N"] \arrow[d, shift left, harpoon, "Q_B"]
	& W \arrow[r, "N"] \arrow[d, shift left, harpoon, "Q_C"]
	& U \arrow[d, shift left, harpoon, "Q_D"] \\
      \mathbb{R}^n \arrow[r, "T_A"] \arrow[rr, bend right, "T_A \circ T_B"'] \arrow[u, shift left, harpoon, "P_B"]
    & \mathbb{R}^m \arrow[r, "T_B"] \arrow[u, shift left, harpoon, "P_C"]
    & \mathbb{R}^p \arrow[u, shift left, harpoon, "P_D"]
\end{tikzcd}
\end{document}
```