#analisi
$\forall\ x, y, z \in \mathbb{R}$:
- $|x + y| \leq |x| + |y|$
- $|x-y| \leq |x-z| + |z-y|$
---
#GAL 
> [!error] Teorema
> $||\underline{v} + \underline{w}|| \leq ||\underline{v}|| + ||\underline{w}||$

> [!error] Dimostrazione
> $||\underline{v} + \underline{w}||^2 = ||\underline{v}||^2 + ||\underline{w}||^2 +  2<\underline{v}, \underline{w}>$ per [[Teorema di Carnot]]
> $$\leq ||\underline{w}||^2 + ||\underline{w}||^2 + 2 |<\underline{v}, \underline{w}>|$$
> Per [[Disuguaglianza di Cauchy-Schwartz]]
> $$\leq ||\underline{v}||^2 + ||\underline{w}||^2 + 2 \cdot ||\underline{v}|| \cdot ||\underline{w}|| = (||\underline{v}|| + ||\underline{w}||)^2$$
> $$\implies \boxed{||\underline{v}, \underline{w}|| \leq ||\underline{v}|| + ||\underline{w}||}$$