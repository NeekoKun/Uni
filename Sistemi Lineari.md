#GAL 

> [!warning] Definizione
> Un sistema lineare è un Sistema di **[[Equazione Lineare|Equazioni Lineari]]**
> Forma standard:
> $$
> \left\{
>\begin{array}{ r @{{}={}} r  >{{}}c<{{}} r  >{{}}c<{{}}  r }
>a_{11}x_{1} &+& a_{12}x_{2} &+& \dots  &+& a_{1n}x_{n} &=& b_{1} \\
>a_{21}x_{1} &+& a_{22}x_{2} &+& \dots  &+& a_{2n}x_{n} &=& b_{2} \\
>\vdots      &+& \vdots      &+& \ddots &+& \vdots \\ 
>a_{m1}x_{1} &+& a_{m2}x_{2} &+& \dots  &+& a_{mn}x_{n} &=& b_{m}
>\end{array}
>\right.
>$$

> [!warning] Definizione
> L'Insieme delle Soluzioni $S$:
> $S =\left\{ \underline{x}=\begin{pmatrix}x_{1}\\x_{2}\\\vdots\\x_{n}\end{pmatrix}\in \mathbb{R}^n:\underline{x}\ \text{soddisfa tutte le equazioni lineari} \right\} \subseteq \mathbb{R}^n$

> [!info] Metodo di Soluzione
> Risoluzione per Sostituzione:
> 1. Risolviamo un'Equazione in una variabile
> 2. Sostituiamo il risultato ad una equazione differente
> 3. Ripetiamo fino ad esaurire le equazioni
> 4. Sostituiamo a ritroso

> [!warning] Definizione
> 2 Sistemi Lineari sono **equivalenti** se hanno gli stessi insiemi delle soluzioni

> [!info] Metodo di Soluzione
> Risoluzione per Trasformazione in Sistemi Equivalenti
> **"Mosse di Gauss"** (Operazioni Elementari sulle Righe)
> 1. Scambiare la posizione di due equazioni ($EQ_{i} \leftrightarrow EQ_{j}$)
> 2. Moltiplicare un'equazione per uno scalare ($cEQ_{i}: c\neq 0$)
> 3. Sommare ad una equazione un multiplo di un'altra ($EQ_{i} + cEQ_{j}: i\neq j$)

> [!warning] Definizione
> Una [[Matrice]] è "**a scala**" se ogni riga *non nulla* inizia con più zeri della riga precedente.
> Un Sistema Lineare si dice "**a scala**" se la sua Matrice Completa è a scala

### Sistema Lineare -> Prodotto di Matrici
$$\begin{cases}
a_{11}x_{1}    & + & a_{12}x_{2}  & + & \dots  & + & a_{1n}x_{n}    & = & b_{1} \\
a_{21}x_{1}    & + & a_{22}x_{2}  & + & \dots  & + & a_{2n}x_{n}    & = & b_{2} \\
\ \ \ \ \vdots &   & \ \ \ \vdots &   & \ddots &  & \ \ \ \ \vdots  &   & \ \vdots \\
a_{m1}x_{1}    & + & a_{m2}x_{2}  & + & \dots  & + & a_{mn}x_{n}    & = & b_{m}
\end{cases} \Leftrightarrow  A \underline{x} = \underline{b} $$
### Sistemi Omogenei
> [!warning] Definizione
> Un sistema si dice ==omogeneo== se $b_{n} = 0\ \forall\ n$
> $\implies A\underline{x} = \underline{0}$

> [!info] Osservazione
> $\mathrm{Ker}A\neq \varnothing$
> - [[Teorema di Roché - Capelli]]
> 	- $\mathrm{rk}(A) = \mathrm{rk}(A, \underline{0})$
> - $\underline{0} \in \mathrm{Ker}A$

> [!error] Teorema
> Sia $A \underline{x}=\underline{b}$ in un sistema lineare, con insieme delle soluzioni S. Supponiamo $S\neq \varnothing$, sia $\underline{v}\in S$ un elemento
> Allora $S = \underline{v} + \mathrm{Ker}A \overset{def}{=} \{ \underline{v} + \underline{w}:\underline{w}\in \mathrm{Ker}A \}$

> [!error] Dimostrazione
> Dato $\underline{u} \in \mathbb{R}^n$
> $\implies \underline{u}\in S \Leftrightarrow \underline{u}\in \underline{v}+\mathrm{Ker}(A)$
> $\implies \underline{u}-\underline{v}=\mathrm{Ker}(A)$
> $\underline{v}\in S\implies A\underline{v}=\underline{b}$
> $\underline{u}\in S\implies A\underline{u}=\underline{b}\Leftrightarrow A\underline{u}=A\underline{v}$
> $\implies A\underline{u}-A\underline{v}=\underline{0}\implies A(\underline{u}-\underline{v})=\underline{0}$
> $\implies \boxed{\underline{u}-\underline{v}\in \mathrm{Ker}(A)}$