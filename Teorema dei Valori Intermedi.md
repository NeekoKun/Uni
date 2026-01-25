#analisi 
> [!error] Teorema
> Generalizzazione del [[Teorema degli Zeri]]
> Sia $f: I \to \mathbb{R}$ continua con $I \subseteq \mathbb{R}$ intervallo allora se $y_{1}, y_{2} \in \Im(f)$, per ogni $\lambda \in \mathbb{R}$ compreso tra $y_{1}$ e $y_{2}$, $\exists\ x_{0} \in I : f(x_{0}) = \lambda$

> [!error] Dimostrazione
> Siano $y_{1},y_{2} \in \Im(f) \subseteq \mathbb{R}$, supponiamo $y_{1} \leq y_{2}$. Dunque $\exists\ x_{1}, x_{2} \in I : f(x_{1}) = y_{1};\ f(x_{2}) = y_{2}$
> - Se $\lambda = y_{1} \lor y_{2}$ -> risolto
> - Se $\lambda \in (y_{1};\ y_{2})$ per comodità supponiamo $x_{1} < x_{2}$.
> Poiché $x_{1}, x_{2} \in I$ e $I$ Intervallo, $[x_{1},x_{2}] \subseteq I$. Costruiamo la funzione ausiliaria $$g: [x_{1};\ x_{2}] \to \mathbb{R}$$ $$g(x) = f(x) - \lambda$$
> Allora $g$ è continua, perché $f$ è continua in $[x_{1},x_{2}]$.
> Inoltre: $$g(x_{1}) = f(x_{1}) - \lambda = y_{1} - \lambda < 0$$ $$g(x_{2}) = f(x_{2}) - \lambda = y_{2} - \lambda > 0$$
> Per il [[Teorema degli Zeri]] applicato alla funzione continua $g$, $\exists\ x_{3} \in [x_{1};\ x_{2}] : g(x) = 0$, quindi: $g(x_{3}) = f(x_{3}) - \lambda = 0 \implies \boxed{f(x_{3}) = \lambda}$
