#GAL 
> [!info] Osservazione
> Siano $\underline{v}, \underline{w} \neq \underline{0} \implies ||\underline{v}||, ||\underline{w}|| \neq 0$
> Per [[Disuguaglianza di Cauchy-Schwartz]] $$\implies \frac{|<\underline{v}, \underline{w}>|}{||\underline{v}|| \cdot ||\underline{w}||} \leq 1 \implies-1 \leq \frac{<\underline{v}, \underline{w}>}{||\underline{v}|| \cdot ||\underline{w}||} \leq 1$$

> [!warning] Definizione
> L'**angolo** tra $\underline{v}$ e $\underline{w}$ è $$\widehat{\underline{v}\ \underline{w}} = \arccos\left( \frac{<\underline{v}, \underline{w}>}{||\underline{v}|| \cdot ||\underline{w}||} \right)$$

> [!info] Osservazione
> - $\cos(\widehat{\underline{v}\ \underline{w}}) = \frac{<\underline{v}, \underline{w}>}{||\underline{v}|| \cdot ||\underline{w}||}$
> - $\widehat{\underline{v}\ \underline{w}} = \frac{\pi}{2} \Leftrightarrow\ <\underline{v}, \underline{w}> = 0$

> [!warning] Definizione
> $\underline{v}, \underline{w}$ sono **ortogonali** $\underline{v} \perp \underline{w} \leftrightarrow\ <\underline{v}, \underline{w}> = 0$

> [!error] Proposizione
> Se $\underline{v}_{1}, \dots, \underline{v}_{n} \neq 0$ ortogonali a 2 a 2 allora sono **Linearmente Indipendenti**

> [!error] Dimostrazione
> Supponiamo $$\sum_{i=1}^{n} c_{i}\underline{v}_{i} = \underline{0}$$ per qualche $c_{i} \in \mathbb{R}$
> Fissiamo un $j \in [1, n]$ e consideriamo $$0 = <\underline{v}_{j}, \underline{0}> = <\underline{v}_{j}, \sum_{i=1}^{n} c_{i}\underline{v}_{i}> \overset{Bilinearità}{=} \sum_{i=1}^{n} c_{i} <\underline{v}_{j}, \underline{v}_{i}>$$
> Per ipotesi, $<\underline{v}_{j}, \underline{v}_{i}> = 0$ se $i \neq j$
> $$= c_{j} <\underline{v}_{j}, \underline{v}_{j}> = c_{j}||\underline{v}_{j}||^2$$
> $$\implies c_{j}||\underline{v}_{j}||^2 = 0$$
> Ma per ipotesi $||\underline{v}_{j}||^2 \neq 0 \implies c_{j} = 0$
- [[Teorema del Coseno]]
