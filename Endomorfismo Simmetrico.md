#GAL
> [!warning] Definizione
> Sia $L:V \to V$ un [[Endomorfismi|Endomorfismo]]
> Si dice **Simmetrico** se
> $$<L(\underline{v}), \underline{w}> = <\underline{v}, L(\underline{w})>$$

> [!error] Proposizione
> Sia $B$ base ortogonale di $V$
> $L$ endorfismo simmetrico $\Leftrightarrow M^{B,B}_{L}$ matrice simmetrica

> [!error] Dimostrazione
> Poniamo $A = M^{B,B}_{L}$
> $$<L(\underline{v}), \underline{w}> = [L(\underline{v})]_{B}^T[\underline{w}]_{B} = (M^{B,B}_{L}[\underline{v}]_{B})^T [\underline{w}]_{B} = [\underline{v}]_{B}^TA^T[\underline{w}]_{B}$$
> $$<\underline{v}, L(\underline{w})> = [\underline{v}]_{B}^T[L(\underline{w})]_{B} = [\underline{v}]^T_{B} (M^{B,B}_{L}[\underline{w}]_{B}) = [\underline{v}]^T_{B}A[\underline{w}]_{B}$$ 
> - Se $A$ è simmetrica $\implies A = A^T \implies <L(\underline{v}), \underline{w}> = <\underline{v}, L(\underline{w})> \implies L$ simmetrico
> - L simmetrico $\implies [\underline{v}]_{B}^TA^T[\underline{w}]_{B} = [\underline{v}]^T_{B}A[\underline{w}]_{B}\ \forall\ \underline{v}, \underline{w} \in V$
> Scegliamo (da spararsi)
