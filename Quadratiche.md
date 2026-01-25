#GAL 
> [!warning] Definizione
> Una forma quadratica è un polinomio $q:\mathbb{R}^n \to \mathbb{R}$ omogeneo di 2° grado in $n$ variabili

> [!warning] Definizione (Segno di una funzione quadratica)
> $q: \mathbb{R}^n \to \mathbb{R}$ si dice
> - **Definita Positiva** se $q(\underline{x}) > 0\ \forall\ x \neq \underline{0}$
> - **Definita Negativa** se $q(\underline{x}) < 0\ \forall\ x \neq \underline{0}$
> - **Semidefinita Positiva** se $q(\underline{x}) \geq 0\ \forall\ x \in \mathbb{R}^n$
> - **Semidefinita Negativa** se $q(\underline{x}) \leq 0\ \forall\ x \in \mathbb{R}^n$
> - **Indefinita** in alternativa

> [!error] Proposizione
> Sia $q(\underline{x}) = \sum_{i\leq j} a_{ij} x_{i} x_{j}$ una forma quadratica in $n$ variabili $q :\mathbb{R}^n \to \mathbb{R}$
> Esiste un'unica matrice simmetrica $A \in \mathrm{Mat}(n,n) :$
> $$q(\underline{x}) = \underline{x}^T A \underline{x}$$
> Dove
> $$(A)_{ij} = \begin{cases} a_{ii} & i = j \\ \dfrac{a_{ij}}{2} & i < j \\ \dfrac{a_{ji}}{2} & i > j \end{cases}$$

> [!error] Proposizione
> Siano $q_{1}, q_{2} : \mathbb{R}^n \to \mathbb{R} : q_{1} = \underline{x}^TA\underline{x},\ q_{2} = \underline{x}^TB\underline{x}$. Allora:
> $$A,B \text{ congruenti} \Leftrightarrow q_{1} = q_{2}$$

> [!error] Dimostrazione
> $q_{1}, q_{2}$ equivalenti $\Leftrightarrow \exists$ isomorfismo $L:\mathbb{R}^n \to \mathbb{R}^n$ tale che $q_{1}(\underline{x}) = q_{2}(L(\underline{x})) \Leftrightarrow \exists\ S$ invertibile tale che
> $$\underline{x}^TA\underline{x} = (S\underline{x})^TB(S\underline{x}) = \underline{x}^T(S^TBS)\underline{x}$$
> $$\implies A = S^TBS$$
> $$\implies \boxed{A,B \text{ congruenti}}$$
## Proprietà
- [[Segnatura]]
- [[Equivalenza]]

## Teoremi
- [[Teorema di Sylvester]]