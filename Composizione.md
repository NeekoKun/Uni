#GAL
> [!warning] Definizione
> Siano $L:U \to V, M:V \to W$ due [[Applicazioni Lineari]], $U, V, W$ [[Spazi Vettoriali]]. La **composizione** $M \circ L : U \to W$ è la funzione definita da $M \circ L (\underline{u}) = M(L(\underline{u}))$

> [!info] Osservazione
> $M \circ L$ è un'[[Applicazioni Lineari|Applicazione Lineare]]
> $\mathbb{R}^n \overset{T_{A}}{\to} \mathbb{R}^m \overset{T_{B}}{\to} \mathbb{R}^p$
> allora $T_{B} \circ T_{A} = T_{BA} : \mathbb{R}^n \to \mathbb{R}^p$

## Identità
> [!warning] Definizione
> $V$ spazio vettoriale. L'identità di $V$ è la funzione $id_{V}: V \to V$ definita da $id_{V}(\underline{v}) = \underline{v}\ \forall\ \underline{v} \in V$

> [!info] Osservazione
> $id_{V}$ è un isomorfismo

## Invertibilità
> [!warning] Definizione
> $L: V \to W$ si dice invertibile se esiste $M : W \to V : M \circ L = id_{V}$ e $L \circ M = id_{W}$

> [!info] Osservazione
> $A \in \mathrm{Mat}(n,n)$ matrice invertibile $\Leftrightarrow T_{A}$ applicazione lineare invertibile
> $T_{A^{-1}} \circ T_{A} = T_{A^{-1}A} = T_{I_{n}} = id_{\mathbb{R}^n}$

> [!info] Osservazione
> $L : V \to W$ isomorfismo $\Leftrightarrow L$ Invertibile