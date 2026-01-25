#GAL 

## Forma Canonica Metrica

> [!error] Teorema
> SIa $Q = \{ \underline{x} \in \mathbb{R}: \underline{x}^TA\underline{x} + \underline{b}^Tx + c = 0 \}$ una quadrica senza centro (cioè $\underline{b} \not\in \mathrm{col}A$)
> Sia $\underline{v}_0$ un vertice (cioè $\underline{v}_{0} \in Q \cap A(Q)$) e $\underline{b}' = \underline{b} - \Pi_{\mathrm{col}A}(\underline{b}) = \Pi_{\mathrm{Ker}A}(\underline{b})$
> $\underline{u}_{1}, \dots, \underline{u}_{n}$ base ortonormale di $\mathbb{R}^n$ di autovettori di $A$, con $\underline{u}_{1}, \dots, \underline{u}_{s}$ associati a $\lambda_{i} \neq 0$
> $\underline{u}_{s+1}, \dots, \underline{u}_{n}$ associati a $\lambda_{i} = 0$ con $\underline{u}_{s+1} = \frac{1}{||\underline{b}'||}\underline{b}'$
> Sia $S = (\underline{u}_{1}, \dots, \underline{u}_{n})$ l'isometria 
> $$\underline{x} = S\underline{z} + \underline{v}_{0}$$
> trasforma l'equazione di $Q$ in
> $$\lambda_{1} z_{1}^2 + \dots + \lambda_{s}z_{s}^2 + 2||\underline{b}'||z_{s+1} = 0$$
> detta **Forma Canonica Metrica**

## Forma Canonica Affine

> [!warning] Definizione (Forma Canonica affine)
> $$z_{i} = \frac{1}{\sqrt{ |\lambda_{i}| }}w_{i},\ \ \forall\ i \in [1, n]$$
> $$z_{s+i} = \frac{1}{2||\underline{b}||'} w_{s+i}$$
> $$z_{1} = w_{1}$$
> l'equazione derivata è
> $$w_{1}^2 + \dots + w_{p^2} - w_{p+1}^2 - \dots - w_{p+r}^2 + w_{s+1} = 0$$
> dove $(p, r, n-p-r)$ è la [[Segnatura]] di $A$ $(s = p+r)$ detta **Forma Canonica Affine** di $Q$
> (centro: $w_{1}^2 + \dots + w_{p}^2 - w_{p+1}^2 - \dots - w_{p+r}^2 + c'' = 0$ con $c'' \in \{ 1, -1, 0 \}$)

> [!info] Osservazione
> La forma canonica affine di una quadratica dipende solo sa:
> - Segnatura di $A$
> - Centro / no centro
> 	- $c'' = \{ 1, -1, 0 \}$
> $\implies$ fissato $n$, numero finito di possibilità
> - $n = 2 \implies 9$ coniche
> - $n = 3 \implies 17$ superfici quadriche