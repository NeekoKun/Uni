#AM2 
> [!info] Definizione
> Un'equazione generale di Bernoulli è della forma
> $$y'(x) = a(x)y(x) + b(x)y^\alpha(x);\ \ \ \alpha \in \mathbb{R} \setminus \{ 0, 1 \}$$

> [!warning] Risoluzione
> Dividento ambo le parti per $y^\alpha(x)$
> $$\frac{y'(x)}{y^\alpha(x)} = a(x)y^{1-\alpha}(x) + b(x)$$
> Ponendo poi $y^{1-\alpha}(x) = z(x)$
> ossia, derivando: $(1-\alpha)y^{-\alpha}(x)y'(x) = z'(x)$
> Otteniamo $$\frac{z'(t)}{1-\alpha} = a(x)z(x) + b(x)$$
> $$\implies \boxed{z'(x) + (\alpha-1)a(x)z(x) = (1-\alpha)b(x)}$$
> Giungendo dunque ad una [[EDO del Primo Ordine Lineari|EDO del Primo Ordine Lineare]]