#AM2 
> [!abstract] Definizione
> $$y'(x) = f(x)g(y)$$

## Risoluzione
> [!info] Osservazione
> La funzione costante $y(x) = a \in \mathbb{R}$ è una soluzione solo nel caso in cui $g(a) = 0$:
> $$y(x) = a \implies y'(x) = 0 \implies 0 = f(x) g(a)$$
> $$\implies 0 = 0$$

- Supponendo quindi che $g(y) \neq 0$:

> [!warning] Soluzione
> $$y'(x) = \frac{dy}{dx} \implies \frac{dy}{dx} = f(x)g(y)$$
> $$\implies \int\frac{dy}{g(y)} = \int f(x)dx$$
> Considerando $G(y) = \int \frac{1}{g(y)}dy$ e $F(x) = \int f(x)dx$
> $$G(y) = F(x) + C;\ \ \ C \in \mathbb{R}$$
> E se $\exists G^{-1}(y)$ allora
> $$\boxed{y(x) = G^{-1}(F(x) + C);\ \ \ C \in \mathbb{R}}$$