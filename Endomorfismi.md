#GAL 
> [!warning] Definizione
> Un **Endorfismo** è un'applicazione lineare della forma $L: V \to V$

> [!info] Osservazione
> Se $L = T_{A}$ con $A$ matrice diagonale, 

## Autovalori, Autovettori

> [!warning] Definizione
> $L:V \to V$ endorfismo se esistono $\lambda \in \mathbb{R}, \underline{0} +\underline{v} \in V: L(\underline{v}) = \lambda \underline{v}$. In questo caso diciamo che:
> - $\lambda$ è un **Autovalore** di $L$
> - $\underline{v}$ è un **Autovettore** di $L$ associato all'**Autovalore** $\lambda$
> 
> Se $L=T_{A}:\mathbb{R}^n \to \mathbb{R}^n$, diciamo anche **autovalore**/**autovettore** di $A$

> [!info] Esempio
> $$
> A = \begin{pmatrix} 1 & 2 \\ 3 & 4 \end{pmatrix} \begin{pmatrix} 1 \\ 2 \end{pmatrix} = \begin{pmatrix}5 \\ 10 \end{pmatrix} = 5\begin{pmatrix} 1 \\ 2 \end{pmatrix}
> $$
> -> 5 è un **Autovalore** di $A$, $\begin{pmatrix}1 \\ 2\end{pmatrix}$ è l'**autovettore** di $A$ associato a 5

> [!error] Proposizione
> $A \in \mathrm{Mat}(n, n)$, $\lambda$ è un autovalore di $A \Leftrightarrow \lambda$ è una radice di $\chi_{A}(x)$, dove $\chi_{A}(x)$ è il [[Polinomio Caratteristico]] di $A$

> [!error] Dimostrazione
> $\lambda$ autovalore di $A \Leftrightarrow \exists\ \underline{0} \neq \underline{v} \in \mathbb{R}^n : A\underline{v} = \lambda \underline{v}$
> Vogliamo dividere per $\underline{v}$ ma non possiamo perché non invertibile
> Quindi
> $$A\underline{v} - \lambda \underline{v} = 0$$
> $$A\underline{v} - \lambda I_{n} \underline{v} = 0$$
> $$(A - \lambda I_{n}) \underline{v} = 0$$
> $$\implies \underline{v} \in \mathrm{Ker}(A - \lambda I_{n})$$
> $$\implies \mathrm{Ker}(A - \lambda I_{n}) \neq \{ \underline{0} \} \Leftrightarrow \det(A - \lambda I_{n}) = 0$$

## Autospazio

> [!info] Osservazione
> $L(\underline{v}) = \lambda \underline{v} \Leftrightarrow L(\underline{v}) - \lambda \underline{v} = \underline{0}$
> $\Leftrightarrow L(\underline{v}) - \lambda I_{v}\underline{v} = \underline{0}$
> $\Leftrightarrow (A - \lambda I_{v})\underline{v} = \underline{0}$
> $\Leftrightarrow \underline{v} \in \mathrm{Ker}(A - \lambda I_{v})$

> [!warning] Definizione
> Sia $\lambda$ un autovettore di un endorfismo $L: V \to V$ l'**autospazio** di L associato a $\lambda$ $$E_{\lambda} = \mathrm{Ker(L - \lambda I_{v})} = \{ \text{Autovettori di L associati a }\lambda \} \cup \{ \underline{0} \} \subseteq V$$
> (Eigenspace)

> [!info] Esempio
> $A = \begin{pmatrix}2 & 1 \\ 1 & 2\end{pmatrix} \implies \lambda = 1,3$
> $$\implies E_{3} = \mathrm{Ker}(A - 3I_{2}) = \mathrm{Ker}\begin{pmatrix}-1 & 1 \\ 1 & -1\end{pmatrix} = \mathrm{Span}\begin{pmatrix}1 \\ 1\end{pmatrix}$$

> [!warning] Definizione (Diagonalizzabile)
> Un **Endorfismo** $L:V\to V$ è **Diagonalizzabile** se esiste una base $B$ di $V$ tale che:
> $M^{B,B}_{L}$ è una matrice diagonale
> Una matrice $A \in \mathrm{Mat}(n.n)$ è **Diagonalizzabile** se $T_{A}$ è diagonalizzabile

- [[Primo Criterio di Diagonalizzabilità]]
- [[Secondo Criterio di Diagonalizzabilità]]
- 
## Utilizzo degli Autospazi
> [!warning] Definizione
> Sia $L:V\to V$ un endorfismo.
> Se si possono trovare abbastanza coppie di autovettori / autovalori per definire una base di $V$, allora si può definire una base $C$ di $V$ con la seguente forma:
> $$M^{C,C}_{L} = \begin{pmatrix}\underline{v}_{1} & \dots & \underline{v}_{n}\end{pmatrix}$$
> Dove $\underline{v}_{i}$ è l'i-esimo autovettore di $L$.

> [!info] Osservazione
> Essendo questa una [[Matrice Diagonale]], è possibile applicare facilmente $L^n$ allo spazio, tramite [[Cambio di Base]]