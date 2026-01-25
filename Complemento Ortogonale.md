#GAL
> [!warning] Definizione
> Sia $H \subseteq V$ un sottospazio.
> Il **Complemento Ortogonale** di $H$ è $H^{\perp} = \{ \underline{v} \in V : \underline{v} \perp \underline{w}\ \forall\ \underline{w} \in H \}$

> [!error] Proposizione
> $H^\perp$ è un [[Sottospazio Vettoriale]] di $V$

> [!error] Proposizione
> Se $H = \mathrm{Span}(\underline{w}_{1}, \dots, \underline{w}_{a})$ allora
> $$H^\perp = \{ \underline{v} \in V: \underline{v} \perp \underline{w}_{i}\ \forall\ i \in [1, a] \}$$

> [!error] Dimostrazione
> $$\{ \underline{v} \in V: \underline{v} \perp \underline{w}\ \forall\ \underline{w} \in H \} = \{ \underline{v} \in V: \underline{v} \perp \underline{w}_{i}\ \forall\ i \in [1, a] \}$$
> - $\boxed\subseteq$ è ovvia
> - $\boxed\supseteq$ Sia $\underline{v} : \underline{v} \perp \underline{w}_{i}\ \forall\ i \in [1, a]$
> Sia $\underline{w} \in H$ qualsiasi
> $\underline{w}_{1}, \dots, \underline{w}_{a}$ generano $H \implies \underline{w} = \sum_{i=1}^{a} c_{i}\underline{w}_{i}$ per qualche $c_{i}$
> $<\underline{w}, \underline{w}> = <\underline{v}, \sum_{i=1}^{a}c_{i}\underline{w}_{i}> = \sum_{i=1}^{n}c_{i}<\underline{v}, \underline{w}_{i}> = \sum_{i=1}^{n}c_{i}0 = 0$
> $\implies \boxed{\underline{v} \perp \underline{w}}$