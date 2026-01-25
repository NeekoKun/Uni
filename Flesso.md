#analisi 
> [!warning] Definizione
> Data $f: (a,b) \to \mathbb{R},\ x_{0} \in (a,b)$, $f$ derivabile in $x_{0}$,
> $x_{0}$ è detto **Punto di Flesso** di $f$ se $\exists\ \delta > 0:$
> $$f(x) \geq f'(x_{0}) + f(x_{0})(x-x_{0}),\ \forall\ x \in [x_{0}, x_{0}-\delta)$$
> $$f(x) \geq f'(x_{0}) + f(x_{0})(x-x_{0}),\ \forall\ x \in (x_{0} - \delta, x_{0}]$$

> [!info] Osservazione
> Con abuso di notazione, per estensione, se $f$ è continua in $x_{0}$, $f'(x_{0})= \pm \infty$, con retta tangente verticale in $x_{0}$, diremo ancora che $x_{0}$ è **Punto di Flesso** per $f$


## Cambio di Concavità
> [!warning] Definizione
> Data $f: (a,b) \to \mathbb{R},\ x_{0} \in (a,b)$, $f$ derivabile in $x_{0}$,
> $x_{0}$ è detto **Punto di Cambio di Concavità** se $\exists\ \delta > 0:$
> $$[x_{0}, x_{0}+\delta) \text{ è concavo (convesso)}$$
> $$(x_{0}-\delta, x_{0}] \text{ è convesso (concavo)}$$

> [!info] Osservazione
> Se esiste la retta tangente, tutti i punti di cambio di concavità sono punti di cambio di flesso

> [!error] Teorema
> Si $f:(a,b) \to \mathbb{R}, x_{0} \in (a,b)$, $f$ è derivabile 2 colte in $x_{0}$ e $x_{0}$ punto di flesso per $f$, allora $f''(x_{0}) = 0$