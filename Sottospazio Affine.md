#GAL 
> [!warning] Definizione
> Sia $V$ uno [[Spazi Vettoriali|Spazio Vettoriale]]
> Un sottoinsieme $S \subseteq V$ si dice **Sottospazio Affine** se $S \neq \emptyset$ oppure se esiste un [[Spazi Vettoriali#Sottospazi Vettoriali|Sottospazio Vettoriale]] $H \subseteq B$ ed un vettore $\underline{v} \in V$ tale che $S = \underline{v}_{0} + H \overset{def}{=} \{ \underline{v}_{0} + \underline{w}:\underline{w} \in H \}$

> [!info] Osservazione
> $\underline{v}_{0}$ p un punto particolare/qualsiasi di $S$, quindi $S$ non è unicamente determinato

> [!error] Teorema
> Questo sotto spazio $H$ è unicamente determinato
> $\underline{v}_{1}, \underline{v}_{2} \in V,\ \ H_{1}, H_{2} \subseteq V$ $$\underline{v}_{1} + H_{1} = \underline{v}_{2}+H_{2} \implies H_{1} = H_{2}$$

> [!error] Dimostrazione
> Supponiamo $\underline{v}_{1} + H_{1} = \underline{v}_{2} + H_{2}$
> Dimostriamo $H_{1} \subseteq H_{2}, H_{2} \subseteq H_{1}$
> 1. $\forall\ \underline{w} \in H_{1} 0> \underline{v}_{1} + \underline{w} \subset \underline{v}_{1}+H_{1} = \underline{v}_{2} + H_{2}$ $$\implies \underline{w} = (\underline{v}_{2} - \underline{v}_{1}) + \underline{u} : \underline{u} \in H_{2}$$
> $\underline{w} = \underline{0} \in H_{2}$ $$\underline{v}_{1} = \underline{v}_{1} + \underline{0} \in \underline{v}_{1} + H_{1} = \underline{v}_{2} + H_{2}$$ $$\implies \underline{v}_{1} = \underline{v}_{2} + \underline{u}'$$ $$\implies \underline{v}_{1} - \underline{v}_{2} = \underline{u}' \in H_{2}$$
> $$\implies (\underline{v}_{2} - \underline{v}_{1}) \in H_{2}$$
> $(\underline{v}_{2} - \underline{v}_{1}) + \underline{u} \in H_{2}$ $$\implies \boxed{\underline{w} \in H_{2}}$$

## Giuntura
> [!warning] Definizione
> Sia $S = \underline{v}_{0} + H \subseteq V$ un Sottospazio Affine con $H \subseteq V$ [[Spazi Vettoriali#Sottospazi Vettoriali|Sottospazio Vettoriale]], $H$ si chiama **Giuntura** di $S$

> [!info] Osservazione
> $\mathrm{dim}(S) = \mathrm{dim}(H)$