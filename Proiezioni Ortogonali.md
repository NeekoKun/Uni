#GAL 
> [!warning]
> Sia $V$ [[Spazi Euclidei|Spazio Euclideo]], $H \subseteq V$ un sottospazio $B = \{ \underline{b}_{1},\dots,\underline{b}_{d} \}$ una [[Base Ortogonale e Ortonormale|Base Ortonormale]] di $H$
> La **Proiezione Ortogonale** su $H$ è la funzione $$\pi_{H}:V \to V \text{ definita da } \pi_{H}(\underline{v}) = \sum_{i=1}^{d} <\underline{v}_{i}, \underline{b}_{i}>\underline{b}_{i}\ \forall\ \underline{v} \in V$$

## Proprietà
> [!error] Proposizione (Linearità)
> $\pi_{H}$ è un'[[Applicazioni Lineari|Applicazione Lineare]]

> [!error] Dimostrazione
> Se $\underline{v}_{1}, \underline{v}_{2} \in V,\ \pi_{H(\underline{v}_{1} + \underline{v}_{2})} = \sum_{i=1}^{d}<\underline{v}_{1} + \underline{v}_{2}, \underline{b}_{i}>\underline{b}_{i}$
> $$= \sum_{i=1}^{d} (<\underline{v}_{1},\underline{b}_{i}> + <\underline{v}_{2}, \underline{b}_{i}>)\underline{b}_{i} = \sum_{i=1}^{d} <\underline{v}_{1}, \underline{b}_{i}>\underline{b}_{i} + \sum_{i=1}^{d} <\underline{v}_{2}, \underline{b}_{i}>\underline{b}_{i}$$ $$= \boxed{\pi_{H}(\underline{v}_{1}) + \pi_{H}(\underline{v}_{2})}$$
> $\pi_{H}(c\underline{v}_{1}) = c\pi_{H}(\underline{v}_2)$ dimostrabile analogamente

---
> [!error] Proposizione
> Se $\underline{w} \in H$ allora $\pi_{H}(\underline{w}) = \underline{w}$

> [!error] Dimostrazione
> Proprietà "Coordinate rispetto a base ortonormale" applicato a $\underline{w} \in H$

---
> [!error] Proposizione
> $\Im\pi_{H} = H$

> [!error] Dimostrazione
> $H \subseteq \Im \pi_{H}$ segue dalla seconda
> $\forall\ \underline{w} \in H \implies \pi_{H}(\underline{w}) = \underline{w} \in \Im\pi_{H}$
> Viceversa, $\underline{v} \in V, \pi_{H}(\underline{v}) \in \mathrm{Span}(\underline{b}_{1},\dots,\underline{b}_{d}) = H$
> $\implies \Im\pi_{H} \subseteq H$

---
> [!error] Proposizione
> $\pi_{H} \circ \pi_{H} = \pi_{H}$

> [!error] Dimostrazione
> $\forall\ \underline{v} \in V \implies \pi_{H}(\underline{v}) \in H$
> $\pi_{H}(\pi_{H}(\underline{v})) \overset{2.}{=} \pi_{H}(\underline{v})$

---
> [!error] Proposizione (Nucleo)
> $\mathrm{Ker}(\pi_{H}) = H^\perp$

> [!error] Dimostrazione
> $\underline{w} \in \mathrm{Ker}(\pi_{H}) \Leftrightarrow \pi_{H}(\underline{w}) = \underline{0} \Leftrightarrow \sum_{i=1}^{d} <\underline{v}, \underline{b}_{i}>\underline{b}_{i} = \underline{0} \overset{L.I.}{\Leftrightarrow} <\underline{v}_{i}, \underline{b}_{i}> = 0\ \forall\ i \in [i,d]$
> $\Leftrightarrow \underline{v} \perp \underline{b}_{i}\ \forall\ i \in [1, d] \Leftrightarrow \underline{v} \in \mathrm{Span}(\underline{b}_{1}, \dots, \underline{b}_{d})^\perp = H^\perp$

---
> [!error] Proposizione
> $\forall\ \underline{v} \in V \implies \underline{v} - \pi_{H}(\underline{v}) \in H^\perp$

> [!error] Dimostrazione
> $\forall\ \underline{v} \in V\ \pi_{H}(\underline{v} - \pi_{H}(\underline{v})) = \pi_{H}(\underline{v}) - \pi_{H}(\pi_{H}(\underline{v})) = \pi_{H}(\underline{v}) - \pi_{H}(\underline{v}) = \underline{0}$
> $\implies \underline{v} - \pi_{H}(\underline{v}) \in \mathrm{Ker}(\pi_{H}) = H^\perp$
> $\implies \boxed{\underline{v} - \pi_{H}(\underline{v}) \in H^\perp}$

## Corollari
> [!error] Corollario
> $\mathrm{dim}H + \mathrm{dim}H^\perp = \mathrm{dim}V$

> [!error] Dimostrazione
> [[Teorema di Nullità + Rango]]

---
> [!error] Corollario
> $H + H^\perp = V$

> [!error] Dimostrazione
> Segue da proprietà 6

---
> [!error] Corollario
> $H\ \cap\ H^\perp = \{ \underline{0} \}$

> [!error] Dimostrazione
> [[Formula di Grassmann]]

---
> [!error] Corollario
> $H^{\perp\perp} = H

> [!error] Dimostrazione
> - $H \subseteq (H^\perp)^\perp$: Ogni $\underline{v} \in H$ è ortogonale a ogni $\underline{w} \in H^\perp$
> - $\mathrm{dim}(H^\perp)^\perp = \mathrm{dim}V - \mathrm{dim}H^\perp = \mathrm{dim}H$
> $$\implies \boxed{H = (H^\perp)^\perp}$$

---
> [!error] Corollario
> $\forall\ \underline{v} \in V \implies \underline{v} = \pi_{H}(\underline{v}) + \pi_{H^\perp}(\underline{v})$

> [!error] Dimostrazione
> Siano
> $B_{1} = \{ \underline{b}_{1}, \dots, \underline{b}_{d} \}$ base **Ortonormale** di $H$
> $B_{2} = \{ \underline{b}_{d+1}, \dots, \underline{b}_{n} \}$ base **Ortonormale** di $H^\perp$
> $\implies B_{1} \cup B_{2}$ è una base ortonormale di $V$
> Se $\underline{v} \in V$, Proprietà "Coordinate Rispetto a Base Ortonormale"
> $$\implies \underline{v} = <\underline{v}_{1}, \underline{b}_{1}>$$

---
> [!error] Corollario
> $\pi_{H} : V \to V$ è l'unica [[Applicazioni Lineari|Applicazione Lineare]] $L:V\to V$ tale che:
> $$L(\underline{v}) = \begin{cases} \underline{v} & \underline{v} \in H \\ \underline{0} & \underline{v} \in H^\perp \end{cases}$$
> In particolare, $\pi_{H}$ non dipende dalla base ortonormale $B$  scelta per $H$

> [!error] Dimostrazione
> Segue dal [[Teorema di Interpolazione]] dato che se:
> - $B_{1}$ base di $H$
> - $B_{2}$ base di $H^\perp$
>
> Allora (per il corollario precedente) $B_{1}\ \cup\ B_{2}$ è una base di $V$

---
> [!error] Corollario
> Dati $\underline{v} \in V, H \subseteq V$ sottospazio, $\pi_{H}(\underline{v})$ è il vettore di $H$ più vicino a $\underline{v}$, cioè:
> $$\forall\ \underline{w} \in H \implies d(\underline{v}, \underline{w}) \geq d(\underline{v}, \pi_{H(\underline{v})})$$

> [!error] Dimostrazione
> Sia $\underline{w} \in H$, scriviamo $0 \leq d(\underline{v}, \underline{w})^2 = ||\underline{v} - \underline{w}||^2 = ||\underline{v} - \pi_{H}(\underline{v}) + \pi_{H}(\underline{v}) - \underline{w}||^2$
> Che, per [[Teorema del Coseno|Teorema di Pitagora]] è
> $$= ||\underline{v} - \pi_{H}(\underline{v})||^2 + ||\pi_{H}(\underline{v}) - \underline{w}||^2$$
> $$= d(\underline{v}, \pi_{H}(\underline{v}))^2 + d(\pi_{H}(\underline{v}), \underline{w})^2$$
> $$\implies 0 \leq d(\underline{v}, \pi_{H}(\underline{v}))^2 + d(\pi_{H}(\underline{v}), \underline{w})^2$$
> $$\implies \boxed{d(\underline{v}, \pi_{H}(\underline{v})) \leq d(\pi_{H}(\underline{v}), \underline{w})}$$

