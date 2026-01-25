#analisi 
> [!error] Teorema
> Sia $f: I \subseteq \mathbb{R} \to \mathbb{R}$, $I$ intervallo, allora $f$ costante in $I \Leftrightarrow f$ derivabile in $I$ e $f'(x) = 0\ \forall\ \\ x \in I$

> [!error] Dimostrazione
> - Se $f$ è costante, allora $$f(x) = \lambda \in \mathbb{R}$$ $$\implies f'(x) = \lim_{ h \to 0 } \frac{f(x+h) - f(x)}{h} = \lim_{ h \to 0 } \frac{\lambda - \lambda}{h}$$ $$\implies f'(x) = 0$$
> - Viceversa, siano $x_{1}, x_{2} \in I$ arbitrari.
> Per comodita, sia $x_{1} < x_{2}$. Vogliamo dimostrare che $f(x_{1}) = f(x_{2})$ nell'ipotesi del teorema
> Consideriamo la funzione $$f: [x_{1}, x_{2}] \to \mathbb{R}$$ allora, essendo $[x_{1},x_{2}] \subseteq I$, allora sarà derivabile e quindi continua in $[x_{1},x_{2}]$.
> Per il [[Teorema del Valore Medio di Lagrange]] $\exists c \in [x_{1},x_{2}] :$ $$f'(c) = \frac{f(x_{2} - f(x_{1}))}{x_{2} - x_{1}}$$ $\implies f(x_{2}) - f(x_{1}) = f'(c)(x_{2} - x_{1})$.
> Poichè abbiamo $f'(x) = 0\ \forall\ x \in I$ per ipotesi, allora $f'(c) = 0$. Segue che $$f(x_{2}) - f(x_{1}) = 0 \implies f(x_{2}) = f(x_{1})$$ $$\implies \boxed{f(x) \text{ è costante}}$$ 

> [!info] Osservazione
> Se $f: D(f) \subseteq \mathbb{R} \to \mathbb{R}$, e $D(f)$ non è un intervallo, può accadere che $f'(x) = 0\ \forall\ x \in D(f)$, ma che $f(x)$ non sia costante. E.g.: $$\begin{cases}-1 & x < 0 \\ 1 & x > 0\end{cases}$$