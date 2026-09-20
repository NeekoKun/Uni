#AM2 
> [!abstract] Definizione
> $$y'(x) + a(x)y(x) = g(x)$$
## Formula Risolutiva
Per il caso generale
$$y'(x) +a(x)y(x) = g(x)$$
$$a, g : I \subseteq \mathbb{R} \in \mathbb{R}$$
Definiamo una qualsiasi primitiva
$$A(x) = \int a(x)dx$$
allora
> [!warning] Soluzione
> $$y(x) = e^{-A(x)}\left( C + \int e^{A(x)}g(x)dx \right)$$

Nel caso in cui sia definito un certo valore per $y(x_{0})$ stiamo risolvendo un [[Problema di Cauchy]]

# Equazione Omogenea
> [!abstract] Definizione
> se $g(x) \approx 0$, l'equazione si dice ==omogenea==:
> $$y'(x) + a(x)y(x) = 0$$

## Formula Risolutiva
Per il teorema precedente, vale
> [!warning] Soluzione
> $$y(x) = Ce^{-A(x)};\ \ \ C \in \mathbb{R}$$

## Step Risolutivi
1. Portare l'equazione nella formula generica, e.g. $$y' = 4xy +x^3 \implies y' - 4xy=x^3$$
2. Riconoscere le funzioni, e.g. $$a(x) = -4x,\ \ g(x) = x^3$$
3. Risolvere l'integrale generale