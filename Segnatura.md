#GAL 
> [!warning] Definizione (Di una quadratica)
> La **segnatura** di una [[Quadratiche]] è la terna di numeri $(n_{+}, n_{-}, n_{0})$ dove:
> - $n_{+} = \mathrm{max}\{ \mathrm{dim}H : H \subseteq \mathbb{R}^n :q(\underline{x}) > 0\ \forall\ \underline{0} \neq \underline{x} \in H \}$
> - $n_{-} = \mathrm{max}\{ \mathrm{dim}H : H \subseteq \mathbb{R}^n :q(\underline{x}) < 0\ \forall\ \underline{0} \neq \underline{x} \in H \}$
> - $n_{0} = n - n_{+} - n_{-}$

> [!warning] Definizione (Di una Matrice)
> Il segno/segnatura di una matrice simmetrica $A$ è il segno/segnatura di $q(\underline{x}) = \underline{x}^TA\underline{x}$

| Segno di $q$          | Segnatura di $q$    |
| --------------------- | ------------------- |
| definita positiva     | $(n, 0, 0)$         |
| definita negativa     | $(0, n, 0)$         |
| semidefinita positiva | $(n_{+}, 0, n_{0})$ |
| semidefinita negativa | $(0, n_{-}, n_{0})$ |
| indefinita            | $n_{+}, n_{-} > 0$  |

> [!error] Proposizione
> Forme quadratiche equivalenti hanno la stessa **Segnatura**
