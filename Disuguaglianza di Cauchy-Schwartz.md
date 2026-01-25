#GAL 
> [!error] Teorema
> $|<\underline{v}, \underline{w}>| \leq ||\underline{v}|| \cdot ||\underline{w}||$

> [!error] Dimostrazione
> Fissiamo $\underline{v}, \underline{w} \in V$.
> - Se $\underline{w} = \underline{0} \implies |<\underline{v}, \underline{0}>| \leq ||\underline{v}|| \cdot 0 = 0$
> - Se $\underline{w} \neq \underline{0}$ abbiamo $|<\underline{v}, \underline{w}>| = \pm <\underline{v}, \underline{w}>$
> 	- Supponiamo $|<\underline{v}, \underline{w}>| = -<\underline{v}, \underline{w}>$
> 	Definiamo una funzione $p: \mathbb{R} \to \mathbb{R}$ $$p(t) = ||\underline{v} - t \underline{w}||^2$$ $$= ||\underline{v}||^2 + t^2||\underline{w}||^2 -2t<\underline{v}, \underline{w}>$$ Allora $p(t)$ è un polinomio di II grado non negativo (perché $||\underline{v} - t\underline{w}||^2 \geq 0\ \forall\ t \in \mathbb{R}$) $$ \implies \Delta = (-2<\underline{v}, \underline{w}>)^2 - 4||\underline{w}||^2||\underline{v}||^2 \leq 0$$ $$\implies 4|<\underline{v}, \underline{w}>|^2 \leq 4||\underline{w}||^2||\underline{v}||^2$$ $$\implies \boxed{|<\underline{v}, \underline{w}>| \leq ||\underline{v}||\cdot||\underline{w}||}$$