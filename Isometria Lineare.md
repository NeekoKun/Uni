#GAL
> [!warning] Definizione
> Sia $V$ uno [[Spazi Euclidei|Spazio Euclideo]].
> Un'**Isometria Lineare** è un [[Endomorfismi|Endorfismo]] $L: V \to V$ tale che:
> $$<L(\underline{v}), L(\underline{w})> = <\underline{v}, \underline{w}>\ \forall\ \underline{v}, \underline{w} \in V$$

> [!info] Osservazione
> Se $L:V \to V$ **Isometria Lineare**
> - $||L(\underline{v})|| = ||\underline{v}||$
> - $d(L(\underline{v}), L(\underline{w})) = d(\underline{v}, \underline{w})$
> - $\widehat{L(\underline{v}), L(\underline{w})} = \widehat{\underline{v}, \underline{w}}$
> - $L$ è un [[Applicazioni Lineari#Biunivicità|Isomorfismo]]

> [!error] Dimostrazione
> $L(\underline{v}) = \underline{0} \Leftrightarrow ||L(\underline{v})|| = 0 \Leftrightarrow ||\underline{v}|| = 0 \Leftrightarrow \underline{v} = \underline{0}$

---
> [!error] Proposizione
> Sia $V$ [[Spazi Euclidei|Spazio Euclideo]], $B = \{  \underline{b}_{1} , \dots, \underline{b}_{n} \}$ base ortonormale, $L:V\to V$ [[Endomorfismi|Endorfismo]].
> Allora $L$ è **Isometria Lineare** $\Leftrightarrow \{ L(\underline{b}_{1}), \dots, L(\underline{b}_{n})\}$ è una [[Base Ortogonale e Ortonormale|Base Ortonormale]]

> [!error] Dimostrazione
> - $\boxed{\Rightarrow}:\ <L(\underline{b}_{i}), L(\underline{b}_{j})>\ =\ <\underline{b}_{i}, \underline{b}_{j}>\ =\ \delta_{i,j} \implies$ Base Ortonormale
> - $\boxed{\Leftarrow}:$ Supponiamo $\{ L(\underline{b}_{1}), \dots, L(\underline{b}_{n}) \}$ base ortonormale di $V$. Dati $\underline{v} = \sum_{i=1}^{n}v_{i}\underline{b}_{i} \in V$, $\underline{w} = \sum_{i=1}^{n}w_{i}\underline{b}_{i} \in V$
> $$<\underline{v}, \underline{w}> = <\sum_{i=1}^{n} v_{i}\underline{b}_{i}, \sum_{j=1}^{n} w_{j}\underline{b}_{j}> = \sum_{i=1}^{n} \sum_{j=1}^{n} v_{i}w_{i} <\underline{b}_{i}, \underline{b}_{j}> = \sum_{i=1}^{n} \sum_{j=1}^{n} v_{i}w_{i} \delta_{i,j}$$
> $$= \sum_{i=1}^{n} v_{i}w_{i}$$
> Inoltre
> $$<L(\underline{v}), L(\underline{w})> = <L(\sum_{i=1}^{n} v_{i}\underline{b}_{i}), L(\sum_{j=1}^{n} w_{j}\underline{b}_{j})> = <\sum_{i=1}^{n} v_{i}L(\underline{b}_{i}), \sum_{j=1}^{n} w_{j}L(\underline{b}_{j})>$$
> $$ = \sum_{i=1}^{n} \sum_{j=1}^{n} v_{i}w_{i} <L(\underline{b}_{i}), L(\underline{b}_{j})> = \sum_{i=1}^{n} \sum_{j=1}^{n} v_{i}w_{i} <\underline{b}_{i}, \underline{b}_{j}> = \sum_{i=1}^{n} \sum_{j=1}^{n} v_{i}w_{i} \delta_{i,j}$$
> $$= \sum_{i=1}^{n} v_{i}w_{i}$$
> Quindi
> $$<\underline{v}, \underline{w}> = \sum_{i=1}^{n} v_{i}w_{i} = <L(\underline{v}), L(\underline{w})>$$
> $$\implies \boxed{<\underline{v}, \underline{w}> = <L(\underline{v}), L(\underline{w})>}$$

> [!info] Osservazione
> $V$ [[Spazi Euclidei|Spazio Euclideo]], $B$ [[Base Ortogonale e Ortonormale|Base Ortogonale]] di $V$
> $<\underline{v}, \underline{w}> = \sum_{i=1}^{n} v_{i}, w_{i} = [\underline{v}]_{B} \cdot [\underline{w}]_{B}$
