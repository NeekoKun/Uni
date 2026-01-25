#analisi 
> [!error] Teorema
> 1. Se $\exists \lim_{  x \to x_{0} } f(x) = l$, con $x_{0}, l \in \overline{\mathbb{R}}$, e se $l > 0$ allora $f(x) > 0$ definitivamente per $x \to x_{0}$
> 2. Se $f(x) \geq 0$ definitivamente per $x \to x_{0}$, e se $\exists \lim_{  x \to x_{0} } f(x) = l: l,x_{0} \in \overline{\mathbb{R}}$ allora $l \geq 0$

> [!info] Osservazione
> Se $f(x) > 0$ definitivamente per $x \to x_{0}$, ed $\exists \lim_{  x \to x_{0} } f(x) = l: l, x_{0} \in \overline{\mathbb{R}}$ allora $l \geq 0$ ma potrebbe essere $l = 0$

> [!error] Dimostrazione
>Pt. 1:
>Se $\lim_{ x \to x_{0} }f(x) = l> 0$ allora $\exists\ u(x_{0})$ intorno di $x_{0}$ tale che $f(x_{0}) > 0 \forall\ x \in u(x_{0}), x \neq x_{0}$
>Con definizione metrica caso $x_{0}, l \in \mathbb{R}$
>Poiché $\lim_{ x \to x_{0} } f(x) = l > 0$ $$\forall\ \epsilon > 0 \exists \delta > 0 : 0 < |x - x_{0}| < \nabla ta \implies l - \epsilon < f(x) < l + \epsilon$$
>scegliamo $\epsilon = \frac{l}{2} > 0$ troviamo che $$\forall\ x \in (x_{0}- \delta, x_{0} + \delta), x \neq x_{0}$$ vale $$f(x) > l - \epsilon = l - \frac{l}{2} = \frac{l}{2} > 0$$
>
> Pt. 2:
> Se $x_{n}$ è una successione tale che $x_{n} \in D \forall\ n, x_{n} \neq x_{0} \forall\ n, \lim_{ n \to \infty }x_{n} = x_{0}$ allora $\lim_{ x \to \infty } f(x_{n}) = l$, per definizione successionale di limite.
> Poiché $x_{n} \to x_{0}$ e poiché definitivamente $x \to x_{0},\ f(x) \geq 0$, deve essere $f(x_{n}) \geq 0$ definitivamente in $n \in \mathbb{N}$.
> Poiché abbiamo visto che $l = \lim_{ n \to \infty } f(x_{n})$, per il teorema di permanenza del segno per successioni deve esere $$l = \lim_{ n \to \infty } f(x_{n}) \geq 0$$
> 