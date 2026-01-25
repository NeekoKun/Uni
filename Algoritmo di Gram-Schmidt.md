#GAL 
> [!error] Algoritmo
> Sia $H \subseteq V$ con base $C = \{ \underline{v}_{1}, \dots \underline{v}_{d} \}$
> e output Base [[Base Ortogonale e Ortonormale|Ortonormale]] $B = \{ \underline{b}_{1}, \dots, \underline{b}_{d} \}$ di $H$
> 1. $\underline{b}_{1} = \dfrac{\underline{v}_1}{||\underline{v}_{1}||} \to H_{1} = \mathrm{Span}(\underline{b}_{1}) = \mathrm{Span}(\underline{v}_{1})$
> 2. $\underline{w}_{n} = \underline{v}_{n} - \pi_{H_{n-1}}(\underline{v}_{n}) \in H_{n-1}^\perp$
> $\underline{b}_{n} = \dfrac{\underline{w}_{n}}{||\underline{w}_{n}||} \to H_{n} = \mathrm{Span}(\underline{b}_{1}, \dots, \underline{b}_{n}) = H_{n-1} + \mathrm{Span}(\underline{b}_{n}) = \mathrm{Span}(\underline{v}_{1}, \dots, \underline{v}_{n})$
> 3. $\underline{w}_{d} = \underline{v}_{d} - \pi_{H_{d-1}}(\underline{v}_{d}) \in H_{d-1}^\perp$
> $\underline{b}_{d} = \dfrac{\underline{w}_{d}}{||\underline{w}_{d}||} \to H_{d} = \mathrm{Span}(\underline{b}_{1}, \dots, \underline{b}_{d}) = H_{d-1} + \mathrm{Span}(\underline{b}_{d}) = \mathrm{Span}(\underline{v}_{1}, \dots, \underline{v}_{d})$