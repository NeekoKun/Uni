#GAL 
> [!warning] Definizione
> Sia $V$ [[Spazi Euclidei|Spazio Euclideo]]
> Si definisce **Distanza** tra $\underline{v}, \underline{w} \in V: d(\underline{v},\underline{w}) = ||\underline{v} - \underline{w}||$

## Distanza tra [[Sottospazio Affine|Sottospazi Affini]]
> [!warning] Definizione
> La **Distanza** tra due Sottospazi Affini $S_{1} = \underline{v}_{1} + H_{1},\ S_{2} = \underline{v}_{2} + H_{2} \subseteq V$ è $d(S_{1}, S_{2}) = \mathrm{min}\{ d(\underline{v}, \underline{w})\ \forall\ \underline{v} \in S_{1}, \underline{w} \in S_{2} \}$

> [!info] Osservazione
> Se $S_{1} \cap S_{2} \neq \emptyset$ scegliamo $\underline{v} = \underline{w} \in S_{1} \cap S_{2} \implies d(S_{1}, S_{2}) = 0$

> [!error] Proprosizione
> Dati [[Sottospazio Affine|Sottospazi Affini]] $S_{1} = \underline{v}_{1} + H_{1}, S_{2} = \underline{v}_{2} + H_{2} \subseteq V$, denotiamo $H = H_{1} + H_{2}$
> $$d(S_{1}, S_{2}) = ||\pi_{H^\perp}(\underline{v}_{2} - \underline{v}_{1})||$$