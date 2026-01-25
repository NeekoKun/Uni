---
aliases:
  - Applicazione Lineare
---
#GAL
> [!warning] Definizione
> Siano $V, W$ due spazi vettoriali.
> Un'**Applicazione Lineare** (o Trasformazione Lineare) è una funzione $L : V \to W:$
> - $L(\underline{v}_{1} + \underline{v}_{2}) = L(\underline{v}_{1}) + L(\underline{v}_{2})\ \forall\ \underline{v}_{1}, \underline{v}_{2} \in V$
> - $L(c\cdot\underline{v}_{1}) =  c\cdot L(\underline{v}_{1})\ \forall\ \underline{v}_{1} \in V$

> [!info] Conseguenze
> $L(\underline{0}_{V}) = L(0 \cdot \underline{0}_{V}) = 0 \cdot L(\underline{0}_{V})$ = $\underline{0}_{W}$
> - $L(c_{1}\underline{v}_{1} + \dots + c_{n} + \underline{v}_{n}) = c_{1}L(\underline{v}_{1}) + \dots + c_{n}L(\underline{v}_{n})$

> [!info] Esempi
> 1. $L_{1} : \mathbb{R}^2 \to \mathbb{R}^2$ definita da $L_{1}\begin{pmatrix}x_{1} \\ x_{2}\end{pmatrix} = \begin{pmatrix}x_{1} + x_{2} \\ x_{1} - x_{2}\end{pmatrix}$ 
> Questa funzione è un'applicazione Lineare

> [!error] Proposizione
> 1. Sia $A \in \mathrm{Mat}(m, n)$. La funzione $T_{A}: \mathbb{R}^n \to \mathbb{R}^m$ definita da $$T_{A}(\underline{v}) = A\underline{v},\ \forall\ v \in \mathbb{R}^n$$ è un'applicazione lineare
> 2. Viceversa, ogni Applicazione Lienare $L: \mathbb{R}^n \to \mathbb{R}^m$ è della forma $T_{A}$ per un'unica matrice $A$

> [!error] Dimostrazione
> 1. Fissiamo $A \in \mathrm{Mat}(m, n)$
> 	1. $T_{A}(\underline{v}_{1} + \underline{v}_{2}) = A(\underline{v}_{1} + \underline{v}_{2}) = A\underline{v}_{1} + A\underline{v}_{2} = T_{A}(\underline{v}_{1}) + T_{A}(\underline{v}_{2})$
> 	2. $T_{A}(c \underline{v}) = A(c \underline{v}) = c A(\underline{v}) = c T_{A}(\underline{v})$
> 2. Fissiamo $L: \mathbb{R}^n \to \mathbb{R}^m$
> 	Consideriamo la matrice $A = (L(\underline{e}_{1}), \dots, L(\underline{e}_{n})) \in \mathrm{Mat}(m, n)$
> 	$L = T_{A} \forall\ \underline{v} \in \mathbb{R}^n \underline{v} = \begin{pmatrix}v_{1} \\ \vdots \\ v_{n}\end{pmatrix} \implies \underline{v} = v_{1}\underline{e}_{1} + \dots + v_{n} \underline{e}_{n}$
> 	$L(\underline{v}) = v_{1}L(\underline{e}_{1}) + \dots + v_{n}L(\underline{e}_{m})$
> 	$= A\begin{pmatrix}v_{1} \\ \vdots \\ v_{n} \end{pmatrix} = A\underline{v} = T_{A(\underline{v})}$

## Immagine e Nucleo
> [!warning] Definizione
> Sia $L: V \to W$ applicazione lineare.
> L'==Immagine== di $L$ è l'immagine di tutto $V$: $$\mathrm{Im}(L) = L(V) = \{  L(\underline{v}) : \underline{v} \in V\} \subseteq W$$
> Il ==Nucleo== di $L$ è la controimmagine di $\{ \underline{0}_{W} \}$: $$\mathrm{Ker}(L) = L^{-1}(\{ \underline{0}_{W} \}) = \{ \underline{v} \in V : L(\underline{v}) = \underline{0}_{W} \} \subseteq V$$

> [!info] Osservazione
> Se $H = \mathrm{Span}(\underline{v}_{1}, \dots, \underline{v}_{n}) = \left\{  \sum_{i=1}^{n} c_{i} \underline{v}_{i} : c_{i} \in \mathbb{R}  \right\} \subseteq V$
> $$\implies L(H) = \left\{  L\left( \sum_{i=1}^{n} c_{i}\underline{v}_{}i \right) : c_{i} \in \mathbb{R} \right\}$$
> $$= \left\{  \sum_{i=1}^{n} c_{i}L(\underline{v}_{i}) : c_{i} \in \mathbb{R}  \right\} = \mathrm{Span}(L(\underline{v}_{1}), \dots, L(\underline{v}_{n})) \subseteq W$$
> $\boxed{\text{Le immagini dei Generatori sono Generatori dell'Immagine}}$

## Iniettività
> [!warning] Definizione
> $L: V \to W$ è iniettiva se: $\underline{v}_{1} \neq \underline{v}_{2} \implies L(\underline{v}_{1}) \neq L(\underline{v}_{2})$
> Oppure se (equivalentemente): $L(\underline{v}_{1}) = L(\underline{v}_{2}) \implies \underline{v}_{1} = \underline{v}_{2}$

> [!error] Proposizione
> $L:V \to W$ applicazione lineare. $L$ è iniettiva $\Leftrightarrow \mathrm{Ker}(L) = \{ \underline{0}_{V} \}$

> [!error] Dimostrazione
> 1. Supponiamo $L$ iniettiva. Sia $\underline{v} \in \mathrm{Ker}(L) \implies L(\underline{v}) = \underline{0}_{W}$ ma anche $L(\underline{0}_{V}) = \underline{0}_{W} \underset{\text{Iniettività}}{\implies} \underline{v} = \underline{0}_{V}$
>$$\implies \mathrm{Ker}(L) = \{ \underline{0}_{V} \}$$
>2. Supponiamo $\mathrm{Ker}(L)$. Dati $\underline{v}_{1}, \underline{v}_{2} \in V : L(\underline{v}_{1}) = L(\underline{v}_{2})$
>$$\implies L(\underline{v}_{1}) - L(\underline{v}_{2}) = \underline{0}_{W} \implies L(\underline{v}_{1} - \underline{v}_{2}) = \underline{0} \implies \underline{v}_{1} - \underline{v}_{2} \in \mathrm{Ker}(L)$$
>ma $\mathrm{Ker}(L) = \{ \underline{0}_{V} \} \implies \underline{v}_{1} - \underline{v}_{2} = \underline{0} \implies \underline{v}_{1} = \underline{v}_{2}$
>$\implies L$ iniettiva

> [!warning] Corollario
> $T_{A} A \in \mathrm{Mat}(m, n)$
> $T_{A} : \mathbb{R}^n \to \mathbb{R}^m$ è iniettiva $\Leftrightarrow \mathrm{Ker}(T_{A}) = \{ \underline{0} \} \Leftrightarrow \mathrm{Ker}(A) = \{ \underline{0} \} \Leftrightarrow \mathrm{dim}(\mathrm{Ker}(A)) = 0 \underset{\text{Nullità + Rango}}{\Leftrightarrow} n - \mathrm{rK}(A) = 0$
> $\Leftrightarrow \mathrm{rK}(A) = n$

> [!info] Osservazione
> In generale, $\underline{v}_{1}, \dots, \underline{v}_{n}$ L.I. $\not\implies$ $L(\underline{v}_{1}), \dots, L(\underline{v}_{n})$ L.I.

> [!error] Proposizione
> Sia $L :V \to W$ iniettiva
> Se $\underline{v}_{1}, \dots, \underline{v}_{n} \in V$ sono L.I. $\implies L(\underline{v}_{1}), \dots, L(\underline{v}_{n})$ sono L.I.

> [!error] Dimostrazione
> Supponiamo $c_{1}L(\underline{v}_{1}) + \dots + c_{n}L(\underline{v}_{n}) = \underline{0}_{W}$ per qualche $c_{i}$
> $$\implies L(c_{1}\underline{v}_{1} + \dots + c_{n}\underline{v}_{n}) = \underline{0}_{W}$$
> $$c_{1}\underline{v}_{1} + \dots + c_{n}\underline{v}_{n} \in \mathrm{Ker}(L) \overset{\text{ipotesi}}{=} \{  \underline{0}_{V} \}$$
> $$\implies c_{1}\underline{v}_{1} + \dots + c_{n}\underline{v}_{n} = \underline{0}_{V} \overset{\text{ipotesi}}{\implies} c_{1} = \dots = c_{n} = 0$$

> [!warning] Corollario
> Sia $L:V \to W$ iniettiva
> Se $\{ \underline{v}_{1}, \dots, \underline{v}_{n} \}$ base di $H \subseteq V \implies \{ L(\underline{v}_{1}), \dots, L(\underline{v}_{n}) \}$ base di $L(H)$
> Inoltre, $\mathrm{dim}(H) = \mathrm{dim}(L(H))$
> 

## Suriettività
> [!warning] Definizione
> $L: V \to W$ è suriettiva se $\mathrm{Im}(L) = W$

> [!warning] Corollario
> $L:V \to W$ è suriettiva $\Leftrightarrow \mathrm{dim}(\mathrm{Im}(L)) = \mathrm{dim}(W)$

## Biunivicità
> [!warning] Definizione
> Un'applicazione lineare biunivoca (iniettiva + suriettiva) si dice ==Isomorfismo==.
> Intuitivamente:
> se $L: V \to W$ isomorfismo, allora $V$ e $W$ hanno la stessa struttura di spazio
> 

> [!error] Proposizione
> Sia $L : V \to W$ un isomorfismo
> Siano $\underline{v}_{1}, \dots, \underline{v}_{2} \in V, H, K \subseteq V$ sottospazi. Allora:
> - $\mathrm{dim}(V) = \mathrm{dim}(W)$
> - $\underline{v}_{1}, \dots, \underline{v}_{n}$ sono L.I. / generatori di $V$ / base di $V \leftrightarrow$ $$L(\underline{v}_{1}), \dots, L(\underline{v}_{n}) \text{sono L.I. / generatori di W / base di W}$$
> - $\mathrm{dim}(H) = \mathrm{dim}(L(H))$
> - $L(H \cap K) = L(H) \cap L(K)$
> - $L(H + K) = L(H) + L(K)$
## Notazione
> [!warning] Definizione
> $[\underline{v}]_{B} = \begin{pmatrix}c_{1} \\ c_{2} \\ \vdots \\ c_{n} \end{pmatrix} \in \mathbb{R}^n$ si chiama "Vettore delle coordinate $\underline{v}$ della base $B$"

> [!warning] Definizione
> $V$ sp. vettoriale, $B = \{ \underline{b}_{1},\dots,\underline{b}_{n} \}$ base di $V$
> La funzione $Q_{B}:V \to \mathbb{R}^n$ definita da $Q_{B}(\underline{v}) = [\underline{v}]_{B}$ si chiama "Mappa delle Coordinate"
## Trasformazioni Lineari nel [[Piano]]

## Teoremi
- [[Teorema di Interpolazione]]
- [[Teorema di Rappresentazione]]

> [!error] Proposizione
> 1. $P_{C}$ è suriettiva $\Leftrightarrow$ $\underline{w}_{1}, \dots, \underline{w}_{n}$ generatori di $W$
> 2. $P_{C}$ è iniettiva $\Leftrightarrow$ $\underline{w}_{1}, \dots, \underline{w}_{n}$  linearmente indipendenti
> 3. $P_{C}$ è un isomorfismo $\Leftrightarrow$  $C$ è una base di $W$
> 4. Ogni [[Applicazioni Lineari|Applicazione Lineare]] $L : \mathbb{R}^n \to W$ è della forma $L = P_{C}$, dove $C = \{ L(\underline{e}_{1}), \dots, L(\underline{e}_{n}) \}$