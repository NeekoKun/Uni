#analisi 
> [!error] Teorema
> Se $f : [a,b] \to \mathbb{R}$ è continua in $[a,b]$ e $x_{0} \in [a,b]$ allora $F:[a,b] \to \mathbb{R}$
> $$F(x) = \int_{x_{0}}^x f(t) dt$$
> è derivabile in $x,\ \forall\ x \in [a,b]$ e vale $F'(x) = f(x),\ \forall\ x \in [a,b]$

> [!error] Dimostrazione
> Se $x \in  [a,b]$, $h \in \mathbb{R}$ tale che $x+h \in [a,b]$ allora
> $$\frac{F(x+h) - F(x)}{h} = \frac{1}{h} \left( \int_{x_{0}}^{x+h} f(t)dt + \int_{x_{0}}^{x} f(t)dt \right) = \frac{1}{h}\int_{x}^{x+h} f(t) dt$$
> - $h > 0$, la funzione è il valore medio di $f$ sull'intervallo $[x, x+h]$.
> Poiché $f$ è continua, per il [[Teorema della Media Integrale]] $\exists\ x_{h} \in [x, x+h]$ tale che
> $$\frac{1}{h}\int_{x}^{x+h}f(t)dt = f(x_{h})$$
> Per il [[Teorema dei due Carabinieri]], essendo
> $$x \leq x_{h} \leq x+h$$ vale $\lim_{ h \to 0 } x_{h} = x$
> essendo $f$ continua $$\lim_{ h \to 0 } f(x_{h}) = f(x)$$ pertanto $$\lim_{ h \to o^+ } \frac{F(x+h) - F(x)}{h} = \lim_{ h \to o^+ } f(x_{h}) = f(x)$$
>
> - Similmente è dimostrabile per $h < 0$
>
> $\implies\ \exists$ finito $$\boxed{F'(x) = \lim_{ h \to 0 } \frac{F(x+h) - F(x)}{h} = f(x)}$$

## Corollari
> [!error] Corollario
> Se $f: [a,b] \to \mathbb{R}$ è continua, essa è [[Integrale di Riemann|Riemann-Integrabile]] in $[a,b]$ ed ammette primitive in $[a,b]$, tutte e sole della forma $$F(x) = \int_{a}^x f(t) \, dt + C$$
> con $C \in \mathbb{R}$ arbitrario. Inoltre per qualunque primitiva $G$ di $f$ in $[a,b]$ vale $$\int_{a}^b f(t) \, dt = G(b) - G(a)$$

> [!error] Dimostrazione
> Applicazione del Teorema Precedente e del [[Teorema di Caratterizzazione dell Primitive di una Funzione]] su un intervallo.
> Inoltre se $G$ è primitiva di $f$ in $[a,b]$ allora $\exists\ C \in \mathbb{R}$ tale che $$G(x) = \int_{a}^x f(t) \, dt + C$$ e vale $$G(b) - G(a) = \int_{a}^b f(t) \, dt$$

> [!info] Osservazione
> è il [[Teorema Fondamentale del Calcolo Integrale I]] per funzioni $f: [a,b] \to \mathbb{R}$ continue