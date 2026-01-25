#analisi 
> [!error] Teorema
> Sia $g$ definita in un intorno di $x_{0}$ e continua in $x_{0}$, cioè $\lim_{ x \to x_{0} } g(x) = g(x_{0})$, sia $f$ definita in un intorno di $t_{0} = g(x_{0})$ e continua in $t_{0}$, cioè $\lim_{ t \to t_{0} }f(t) = f(t_{0})$. 
> Allora $f\circ g (x)$ è definita in un intorno di $x_{0}$ ed è continua in $x_{0}$. cioè $$\lim_{ x \to x_{0} } f(g(x)) = f(g(x_{0}))$$

> [!error] Dimostarzione
> Per il teorema di cambio di variabile nei limiti, essendo entrambe funzioni continue $$\lim_{ x \to x_{0} } f(g(x)) = \lim_{ t \to t_{0} } f(t) = f(t_{0}) = f(g(x_{0}))$$

> [!info] Osservazione
> $\lim_{ x \to x_{0} } f(g(x)) = f(g(x_{0})) = f(\ \lim_{ x \to x_{0} } g(x)\ )$