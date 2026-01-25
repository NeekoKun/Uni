#GAL
> [!warning] Definizione
> Due matrici $A,B$ tali che $$A = S^{-1}BS$$ si dicono **Matrici Simili**

> [!error] Proposizione 
> Siano $A,B$ matrici simili. Allora:
> - $\det A = \det B$
> - $\mathrm{rk}A=\mathrm{rk}B$
> - $\chi_{A}(x)=\chi_{B}(x)$
> - $A^{-1}, B^{-1}$ sono simili
> - $A^k, B^k$ sono simili $\forall\ k \in \mathbb{N}$
> - $A^T, B^T$ sono simili

> [!error] Dimostrazione
> Per ipotesi, $A = S^{-1}BS$ con $S$ invertibile
> 1. $\det A = \det (S^{-1}BS)  = \det S^{-1} \det B \det S = \det B$ $$\implies \boxed{\det A = \det B}$$
> 2. $\mathrm{rk}(A) = \mathrm{dim}\Im T_{A} = \mathrm{dim} (T_{S^{-1}} \circ T_{B} \circ T_{S})$ ma $T_{S}$ è un isomorfismo, quindi $$\mathrm{dim}(T_{S^{-1}} \circ T_{B} \circ T_{S}) = \mathrm{dim} (T_{B}) = rk(B)$$ 
> $$\implies \boxed{\mathrm{rk}A = \mathrm{rk}B}$$
> 3. $A -xI_{n} = S^{-1}BS - xI_{n} = S^{-1}BS - S^{-1}xI_{n}S = S^{-1}(B - xI_{n})S$
> $$\implies A - xI_{n},\ B - xI_{n} \text{ sono simili}$$
> $$\implies \boxed{\chi_{A}(x) = \chi_{B}(x)}$$
> 4. $A^k = (S^{-1}BS)^k = (S^{-1}BS)(S^{-1}BS)\dots(S^{-1}BS) = S^{-1}B(SS^{-1})B(S\dots S^{-1})BS$
> $$= S^{-1}BB\dots BS = S^{-1}B^kS$$ $$\implies \boxed{A^k = S^{-1}B^kS}$$

> [!info] Osservazione
> Queste condizioni sono **necessarie ma non sufficienti**