> [!error] Teorema
> Sia $f:(a,b) \to \mathbb{R},\ x_{0}\in(a,b)$, $f$ derivabile n-volte in $x_{0}$, $n \geq 0$
> Allora per $x \to x_{0}$
> $$f(x) = P_{n}(x) + \sigma((x-x_{0})^n)$$
> Dove $P_{n}$ è il [[Polinomio di Taylor]] e $\sigma((x-x_{0})^n)$ è il **Resto di Peano**
> Cioè
> $$\lim_{ x \to x_{0} } \frac{f(x) - \sum\limits_{k=0}^n \frac{f^{(k)}(x)}{k!}(x-x_{0})^n}{(x-x_{0})^n} = 0$$

> [!error] Dimostrazione
> Dimostrazione per induzione

## Corollari
> [!error] Corollario
> Sia $f: (a,b) \to \mathbb{R}$ derivabile $n$ volte in $x_{0} \in (a,b)$, con $n \geq 2$ e $$f'(x_{0}) = f''(x_{0}) = \dots = f^{(n-1)}(x_{0}) = 0$$
> e $f^{(n)}(x_{0}) \neq 0$ allora
> 1. Se $n$ è dispari, $x_{0}$ è un [[Flesso]]
> 2. Se $n$ è pari:
> 	1. Se $f^{(n)}(x_{0}) > 0$, $x_{0}$ è un minimo
> 	2. Se $f^{(n)}(x_{0}) < 0$, $x_{0}$ è un massimo

> [!error] Dimostrazione
> --no dim--