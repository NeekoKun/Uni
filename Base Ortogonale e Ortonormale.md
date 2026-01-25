#GAL
> [!warning] Definizione (Ortogonale)
> Sia $H \subseteq V$ un [[Sottospazio Vettoriale]], $B = \{ \underline{b}_{1}, \dots, \underline{b}_{d} \}$ base di $H$
> - $B$ è una **Base Ortogonale** di $H$ se $<\underline{b}_{i}, \underline{b}_{j}> = 0\ \forall\ i \neq j$

> [!warning] Definizione (Ortonormale)
> Sia $H \subseteq V$ un [[Spazi Vettoriali]], $B = \{ \underline{b}_{1}, \dots, \underline{b}_{d} \}$ base di $H$
> - $B$ è una **Base Ortonormale** di $H$ se $B$ è una Base Ortogonale di $H$ e $||\underline{b}_{i}|| = 1\ \forall\ i$

## Normalizzazione
> [!info] Osservazione 
> Dividendo ogni vettori di una **Base Ortogonale** per la propria norma,, otteniamo una **Base Ortonormale**

> [!error] Proposizione (Coordinate rispetto ad una Base Ortogonale)
> Sia $B = \{ \underline{b}_{1}, \dots, \underline{b}_{n} \}$ base ortonormale di uno [[Spazi Euclidei|Spazio Euclideo]] V. Per ogni $\underline{v} \in V$ allora 
> $$[\underline{v}]_{B} = \begin{pmatrix} <\underline{v}, \underline{b}_{1}> \\ \vdots \\ <\underline{v}, \underline{b}_{n}> \end{pmatrix}$$
> Cioè $\underline{v} = \sum_{i=1}^{n} <\underline{v}, \underline{b}_{i}>\underline{b}_{i}$

> [!error] Dimostrazione
> Sia $[\underline{v}]_{B} = \begin{pmatrix}c_{1} \\ \vdots \\ c_{n}\end{pmatrix} \in \mathbb{R}^n$, cioè $\underline{v} = \sum_{i=1}^{n}c_{i}\underline{b}_{i}$
> Per ogni $j$
> $$<\underline{v}, \underline{b}_{j}> = <\sum_{i=1}^{n} c_{i}\underline{b}_{i}, \underline{b}_{j}> = \sum_{i=1}^{n} c_{i}<\underline{b}_{i}, \underline{b}_{j}> \overset{\text{Ortog.}}{=} c_{j}<\underline{b}_{j}, \underline{b}_{j}> = c_{j}||\underline{b}_{j}||^2 = c_{j}$$

## Generazione
- [[Algoritmo di Gram-Schmidt]]
- 