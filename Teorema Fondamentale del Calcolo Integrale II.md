#analisi 

> [!error] Teorema
> sia $f:[a,b] \to \mathbb{R}$ [[Integrale di Riemann|Riemann-Integrabile]] in senso proprio o improprio in $[a,b]$ e sia $x_{0} \in [a,b]$. Sia $F:[a,b] \to \mathbb{R}$
> $$F(x) = \int_{x_{0}}^x f(t) \, dt$$
> Allora
> 1. $F$ è continua in $[a,b]$
> 2. Se $f$ è continua in $\overline{x} \in [a,b]$ allora $F$ è derivabile in $\overline{x}$ e vale $F'(\overline{x}) = f(\overline{x})$

> [!error] Dimostrazione
> -- no dim --

## Corollari
> [!error] Corollario
> Sia $f:\mathbb{R} \to \mathbb{R}$ continua, e siano $a(x), b(x) : \mathbb{R} \to \mathbb{R}$ derivabili.
> Consideriamo $$G(x) = \int_{a(x)}^{b(x)} f(t) \, dt$$
> Allora $G$ è derivabile e vale $$G'(x) = b'(x)f(b(x)) - a'(x)f(a(x))$$
> per il [[Teorema della Catena]]

> [!error] Dimostrazione
>  Per il [[Teorema della Catena]] sia $x_{0} \in \mathbb{R}$ e sia $$F(x) = \int_{x_{0}}^x f(t) \, dt$$
>  Allora $F$ derivabile e $F'(x) = f(x)\ \forall\ x \in \mathbb{R}$. inoltre
>  $$G(x) = \int_{a(x)}^{b(x)}f(t) \, dt = \int_{x_{0}}^{b(x)} f(t) \, dt - \int_{x_{0}}^{a(x)} f(t)$$