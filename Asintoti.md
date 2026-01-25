#analisi 

## Asintoto Orizzontale
> [!warning] Definizione
> Si dice che una funzione ha asintoto orizzontale $y = l$ con $l \in \mathbb{R}$ per $x \to +\infty$ se $\lim_{ x \to \infty } f(x) = l$

> [!warning] Definizione
> Se $l \in \mathbb{R},\ x_{0} \in \mathbb{R}$ si dice che $$\lim_{ x \to x_{0} } f(x) = l^+ $$
> se $\lim_{ x \to x_{o} }f(x) = l$ ed inoltre $\exists\ u(x_{0})$ intorno di $x_{0}$ tale che
> $$f(x) \geq l\ \forall\ x \in u(x_{0}),\ x \neq x_{0}$$

> [!info] Osservazione
> - $\lim_{ x \to \infty }f(x) = l^+,\ l \in \mathbb{R}$
> $\forall\ \epsilon > 0\ \exists\ M > 0 :$ $$x > M \implies l \leq f(x) < l + \epsilon$$

## Asintoto Obliquo
> [!warning] Definizione
> Si dice che una funziona ha **Asintoto Obliquo** $y =mx+q$ con $m \in \mathbb{R}\setminus \{ 0 \}$ e $q \in \mathbb{R}$, per $x \to +\infty$ se $$\lim_{ x \to \infty } (f(x) - (mx + q)) = 0$$

> [!info] Osservazione
> $\lim_{ x \to \pm\infty } f(x) - (mx + q) = 0$ equivale a $$f(x) - (mx + q) = \sigma(1)\ \ x \to \pm \infty$$ $$f(x) = mx + q + \sigma(1)\ \ x \to \pm \infty$$

> [!error] Proposizione
> $f$ ha asintoto obliquo a $\pm \infty$ se e solo se:
> 1. $\lim_{  x \to \pm\infty } \frac{f(x)}{x} = m \in R\setminus\{ 0 \}$
> 2. $\lim_{ x \to \pm\infty } f(x) - mx = q \in \mathbb{R}$

## Asintoto Verticale

> [!warning] Definizione
> Se $x_{0} \in \mathbb{R}$ e $$\lim_{ x \to \pm\infty } f(x) = \pm \infty$$
> allora diremo che $x = x_{0}$ è un Asintoto Verticale per $f$